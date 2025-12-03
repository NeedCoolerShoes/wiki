# Working with Embeds

NeedCoolerShoes allows users to embed a 3D preview of any public / unlisted skin, on to their own site.

This guide assumes that the reader is familiar with basic HTML. We will be working with [iframes](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe).

## Step 1: Getting the iframe Code

First, browse to the skin you want to embed. Visit its page, and then click the **Sharing & Attribution** button.

<figure>
  <img src="https://res.cloudinary.com/needcoolershoes/image/upload/v1764720322/EmbedGuide2025_ksrgkp.png" alt="Skin Page">
  <figcaption>The open Sharing & Attribution menu</figcaption>
</figure>

Where it says '**Embed Skin**', copy the iframe code from within the text area.

## Step 2: Embedding it on your Own Site

The next step is to paste the iframe in to the code of your website. In the next step, we'll discuss making it look good, but for now we just want something that works.

<figure>
  <img src="https://res.cloudinary.com/moxvallix/image/upload/v1720160527/NeedCoolerShoes/guides/working-with-embeds-2_nzt5ma.png" alt="Example HTML">
  <figcaption>Some example code, with the iframe.</figcaption>
</figure>

Once you have added it to your HTML, open it in your browser and confirm the skin is loading correctly. If it is, move to [Step 3](#step-3-customization).

### Help! The iframe is just showing an error message!

Firstly, make sure the skin is not set to private. Private skins cannot be embedded.

If it's not private, it's likely you have CSP on your website. Explaining CSP is out of scope for this guide, but [here is a great MDN article on the topic](https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP).

You will need to add the following policy to your CSP:

`frame-src needcoolershoes.com;`

## Step 3: Customization

The iframe itself can be styled much like any other element. You can resize it to any size you like; the skin will scale to fit the given size.

Unfortunately, due to limitations with iframes that exist for security reasons, CSS on your site cannot style content within the iframe.

As such, the embed URL has some [parameters](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/What_is_a_URL#parameters) that can be set to change the style of the embed. They are as follows.

| Name | Values | Description |
| --- | --- | --- |
| color | [A CSS Color](https://developer.mozilla.org/en-US/docs/Web/CSS/color). | Changes the text color of the link to NeedCoolerShoes. |
| scale | A decimal number, recommended to be between 0 and 1. | Changes the initial zoom level of the skin. |
| username | Any text. | Sets the username to be displayed on the skin. |
| position | `top-left`, `top-right`, `bottom-left` or `bottom-right`. | Configures where the link should be placed. |

### An Example:

`https://needcoolershoes.com/skins/1/embed?color=green&username=Moxvallix`

Using the URL above in the iframe will render the NeedCoolerShoes link in green, and set the skin's username to Moxvallix.
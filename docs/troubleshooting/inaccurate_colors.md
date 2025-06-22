# Help! My colors are inaccurate!

While using the editor, you might have received a pop-up saying "Color inaccuracies detected!", this is usually due to tracking protections that the browsers have. While it is fairly easy to solve this, it can be very annoying when exporting your skin.

Here is a list of browsers and their associated features that cause this bug:

| Browser | Feature | Affected Versions/OS |
| --- | --- | --- |
| Firefox | Private Tab | Mobile and Desktop |
| Librewolf | Normal Tab | All versions on Desktop |
| Brave | Brave Shield | Mobile and Desktop |
| Safari | Normal Tab | iOS 18.5 |

## Firefox
This issue could be caused by one of two things. Firstly, try disabling Enhanced Tracking Protection by clicking the shield icon in your
URL bar, and then toggling off Enhanced Tracking Protection. For more help, consult [this guide](https://support.mozilla.org/en-US/kb/enhanced-tracking-protection-firefox-desktop#w_what-to-do-if-a-site-seems-broken).

If the issue persists even after turning off Enhanced Tracking Protection for the site, you may have Resist Fingerprinting enabled. Changing this
unfortunately cannot be done on a per-site basis, so the improved privacy benefits from it will be lost on all sites when disabled. If this is
something you purposefully set up, it may be worth creating a different Firefox profile to use for sites that need it disabled.

To disable Resist Fingerprinting, follow [this guide](https://support.mozilla.org/kb/resist-fingerprinting#w_how-to-tell-if-you-have-resist-fingerprinting-enabled-and-if-so-disable-it)

## Librewolf
Librewolf defaults to have both Resist Fingerprinting, and Enhanced Tracking Protection set up in such a way to cause the issue. Follow the same
steps in the [Firefox](#firefox) section to resolve the issue.

## Brave
Disabling Brave Shield should fix this problem. Brave Shield is usually located to the right side of the adress bar on both Mobile and Desktop.

## Safari

Unknown. If you find a solution please contact us, in the meanwhile you can use Firefox or any other browser that doesn't have this bug.
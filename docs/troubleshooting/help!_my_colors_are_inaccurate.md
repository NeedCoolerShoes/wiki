# Help! My colors are inaccurate!

While using the editor, you might have received a pop-up saying "Color inaccurasies detected!", this is usually due to tracking protections that the browsers have. While it is fairly easy to solve this, it can be very annoying when exporting your skin.

Here is a list of browsers and their associated features that cause this bug:

| Browser | Feature | Affected Versions/OS |
| --- | --- | --- |
| Librewolf | Unknown | All versions on Desktop |
| Brave | Brave Shield | Mobile and Desktop |
| Firefox | Private Tab,  | Mobile and Desktop |
| Safari | Normal Tab | iOS 18.5 |

## Librewolf

Unknown. If you find a solution please contact us, in the meanwhile you can use Firefox or any other browser that doesn't have this bug.

## Brave

Disabling Brave Shield should fix this problem. Brave Shield is usually located to the right side of the adress bar on both Mobile and Desktop.

## Firefox

This bug is usually caused by the `privacy.resistFingerprinting` and `privacy.resistFingerprinting.randomization.canvas.use_siphash` config flags. These are enabled in the Private Tab by default. If you are not using the private tab and still have this bug. Visit the `about:config` page and change these values to false.

## Safari

Unknown. If you find a solution please contact us, in the meanwhile you can use Firefox or any other browser that doesn't have this bug.
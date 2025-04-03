## Description
The **Shade** tool allows you to easily shade your skin without manually changing colors. You can change the **Force** value to do more coarse/subtle adjustments.
## How to use
- Hold the **Left Mouse Button** to make pixels **Darker**
- Hold the **Right Mouse Button** to make pixels **Brighter**
## Modifiers
- **Force** - Adjusts how much the tool shades pixels 

## Math
The **Shade** tool calculates the brightness using simple **addition/subtraction** from the original color by the **Force** value. Here's an example:<br>
Let's say an user left clicked on a pixel with the color `#F69901` using the **Shade** tool with the **Force** value set to 5, here's how to calculate the resulting color:<br>

- First thing to do is to convert the hexadecimal`#F69901` to a decimal value. the result would be `246, 153, 1`
- Next, the **Force** value has to be subtracted from the decimal values, so the result would be:<br>
  246 - 5 = 241<br>
  153 - 5 = 148<br>
  1 - 5 = -4
!!! info
    The values get clamped between 0 and 255, if a value is negative, it gets clamped to 0 and if the value is higher than 255, it gets clamped back to 255 
- Lastly, we convert the value `241,148,0` is converted back to hexadecimal, the result is `#f19400`

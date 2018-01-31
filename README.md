# macropad-calculator

Current KLE Designs:

[keyboard-layout-editor](http://www.keyboard-layout-editor.com/#/gists/c2c9d6496090510a4558f0a1e2d1008c)

## Design ideas

* Project inspired by G80-9009 built-in calculator and functions.
* Also drawing inspiration from the old HP 35/45 calculators for **RPN**, functions and color scheme.
* The "Paste" function key takes the current value and:
    * Pastes the numeric text into the data stream of the keyboard and onto the computer, and
    * exits Calculator mode.
* Expecting to hand-wire it.
* Geekhack [macropad project](https://geekhack.org/index.php?topic=85874.0) -- no display.
* Arduino [trivial calculator](http://www.microcontroller-project.com/calculator-with-pic16f877-microcontroller.html) with 16x2 screen
* [Quick Key Adapter, 10 Button
Keyboard](http://www.instructables.com/id/Quick-Key-Adapter-10-Button-HID-
Keyboard/) PIC18F14K50. Complete parts kit: $25.00 (sold out) Programable w/Modifier keys.
* For full matrix would need this I/O:
    * USB
    * 10 pins = 6 x 4 matrix
    * 4 pins for LCD display
    * LED for Calc mode on/off?
    * Power control for LCD on/off (save power and use as Calc mode indicator
    * Plus something to control contrast(?)

## Features
* Unary operators:
    1/x, √, M+, M-, M store, M recall
* Binary operators:
    + -, *, /, CL X
* Others:
    x <==> y, rotate, Clear (all), Backspace, +/-, E EX, Paste, Enter


## Resources

* 22-key pad, metal, USB, without display, available @ Amazon, $22:
    https://www.amazon.com/Jelly-Comb-Responsive-Mechanical-Notebook/dp/B075NZBHY4/ref=sr_1_7
* H4JO 22 Key Numeric Keypad, Ice Blue, no display. Also $14.00 @ Wallmart:
    https://www.ebay.com/i/332471028408?chn=ps
* Ducky makes a Calc + Macro pad for $74.00. 23-key. Only 9 chatacter display
(I prefer 16, 2 lines). Expensive to buy "for parts."
   https://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=2249

* DIY numpad, case, display, $16, no usb:
    https://www.amazon.com/KKmoon-Calculator-Multi-purpose-Electronic-Electronics/dp/B076SBY7DG/ref=sr_1_1


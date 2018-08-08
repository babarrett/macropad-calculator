# macropad-calculator

Current KLE Designs:

[Jelly Comb](http://www.keyboard-layout-editor.com/#/gists/c2c9d6496090510a4558f0a1e2d1008c) based case design (no display included). 22 keys.

[Kensington](http://www.keyboard-layout-editor.com/#/gists/890397669938b2e2cf52ddd841844c0e) based case design, 1-line display, 30 keys, includes USB hub.

## Design ideas

* Project inspired by G80-9009 built-in calculator and functions.
* Also drawing inspiration from the old HP 35/45 calculators for **RPN**, functions and color scheme.
* The "Paste" (or "Send") function key takes the current value and:
    * Pastes the numeric text into the data stream of the keyboard and onto the computer, and
    * exits Calculator mode.
* Expecting to hand-wire it, but TBD.
* For full matrix would need this I/O:
    * USB
    * 10 pins = 6 x 4 matrix
    * 6 (maybe 4?) pins for LCD display
    * 1 pin + power transistor for Power control for LCD on/off (save power and use as Calc mode indicator)
    * Manual knob to control contrast

## Features
* Unary operators:
    1/x, √, M+, M-, M store, M recall, CL X
* Binary operators:
    \+ -, *, /
* Others:
    x <==> y, rotate, Clear (all), Backspace, +/-, E EX, Paste, Enter
* Modes: Set number od decimals to right of "." Hex/Decimal would be nice.
* Stack (at least 3 level)
* Memory (up to 10 addressable). M Store + #, where # is from 0 to 9, stores X into that memory. M Recall, # likewise.
* M Recall repeated could scroll through the stored addresses

## Useful Similar Projects:

* Geekhack [macropad project](https://geekhack.org/index.php?topic=85874.0) -- no display.
* Arduino [trivial calculator](http://www.microcontroller-project.com/calculator-with-pic16f877-microcontroller.html) with 16x2 screen
* [Full, scientific, RPN](https://forum.arduino.cc/index.php?topic=388331.0)
Arduino calculator. Simple(?) to wire? 64 bit floating point, battery powered.
Two line, about 16 character, green (LED?) display. Small keys, Hex/Decimal
modes, compiled to 32K on a 328p so no room for a boot loader.
* [Arduino LDC + 16
keys](https://www.allaboutcircuits.com/projects/simple-arduino-based-calculator/). 
Breadboarded. Used an UNO and LCD1602A display. 4 x 4 (16) keys. Integer arithmetic.
Pointer to: [BigNumber Library](http://www.gammon.com.au/forum/?id=11519)


## Resources

### Existing calculator + numeric entry keypads:

* Newegg [Kensington K72274US](https://www.kensington.com/us/us/6756/k72274us/laptop-keypadcalculator-with-usb-hub) 
(calculator 12 digit, one line, 19-key pad, 12 small keys = 31 total, USB hub, +2 ports) 
[Manual](https://accoblobstorageus.blob.core.windows.net/literature/1393.pdf)
* Amazon [HP CalcPad 200](https://www.amazon.com/HP-CalcPad-Calculator-Numeric-Keypad/dp/B002J6BUEI/)
28 keys. One line 12 digit LCD display. Flat keys. $16
* [I Focus 2 in 1 Wireless Numeric Keypad](https://www.amazon.com/Focus-Wireless-Calculator-Financial-Accounting/dp/B01N1Q2BP0/)
29 keys. Flat keys, wireless, $19
* Ducky makes a [Calc + Macro pad](https://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=2249) 
for $74.00. 23-key. Only 9 chatacter display (I prefer 16, 2 lines). Expensive to buy "for parts."
   

### Numeric pads only.
* 22-key pad, metal, USB, without display, available @ Amazon [Jelly Comb](https://www.amazon.com/Jelly-Comb-Responsive-Mechanical-Notebook/dp/B075NZBHY4/ref=sr_1_7), $22:
* [H4JO](https://www.ebay.com/i/332471028408?chn=ps) 22 Key Numeric Keypad, Ice Blue, no display. Also $19.00 @ ebay.
    

### Calculators only:

* [DIY Calculator](https://www.amazon.com/KKmoon-Calculator-Multi-purpose-Electronic-Electronics/dp/B076SBY7DG/ref=sr_1_1), 
case, 16 x 2 line, display, $16, no USB. With displays going for $10 this is a good price (if anything else in there is worth while.)
    


### Parts

* 16 x 2 LCD display [Adafruit](https://www.adafruit.com/product/181) $9.95. Requires 6 I/O pins.
* i2c / SPI character LCD backpack [Adafruit](https://www.adafruit.com/product/292) $9.95 assembled. Requires 2 I/O pins instead of 6.
* 16 x 2 LCD display [Jameco](https://www.jameco.com/z/181-Adafruit-Industries-Standard-LCD-16x2-White-on-Blue-with-Header-and-Contrast-Pot_2274919.html), $12.95
    - 6 pins to control
    - 8 custom glyphs
    - English/Japanese text
    - Hitachi HD44780U [datasheet](https://cdn-shop.adafruit.com/datasheets/HD44780.pdf).
* Enclosure:
    - https://www.okwenclosures.com/en/Comtec/A0615007.htm?var=f30d2022-633f-11e3-937d-00163e72470b
    - others



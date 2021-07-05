---
title: "micro:bit Pins"
date: 2021-06-20T21:04:11+01:00
draft: false
---

This week we will take a look at what we can do with the General Purpose Input Output (GPIO) pins. You can do a lot of things using the pins at the bottom of the micro:bit including using touch, connecting them to tinfoil, fruit, headphones or other electronic components using crocodile clips. You can even use them with add-on boards like motor controllers, LED screens and more.

<!--more-->

## MakeCode

1. open [MakeCode](https://makecode.microbit.org/#editor) within your favourite browser
2. Click on the **on start** block and drag it to the left and drop it in the bin. Do the same for the **forever** block
3. Click on **Input** Click and drag a **on p0 pressed** block to the code area and drop it
4. Click on **Basic** Click and drag a **show string "Hello!"** block to the code area and attach it within the **on p0 pressed** block


Your code is now complete and ready to download to your micro:bit.

**NOTE:** You can use this code different ways. You can just hold the GND pin and press pin 0 or you can glue some tinfoil to cardboard and connect the pins with crocodile clips.

Completed Code

![Completed Code within MakeCode](/Pins01.png)

## EduBlocks

1. Open [EduBlocks](app.edublocks.org) within your favourite browser
2. Click on **Basic** Click and drag a **from microbit import \*** block to the code area and drop it
3. Click on **Basic** Click and drag a **while True:** block to the code area and attach it under the **from microbit import \*** block
4. Click on **Basic** Click and drag a **if True:** block to the coding area and attach it within the **while True:** block
5. Click on **Pins** Click and drag a **pin 0.is_touched()** block to the code area and attach it where it says **True** in the **if** block
6. Click on **Display** Click and drag a **display.scroll("Hello World")** block to the code area and attach it within the **if pin 0.is_touched()** block

Your code is now complete and read to download to your micro:bit and try out.

Completed Code

![Completed Code within EduBlocks](/Pins02.png)

## Python

1. Open your favourite Python editor to use with the micro:bit
2. Type ```from microbit import *``` This imports the Python library for micro:bit so we can now interact with the micro:bit
3. Type ```while True:``` This creates a loop that will carry on while the conditions are true
4. Type ```if pin0.is_touched:``` Creating a condition on pin 0, so when pin 0 is touched
5. Type ```display.scroll("Hello World!")``` When pin 0 is touched Hello World! will scroll across the LED display.

Your code is now complete and ready to try out.

### Completed Code

```py
from microbit import *

while True:
    if pin0.is_touched:
        display.scroll("Hello World!")
```

## Conclusion

That's it for this week. Come back next Monday where we will dig into the pins a little bit deeper and create a simple robot.
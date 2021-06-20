---
title: "micro:bit LED Matrix"
date: 2021-06-20T20:37:40+01:00
draft: true
---

Within this post we are going to get to know what we can do with the LED matrix on the front of the micro:bit.

I will include code for the MakeCode, EduBlocks and microPython editors.

Lets get started!

<!--more-->

## Displaying Text

The first thing we will look at is to display text on the micro:bit, This could be used to send messages or used as a name badge.

### MakeCode

Here is how to display text using MakeCode:

1. Open the  MakeCode editor in your favourite browser [MakeCode](https://makecode.microbit.org)
2. Delete the **on start** block by clicking and dragging it to the left odf the screen and dropping it on the recycle bin.
3. Click on **Basic**. Click and drag a **show string "Hello!"** block to the code area and attach it within the **forever** code block.
4. Click on **Download** to download the code to your computer.
5. Plug your micro:bit into your computer using a microUSB cable.
6. Navigate to where your code downloaded to, This will normally be the downloads folder on your computer. Copy the file to the **MICROBIT drive**.

Once the code has copied to the micro:bit you will see **Hello!** scroll across the LED Matrix.

Completed Code

![Completed code for Displaying text on a micro:bit in MakeCode](/LEDMatrix01.png)

### EduBlocks

1. Open the EduBlocks editor in your favourite browser [EduBlocks](http://app.edublocks.org/)
2. Click on micro:bit.
3. Click on **Basic**. Click and drag a **from microbit import *** and drop it within the coding area.
4. Click on **Basic**. Click and drag a **while True:** block to the code area and attach it under **from microbit import ***.
5. Click on **Display**. Click and drag a **display.scroll("Hello World")** to the coding area and attach it within the **while True:** block.
6. Click on **Download Hex**, this will download the code to your computer.
7. Plug your micro:bit into your computer using a microUSB cable.
8. Navigate to where your code downloaded to, This will normally be the downloads folder on your computer. Copy the file to the **MICROBIT drive**.

Once the code has copied to the micro:bit you will see **Hello World** scroll across the LED Matrix.

Completed Code

![Completed code for displaying text on a micro:bit using EduBlocks](/LEDMatrix02.png)

### Python

There are two common ways to program the micro:but using microPython. The first one is to open the web version in your browser [Python](https://python.microbit.org/v/1) or by downloading the Mu editor from [downloading Mu](https://codewith.mu/en/download) (within this post I am using My)

1. Open your preferred method for programming Python.
2. Type ```from microbit import *``` this will import the micro:bit library to use with Python and press enter.
3. Type ```while True:``` this will create a while True loop meaning that the code inside it runs forever press enter.
4. Type ```display.scroll("Hello World")``` This will display Hello World on the micro:bit LED matrix forever.
5. Plug your micro:bit into your computer using a microUSB cable.
6. Click on **Flash**, this will download the code to your computer (if this gives you an error click **flash** again and it should work).

Completed code

``` Python
from microbit import *

while True:
    display.scroll("Hello World")
```

## Displaying Images

The other thing we can use the LED matrix for is displaying images. Let’s look and see what we can do by expanding on the code above.

### MakeCode

1. Click on **Basic**. Click and drag a **show  icon** block to the code area and attach it under the **show string "Hello!** code block.
2. Click on **Download** to download the code to your computer.
3. Navigate to where your code downloaded to, This will normally be the downloads folder on your computer. Copy the file to the **MICROBIT drive**.

Once the code has copied to the micro:bit you will see **Hello!+heart** scroll across the LED Matrix (see the simulator below).

you can also change the icons by clicking the white arrow next to the heart.

Completed Code

![Completed code to show Text and images together on a micro:bit using MakeCode](/LEDMatrix03.png)

### EduBlocks

1. Click on **Display**. Click and drag a **display.show(Image.HAPPY)** block to the code area and attach it under the **display.scroll("Hello World")** code block.
2. Click on **Basic**. Click and drag a **sleep(1000)** block to the code area and attach it under **display.show(Image.HAPPY)**
3. Click on **Download Hex** to download the code to your computer.
4. Navigate to where your code downloaded to, This will normally be the downloads folder on your computer. Copy the file to the **MICROBIT drive**.

Once the code has copied to the micro:bit you will see **Hello Wold +a happy face** scroll across the LED Matrix (see the simulator below).

you can also change the icons by typing a name of an image all in CAPS after Image. here is a list of supported Images [Supported Images](https://microbit-micropython.readthedocs.io/en/latest/tutorials/images.html)

Completed Code

![Completed code to show Text and images together on a micro:bit using EduBlocks](/LEDMatrix04.png)

### Python 

1. Type ```display.show(Image.HAPPY)``` and press enter. This will display a picture of a happy face.
2. Type ```sleep (1000)```. This will pause your program for 1 second. If this isn't included your program will skip over the happy face.
3. Click on **Flash** to download the code to your micro;bit.

Once the code has copied to the micro:bit you will see **Hello Wold +a happy face** scroll across the LED Matrix (see the simulator below).

you can also change the icons by typing a name of an image all in CAPS after Image. here is a list of supported Images [Supported Images](https://microbit-micropython.readthedocs.io/en/latest/tutorials/images.html#)

Completed Code

``` python
from microbit import *

while True:
    display.scroll("Hello World")
    display.show(Image.HAPPY)
    sleep(1000)
```

## Challenge

Use what you have learned within this blog post to make a custom Name badge.

## Conclusion

That's all for Today! Come back next week to learn how to use the [buttons]().
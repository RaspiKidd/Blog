---
title: "micro:bit Compass"
date: 2021-06-20T20:31:17+01:00
draft: false
---

Welcome to another micro:bit Monday blog post. This week we are going to look at creating a simple compass which shows the bearing from magnetic North in degrees.

The built-in compass sensor is called a magnetometer. This can be used to measure the Earths magnetic field.

Here is how to code it.

<!--more-->

## MakeCode

1. Open [MakeCode](https://makecode.microbit.org/#editor) editor within your favourite browser
2. Click and drag the **forever** block to the left and drop it in the bin
3. Click on **Basic** Click and drag a **show string "Hello!"** block to the coding area and attach it within the **on start** block
4. Click where it says **Hello!** and type **Press button A**
5. Click on **Input** Click and drag an **on button A pressed** to the coding area and drop it
6. Click on **Basic** Click and drag a **show number 0** block to the coding area and attach it within the **on button A pressed** block
7. Click on **Input** Click and drag a **compass heading (°)** block to the coding area and attach it within the **0** of the **show number** block

Your code is now ready to download to your micro:bit and test out

Completed Code

![Completed code within MakeCode](/Compass01.png)

## EduBlocks

1. Open [EduBlocks](http://app.edublocks.org/) within your favourite browser and click on micro:bit
2. Click on **Basic** Click on **from microbit import \*** and drop it within  the coding area
3. Click on **Compass** Click on **compass.calibrate()** and attach it under **from microbit import \***
4. Click on **Display** Click and drag a **display.scroll("Hello World")** and attach it under **compass.calibrate()**
5. Click on **Hello World** and type **Press button A**  
6. Click on **Basic** Click on **while True:** and attach it under **display.scroll("Hello World")**
7. Click on **Basic** Click and drag an **if True:** block to the code area and attach it within the **while True:** block
8. Click on **Button** Click and drag a **button_a.was_pressed** block to the code area and attach it within the **True** of the **if** block
9. Click on **Display** Click and drag a **display.scroll(0)** block to the coding area and attach it within the  **if button_a.was_pressed**
10. Click on the **0** within the  **display.scroll** block and type **str(compass.heading())**

Your code is now complete and ready to download to your micro:bit to test it.

Completed Code

![Completed code within EduBlocks](/Compass02.png)

## Python

1. Open up your favourite Python editor for the micro:bit
2. Type ```from microbit import *``` This imports the micro:bit library to use within python so we can program with the micro:bit
3. Type ```compass.calibrate()``` This tells the micro:bit to calibrate the magnetometer sensor
4. Type ```display.scroll("Press button A")``` This scrolls Press button A across the LED Matrix
5. Type ```while True:``` This create a loop that will go on forever
6. Type ```if button_a.was_pressed()``` This creates a statement to check if button A on the micro:bit was pressed
7. Type ```display.scroll(str(compass.heading()))``` This will scroll the direction the compass is facing in Degrees across the display

Your code is now ready to download to the micro:bit and test out.

Completed Code

```py
from microbit import *

compass.calibrate()

display.scroll("Press button A")

while True:
    if button_a.was_pressed()
    display.scroll(str(compass.heading()))
```

## Conclusion

That's it for this week comeback next week where we discover how to use the pins on the bottom edge of the micro:bit
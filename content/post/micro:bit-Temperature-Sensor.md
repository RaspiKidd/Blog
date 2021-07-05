---
title: "Micro:bit Temperature Sensor"
date: 2021-06-20T21:31:58+01:00
draft: false
---

This week in micro:bit Monday we will be looking at the temperature sensor to detect what the temperature is and display it on the LED matrix.

You can do this indoors tethered to your computer by the USB cable or why not attach a battery pack and take it outdoors and see what the difference in temperature is!

<!--more-->

## MakeCode

1. Open [MakeCode](https://makecode.microbit.org/#) within your favourite browser and open a new project
2. Click and drag the **on start** block to the left of the screen and drop it in the bin
3. Click on **Basic**, click and drag a **show number 0** block to the code area and attach it within the **forever block**
4. Click on **Input**, click and drag a **temperature (°c)** block to the code area and drop it within the **0** of the **show number** block

Now you can download your code and test on an actual micro:bit!

Completed Code

![Completed code within MakeCode](/TempSensing01.png)

## EduBlocks

1. Open [EduBlocks](http://app.edublocks.org/) within your favourite browser and click on **micro:bit**
2. Click on **Basic**, click and drag a **from microbit import `*`** block to the code area and drop it
3. Click on **Basic**, click and drag a **while True:** block to the code area and attach it under **from microbit import `*`**
4. Click on **Display**, click and drag a **display.scroll(0)** block to the code area and attach it within the **while True:** block
5. Click within the **0** of the **display.scroll** block and type **temperature ()**

Your code is now completed and ready to download to your micro:bit

Completed Code

![Completed code in EduBlocks](/TempSensing02.png)

## Python

1. Open your favourite Python editor used to code the micro:bit
2. Type ```from micro:bit import *``` This will import the micro:bit library and allow you to interact with the micro:bit
3. Type ```while True:``` This will create a loop that will keep executing the instructions inside it forever
4. Type ```display.scroll(temperature())``` This will scroll the current temperature across the LED matrix

Your code is now complete and ready to download(flash) to your micro:bit

Completed Code

``` Python
from microbit import *

while True:
    display.scroll(temperature())
```

## Conlusion

That's it for this week come back next Monday to find out how to use the compass on the micro:bit 
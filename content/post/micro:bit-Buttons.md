---
title: "micro:bit Buttons"
date: 2021-06-20T20:20:34+01:00
draft: false
---

Welcome to another micro:bit Monday post. Today we will be looking at what we can do with the buttons on the micro:bit.
<!--more-->

## MakeCode

Here is how to use the buttons within the Microsoft MakeCode editor.

1. Open [MakeCode](https://makecode.microbit.org) within your favourite browser.
2. Click and drag the forever block from the coding area to the left side of the screen and drop it in the bin.
3. Click on **Basic**. Click and drag a **show string "Hello!"** block to the coding area and attach it within the **on start** block.
4. Within the **show string** block click on **"Hello!"** and type **Press button A**.
5. Click on **Basic**. Click and drag a **show leds** block to the coding area and attach it under the **show string "Press button A"** block. 

Create an arrow pointing left like this:

![Left-facing arrow](/Buttons01.png)

6. Click on **Input**. Click and drag an **on button A pressed** block to the coding area and drop it.
7. Click on **Basic**. Click and drag a **show icon block** to the coding area and attach it within the **on button A pressed** block. Change the icon by clicking on the white arrow to a **happy face**.
8. Click on **Basic**. Click and drag a **show string "Hello!"** block to the coding area and attach it under the **show icon** block. Now change the text to read **Press button B**.
9. Click on **Basic**. Click and drag a **show leds** block to the coding area and attach it under **show string "Press button B** block.

Create an arrow pointing right like this:

![Right-facing arrow](/Buttons02.png)

10. Click on **Input**. Click and drag an **on button A pressed** block to the coding area and drop it. Click on the small arrow next to **A** and click on **B**.
11. Click on **Basic**. Click and drag a **show icon block** to the coding area and attach it within the **on button B pressed** block. Change the icon by clicking on the white arrow to a **happy face**.
12. Click on **Basic**. Click and drag a **show string "Hello!"** block to the coding area and attach it under the **show icon** block. Now change the text to read **Press button A + B**.
13. Click on **Basic**. Click and drag a **show leds** block to the coding area and attach it under **show string "Press button A + B** block. 

Create a right and left facing arrow.

![Left and right-facing arrows](/Buttons04.png)

4. Click on **Input**. Click and drag an **on button A pressed** block to the coding area and drop it. Click on the small arrow next to **A** and click on **A+B**.
15. Click on **Basic**. Click and drag a **show icon block** to the coding area and attach it within the **on button A+B pressed** block. Change the icon by clicking on the white arrow to a **happy face**.
16. Click on **Basic**. Click and drag a **show string "Hello!"** block to the coding area and attach it under the **show icon** block. Now change the text to read **You now know how to use the buttons!**.

Your completed code should look like this:

![Completed Code](/Buttons05.png)

## EduBlocks

Here is how to use buttons within EduBlocks.

1. Open [EduBlocks](http://app.edublocks.org/) within your favourite browser and click on micro:bit.
2. Click on **Basic**. Click and drag a **from microbit import *** block to the coding area and drop it.
3. Click on **Display**. Click and drag a **display.scroll("Hello World")** block to the coding area and attach it under the **from microbit import *** block.
4. Click where it says **Hello World** and delete it, now type **Press button A**.
5. Click on **Basic**. Click and drag a **sleep(1000)** block to the coding area and attach it under **display.scroll("Press button A")**.
6. Click on **Display**. Click and drag a **display.show(Image.HAPPY)** block to the coding area and attach it under **sleep(1000)** block. Click on where it says **Image.HAPPY** and delete it, now type **Image.ARROW_W**.
7. Click on **Basic**. Click and drag a **while True:** block to the coding area and attach it under **display.show(Image.ARROW_W)** block.
8. Click on **Basic**. Click and drag an **if True:** block to the coding area and attach it within the **while True:** block.
9. Click on **Buttons**. Click and drag a **button_a.is_pressed()** block to the coding area and attach it within the **True** of the **if True:** block.
10. Click on **Display**. Click and drag a **display.show(Image.HAPPY)** block to the coding area and attach it within **if button_a.is_pressed** block.
11. Click on **Basic**. Click and drag a **sleep(1000)** block to the coding area and attach it under **display.show(Image.HAPPY)**
12. Click on **Display**. Click and drag a **display.scroll ("Hello World")** block to the coding area and attach it under the **sleep(1000)** block.
13. Click where it reads **Hello World** and delete it, now type **Press button B**.
14. Click on **Display**. Click and drag a **display.show(Image.HAPPY)** block to the coding area and attach it under **display.scroll("press button B")**.
15. Click where it says **Image.HAPPY** and delete it, now type **Image.ARROW_E**.
16. Click on **Basic**. Click and drag an **if True:** block to the coding area and attach it under the **if button_a.is_pressed():** block.
17. Click on **Buttons**. Click and drag a **button_a.is_pressed()** block to the coding area and attach it within the **True** of the **if True:** block. Click on the little **arrow** next to **a** and click on **b**.
18. Click on **Display**. Click and drag a **display.show(Image.HAPPY)** block to the coding area and attach it within **if button_b.is_pressed** block.
19. Click on **Basic**. Click and drag a **sleep(1000)** block to the coding area and attach it under **display.show(Image.HAPPY)**
20. Click on **Display**. Click and drag a **display.scroll ("Hello World")** block to the coding area and attach it under the **sleep(1000)** block.
21. Click where it reads **Hello World** and delete it, now type **Well done! you now know how to use buttons!**

Your completed code should look like this:

![Completed EduBlocks Code](/Buttons06.png)

## Python

There are two common ways to program the micro:but using microPython. The first one is to open the web version in your browser [Python](https://python.microbit.org/v/1) or by downloading the Mu editor from [downloading Mu](https://codewith.mu/en/download) (within this post I am using Mu)

1. Open your preferred method for programming Python.
2. Type ```from microbit import *``` this will import the micro:bit library to use with Python and press enter.
3. Type ```display.scroll("Press button A``` this will display **press button A** scrolling accross the LED matrix.
4. Type ```sleep(1000)``` This will pause the program for 1 second.
5. Type ```display.show(Image.ARROW_W)``` this will display a left facing arrow on the LED matrix.
6. Type ```while True:``` this will make the code loop forever.
7. type ```if button_a.is_pressed():``` this will run the next lot of code only if the **A** button on the micro:bit has been pressed.
8. Type ```display.show(Image.HAPPY)``` this will show a happy face on the LED matrix.
9. Type ```sleep(1000)``` this will pause the program for one second.
10. Type ```display.scroll("Press button B")``` this is will scroll **Press button B** accross the LED display.
11. Type ```display.show(Image.ARROW_E)``` this will display a right facing arrow on the LED matrix.
12. Type ```if button_b.is_pressed():``` this will execute the next bit of code if **button B** is pressed.
13. Type ```display.show(Image.HAPPY)``` This will show a happy face on the LED matrix.
14. Type ```sleep(1000)``` this will pause the program for 1 second.
15. Type ```display.scroll("Well done! You can now use buttons!")``` this will scroll accross the LED matrix.
    
Completed code

``` Python
from microbit import *

display.scroll("Press button A")
sleep(1000)
display.show(Image.ARROW_W)
while True:
    if button_a.is_pressed():
        display.show(Image.HAPPY)
        sleep(1000)
        display.scroll("Press button B")
        display.show(Image.ARROW_E)
    if button_b.is_pressed():
        display.show(Image.HAPPY)
        sleep(1000)
        display.scroll("Well done! You can now use buttons!")
```

## Challenge

Now that you know how to use the buttons on your micro:bit why not go back to to last weeks challenge and add more to your name badge so different messages or images display when you press a button.

Come back next week to learn about the radio function of the micro:bit.
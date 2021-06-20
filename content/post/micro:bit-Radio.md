---
title: "micro:bit Radio"
date: 2021-06-20T21:18:42+01:00
draft: true
---

This week in micro:bit Monday we are going to discover how to use the micro:bit radio.

<!--more-->

## MakeCode

1. open [MakeCode](makecode.microbit.org/) within your favourite browser
2. Click and drag the **forever** block to the left to delete it as we will not be using that block
3. Click on **Radio** Click and drag a **radio set group 1** to the code area and attach it within the **on start** block
4. Click on **Input** Click and drag a **on button A pressed** block to the code area
5. Click on **Basic** Click on **...more** click and drag a **clear screen** block to the coding area and attach it within **on button A pressed** block
6. Click on **Radio** Click and drag a **radio send string ""** block to the coding area and attach it under the **clear screen** block within the **on button A pressed** block
7. Click within the blank space of the **radio send string** block and type **Hello**
8. Click on **Radio** Click and drag a **on radio received receivedString** block to the coding area
9. Click on **Basic** Click and drag a **Show String "Hello"** block to the coding area and attach it within the **on radio received receivedString** block.

Your code is now complete and ready to download to a micro:bit.

Completed Code:

![Completed Code within MakeCode](/Radio01.png)

## EduBlocks

1. Open [EduBlocks](app.edublocks.og) within your favourite browser and click on micro:bit
2. Click on **Basic** Click and drag a **from microbit import *** block to the coding area
3. Click on **Radio** Click and drag a **import radio** block to the code area and attach it under the **from microbit import *** block
4. Click on **Radio** click and drag a **radio.on()** block to the coding area and attach it under the **import radio** block
5. Click on **Radio** Click and drag a **radio.config(channel=7)** block to the code area and attach it under **radio.on()**
6. Click on  **Basic** Click and drag a **while True:** block to the code area and attach it under **radio.config(channel=7)** block
7. Click on **Display** Click and drag a **display.clear** block to the coding area and attach it within the **while True** block
8. Click on **Basic** click and drag an **if True:** block to the code area and attach it under **display.clear**
9. Click on **Buttons** Click and drag a **button_a.is_pressed()** block to the coding area and attach it within the **if** block where it says **True**
10. Click on **Radio** click and drag a **radio.send("hello")** block to the coding area and attach it within the **if button_a.is_pressed()** block
11. Click on **Radio** click and drag a **incoming=radio.receive()** block to the code area and attach it under the **if button_a.is_pressed():** block
12. Click on **Radio** Click and drag a **if incoming == "hello":** block to the code area and attach it under the **incoming=radio.received()** block
13. Click on **Display** Click and drag a **display.scroll("Hello World")** block to the coding area and attach it within the **if incoming =="hello"** block
14. Click on **Basic** Click and drag a **sleep(1000)** block to the code area and attach it under the **if incoming == "hello":** block.

Your code is now complete and ready to download.

Completed Code

![Completed EduBlocks Code](/Radio02.png)

## Python

1. Open your favourite micro:bit Python editor
2. Type ```from microbit import *``` this impoorts the micro:bit libaray for us to communicate with the micro:bit
3. Type ```import radio``` this will import the radio libaray for us to communicate with the radio on the micro:bit
4. Type ```radio.on()``` This will turn the radio module on so we can interact with it
5. Type ```radio.config(channel=1)``` this sets the radio channel to 1. It is important to make sure the micro:bits you are using are on the same channel. These can be numbered from 1-255.
6. Type ```while True:``` This will create a loop that will run forever
7. Type ```dispplay.clear()``` this clears the display on the micro:bit
8. Type ```if button_a.is_pressed():``` this executes the next instuction if button a on the micro:bit is pressed
9. Type ```radio.send("hello")``` This sends the message hello to another micro:bit that is listening on the same channel
10. Type ```incoming=radio.receive()``` This sets a variable called incoming to radio.receive
11. Type ```if incoming == "hello":``` This executes the next lot of instructions if the incoming message = hello
12. Type ```display.scroll("Hello World")``` this will scroll Hello World accross the micro:bit display
13. Type ```sleep(1000)``` this will pause the program for 1 second.

Your code is now complete and ready to be flashed to the micro:bit.

### Completed Code

``` Python
from microbit import *
import radio

radio.on()

radio.config(channel=1)

while True:
    display.clear()
    if button_a.is_pressed():
        radio.send("hello")
    incoming=radio.receive()
    if incoming == "hello":
        display.scroll("Hello World")
    sleep(1000)
```

## Challenge

Why not send a message to your partner with your name.

## Conclusion

That's all for this week. Why not come back next week to learn about the micro:bit Pins.
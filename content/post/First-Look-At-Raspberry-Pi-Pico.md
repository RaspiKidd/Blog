---
title: "First Look at Raspberry Pi Pico"
date: 2021-06-20T19:41:14+01:00
draft: false
---

The Pico is a brand new microcontroller from the Raspberry Pi Foundation.  It is based on the RP2040 chip developed by the Raspberry Pi Foundation here within the UK.

<!--more-->

## Specs

* Dual cores Arm cortex M0+ running at 133MHz
* 264kB RAM (Random Access Memory)
* 26 GPIO (Genral Purpose Input Output) pins
    * 2 x I2C (Inter- Integrated Circuit)
    * 2 x SPI (Serial Peripheral Interface)
    * 2 x UART (Universal Asynchronous Receiver/Transmitter)
    * 3 x Analogue
* 2Mb flash storage for your programs and data

![Raspberry Pi Pico](/Pico01.jpg)

## What can it do?

The Raspberry PI Pico can become the brains of your next project whether it be a robot, DIY home automation gadget or an electronic musical instrument like a theremin and much more.

## How to Program the Pico?

The Pico can be programmed using MicroPython, C and C++ from launch. We will look at MicroPython to program the Pico later within this guide.

## Soldering the Pins

To solder the pins onto the Pico you will need:

* Soldering iron
* Solder
* Header Pins
* The Pico board
* Breadboard

Breadboard may sound a little strange, but it helps keep your Pico board and pins steady while you solder them.

<iframe width="560" height="315" src="https://www.youtube.com/embed/-5mHSnBScS4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Installing MicroPython

1. Plug the Pico into your computer while holding down the BOOTSEL button on the front of the board
2. Let go of the BOOTSEL button and you should see the Pico pop-up as a removable drive like you have plugged in a pen drive named RPI-RP2
3. Open up the Pico drive and click on INDEX.HTM. This will open up a web page telling you all about the Pico
4. Scroll down the page and click on the Getting Started with MicroPython tab
5. Click on Download UF2 file button and save it to your RPI-RP2 drive. The Pico will reboot and you are now running MicroPython on your Pico.

<iframe width="560" height="315" src="https://www.youtube.com/embed/dDwv7UvJ1QY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Installing The Thonny Python Editor

1. Plug the Pico into your computer while holding down the BOOTSEL button on the front of the board
2. Let go of the BOOTSEL button and you should see the Pico pop-up as a removable drive like you have plugged in a pen drive named RPI-RP2
3. Open up the Pico drive and click on INDEX.HTM. This will open up a web page telling you all about the Pico
4. Scroll down the page and click on the Getting Started with MicroPython tab
5. Click on Download UF2 file button and save it to your RPI-RP2 drive. The Pico will reboot and you are now running MicroPython on your Pico.

<iframe width="560" height="315" src="https://www.youtube.com/embed/0FirNXYtPOY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Setting up Thonny

1. Click on Thonny to open the editor
2. Make sure your Pico is plugged into your computer
3. Click on Python 3.xx down in the bottom right corner. This is where we can change the version of Python that we are programming in. From the menu that appears click on MicroPython(Raspberry Pi Pico).

We are now ready to program our Pico.

<iframe width="560" height="315" src="https://www.youtube.com/embed/K-BSwf4c7VA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Coding the LED

The Pico has a built-in LED that we can program Let's see how to do this.

Type the following code:

``` Python
import machine

led_onboard = machine.Pin(25, machine.Pin.OUT)
led_onboard.value(1)
```

<iframe width="560" height="315" src="https://www.youtube.com/embed/-K-WwZQKP6E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Wrapping Up

That is us completed the first steps to getting started with the Raspberry Pi Pico.

Follow me on [Twitter](https://twitter.com/RaspiKidd) and [Instagram](https://www.instagram.com/raspikidd/) to see more of my discoveries with the Pico over the coming weeks.

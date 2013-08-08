scratch-pi
==========

Projects for Scratch + Raspberry Pi

Getting Started
===============

To complete all of the enclosed proejcts you will need at least: 
* Raspberry Pi with monitor, keyboard and mouse
* Breadboard
* Jumper cables
* LEDs (at least 10)
* resistors (at least 330 &#8486;, an assortment between 100 and 390 &#8486; is best, or whatever values correspond with your LEDs at 5V and 20mA)
* A 4017 "decade counter" chip
* A 4026 "counter and display decoder" chip
* A single digit 7-segment display
* A ULN2003A "Darlington transistor array" (see note below) 
* A Unipolar stepper motor (see note below)
* An NPN transistor (like the 2n4401)

NOTE: You can get an inexpensive stepper motor and the ULN2003A together, look for the "28BYJ-48" stepper motor and driver board

Projects
========

* blinky-light-left-right - a good project to start with. Use left and right arrow keys on your keyboard to blink the LEDs and make simple sounds.
* blink - A simple, non-interactive blink project which uses a transistor to power the LED, rather than the GPIO pin. The Raspberry Pi's GPIO pins can only provide a small amount of current, but the 5V pin can provide more (although still limited). The transistor in this project allows the GPIO pin to turn the LED on and off, but for the LED's power to be drawn from the 5V pin
* 4017 - Another non-interactive project using LEDs which lights up a series of LEDs in sequence. This project is a lead in to the 4017_arrows project, and is a good way to make sure everything is hooked up correctly
* 4017_arrows - This project builds on the 4017 project by adding two arrows to the scene, when clicked, the arrows change the LED that is illuminated. Note that there is one additional wire used in this project beyond what was set up in the 4017 project
* 4026 - This project is similar to the 4017 project with arrows, but replaces the LEDs with a 7 segment display that counts up and down.
* stepper_motor - This is a non-interactive project that demonstrates how to wire up and move a stepper motor. Note that the diagram shows how to wire up the project using a separate ULN2003A and stepper motor, if you get the 28BYJ-48 motor, wire things up so that the wire colors match.


Credits
=======

None of it could be possible without Cymplecy's Scratch GPIO extension
http://cymplecy.wordpress.com/2013/04/22/scratch-gpio-version-2-introduction-for-beginners/

The stepper motor project is based entirely on Cymplecy's walkthough
http://cymplecy.wordpress.com/2013/04/23/scratch-gpio-version-2-using-stepper-motors/

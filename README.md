scratch-pi
==========

Projects for Scratch + Raspberry Pi

Hardware Needed
===============

To complete all of the enclosed projects you will need at least:
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

In each project folder you will find a starter Scratch project and a solution Scratch project. The docs folder contains the circuit diagram for the relevant circuit. The circuit is also visible in the background of the Scratch stage for each project, but that is often not large enough to be useful.

There is a [student guide](https://docs.google.com/document/d/1HvhqimYz74FFc9-a1SsnBxWn7TzPp8uPVilyk3O5iWs/edit?usp=sharing) and a [teacher guide](https://docs.google.com/document/d/1HLV7XSzdQq8FjuiK82BpgcF5K6oz1XSTyaMG_c4S8dU/edit?usp=sharing) available for these projects. The student guides contain information about the electronic components in each circuit, tips for building it successfully and some pseudo-code to get you started with your Scratch code.

TIP: If you get stuck you can always peek at the solution Scratch project. If that doesn't work then there is probably a bug in your circuit.

* make-it-shine - a good project to start with. Use left and right arrow keys on your keyboard to blink the LEDs and make simple sounds.
* make-it-safer - A simple, non-interactive blink project which uses a transistor to power the LED, rather than the GPIO pin. The Raspberry Pi's GPIO pins can only provide a small amount of current, but the 5V pin can provide more (although still limited). The transistor in this project allows the GPIO pin to turn the LED on and off, but for the LED's power to be drawn from the 5V pin
* make-it-sequence - Another non-interactive project using LEDs which lights up a series of LEDs in sequence. This project is a lead in to the make-it-sequence-2 project, and is a good way to make sure everything is hooked up correctly
* make-it-sequence-2 - This project builds on the make-it-sequence project by adding two arrows to the scene, when clicked, the arrows change the LED that is illuminated. Note that there is one additional wire used in this project beyond what was set up in the make-it-sequence project
* make-it-count - This project is similar to the make-it-sequence-2 project with arrows, but replaces the LEDs with a 7 segment display that counts up and down.
* make-it-spin - This is a non-interactive project that demonstrates how to wire up and move a stepper motor. Note that the diagram shows how to wire up the project using a separate ULN2003A and stepper motor, if you get the 28BYJ-48 motor, wire things up so that the wire colors match.


Credits
=======

This project was created by [Audrey Troutt](https://github.com/atroutt) and [Andrew Ganim](https://github.com/aganim) for a [TechGirlz](http://www.techgirlz.org/) TechShop in September 2013.

None of it could be possible without Cymplecy's Scratch GPIO extension
http://cymplecy.wordpress.com/2013/04/22/scratch-gpio-version-2-introduction-for-beginners/

The stepper motor project is based entirely on Cymplecy's walkthough
http://cymplecy.wordpress.com/2013/04/23/scratch-gpio-version-2-using-stepper-motors/

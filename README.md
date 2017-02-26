#Microcontroller Lab1

This lab is an introduction to Arduino Microcontrollers. In this lab, you will be familiarized with the Arduino platform, and how do develop for it. Arduinos are an open source microcontroller, developed to democratize access to microcontrollers. 

Arduionos are controlled through  __sketches__, which are the arduino code format. A __sketch__ has two parts, `setup()` and `loop()`.  *setup* is code that runs once, on startup, while *loop* runs infinitely, continuously repeating. You can think of `loop()` as a `while(True)` loop.  This is where program logic should go. 

Note on the arduino language from the arduino website:

	The Arduino language is based on C/C++. It links against AVR Libc and allows the use of any of its functions; see its user manual for details. 


To learn about the arduino platform, we will be doing a series of labs.  For today's lab __(Lab1)__, we will be using the following parts:

	Red LED
	Potentiometer
	Several Resistors
	Push Button

### First Component
The first lab component is learning to make an LED blink with the arduino.  To do this, we use the digital I/O of the arduino to set pin 13 high. To accomplish this, we use the method `digitalWrite(PIN, STATE)`.  This method can set the selected PIN to be either `HIGH` (__5v__), or `LOW` (__GND__). Through 

	digitalWrite(13, HIGH) 
we can set pin 13 high, which is 5v on standard arduinos (some arduino variants operate at 3.3 V but we won't be using those for these labs).

### Second Component
The second component is to learn about arduino logic and learning to use *input* as well as *output*. We will be using several methods, primarily `digitalRead(IN_PIN)`.  This method reads the state of a pin as either HIGH, or LOW, similar to the output `digitalWrite()`.  Through 

	state = digitalRead(13);
we set the variable `state` to the value retrieved through `digitalRead(13)`, which is the value of pin 13. 

This will also introduce us to an important concept called __Debouncing__. This will also introduce you to Boolean Logic on an Arduino.

### Third Component

In the third component, we will be using a potentiometer to control the brightness of an LED.  The LED is controlled via PWM, and the analog potentiometer input values are transmitted to our computers using the built in Serial Monitor
			
## Closing thougts
This is the basics of using an arduino. Through this, you can create almost anything by building with these building blocks, Digital I/O, Analog I/O, and the Serial interface.
		

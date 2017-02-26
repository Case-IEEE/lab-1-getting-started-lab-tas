# Component Three

In Component Three we will be expanding our program to include analog inputs, using the `analogRead(PIN)` method.  This method returns an `int` value. We will be reading the value of a Potentiometer.

We will also be using the Serial Monitor built into arduino to transmit the analog value to our computer.  

### Step One

Build the circuit according to the provided diagram.

### Step Two

In order to read an analog pin value, instead of using `digitalRead()`, we will use `analogRead(analogInPin);`.  This returns an int value cooresponding to an 10 bit value.  

We will also be using `analogWrite()` to set the brightness of the LED.  `analogWrite()

# Component Three

In Component Three we will be expanding our program to include analog inputs, using the `analogRead(PIN)` method.  This method returns an `int` value. We will be reading the value of a Potentiometer.

We will also be using the Serial Monitor built into arduino to transmit the analog value to our computer.  

### Step One

Build the circuit according to the provided diagram.

### Step Two

In order to read an analog pin value, instead of using `digitalRead()`, we will use `analogRead(analogInPin);`.  This returns an int value cooresponding to an 10 bit value.  

We will also be using `analogWrite()` to set the brightness of the LED.  `analogWrite()` only can handle 8 bits of data, so we will use the `map()` method to map the 10 bit value to the 8 bit value.  These methods look like:

```
sensorValue = analogRead(analogInPin);
outputValue = map(sensorValue, 0, 1023, 0, 255);
analogWrite(analogOutPin, outputValue);
```

Step two is to add the read/write loop to our Component Three sketch.

### Step Three

Once our arduino can read and write analog values, we want to see the specific values, so we will print those to our computer using `Serial.print("...");`

To use Serial, declare serial in the `setup()` method:
```
Serial.begin(9600);
```
then just use `Serial.print("...");` or `Serial.println("...");` to print with a carriage return.

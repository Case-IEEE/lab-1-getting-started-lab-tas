#Component One

Component One is the easiest Lab you will be doing, but also one of the most critical.  In this lab, you will be uploading a simple sketch onto your arduino, and running it.  

###Step One

The first thing to do is create the circuit.  Circuit can be found in Component One folder.

###Step Two

Now that we are ready to program the arduino, the second step is to write the code. 

In the `setup()` method, initialize your pin from step one as an output. To do this, use the *pinmode* method: `pinMode(13, OUTPUT);`.  This sets pin `13` to be an `output`.

 Now, we have to edit the `loop()` method, including code that turns on pin, a timer, and code that turns off the pin.  These functions are `digitalWrite()` and `delay()`.  *digitalWrite* takes two arguments, an `int` cooresponding to the pin, and either `HIGH` or `LOW`.  *delay* takes one argument, an `int` cooresponding to the length of the delay, in milliseconds. This would look something like `digitalWrite(13, HIGH); delay(1000); `
 
Attached to the repo is a blank sketch that you can use to structure your code.  Alternatively, there is a completed Blink sketch located there.

### Step Three

The third step is to compile the code, and debug as needed.  Find the Check Button, and click it. 

### Step Four

The fourth step is to run the code on the board.  Find the Upload Button, and click it.

If the board does not automatically connect, go to "Tools" > "Port" > "/dev/cu.usbmodem..."

#Component Two

In Component Two we will be learning about logic, and digital input.  To do this we will create an arduino sketch that turns on the LED in the previous sketch when there is a button pushed.  To do this, we need to add a push button to our board.  See wiring diagram for how to set up a push button. Then reuse the wiring from Component One to set up the LED on Pin 13. 

### Step One

Make the Circuit.

### Step Two

This time, we need to initialize a pin as an input.  We still use `pinMode` but this time, we use: `pinMode(5, INPUT);` to set pin 5 as an input.

In order read value from the pin, we use `digitalRead()` which returns the value of the pin. In our example, `buttonState = digitalRead(pushButtonPinNumber);` collects this value. 

For a more complicated version of the Button lab, there is an attached *Debounce* sketch, which includes code to debounce the input.  This lab uses button pushes to toggle the LED from __on__ to __off__ and vice-versa.  

In order to use `buttonState` (an `int`) we have to declare it as a global variable.  To do this we declare `int buttonState = 0;` before our `setup()` method.

If we want to change the behavior of our `loop()` depending on the `buttonState` we can use an *if* statement.  These *if* statements look like any other C based language.  

```
if(buttonState==HIGH){
  //do something
}else{
  //do something else
}
```

### Step Three

Set the if/else statement to toggle the LED on or off.  To do this we can reuse the code from Component One.


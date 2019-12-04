*********************
**Example Projects**
*********************

Example 01: Blinling LED
=========================

**->Introduction**

In this example you are learning how to turn on and off a LED or any other actuator which can be controlled by a digital output such as relay, bulb, motor.


**->Learning Outcomes**

From this example, you'll get an understanding about,

- Pin Mode

- Digital Write

- Delay Functions

**->Components**

- Magic Bit

**->Theory**

A digital output allows you to control a voltage with an electronic device. If the device instructs the output to be high, the output will produce a voltage (generally about 5 or 3.3 volts). If the device instructs the output to be low, it is connected to ground and produces no voltage.Here magicbit is the device and output voltage is either 3.3V for HIGH and 0V for LOW.

**->Methodology**

Magicbit equipped with four onboard leds in magicbit development board, Lets select red LED (which is wired to D27).

.. image:: https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/image4.png?raw=true

**->Coding (Live_mode)**

.. image:: https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/blink_led_new.png?raw=true

**->Explanation**

- **When clicked:** After clicked the when clicked block with the green flag the program starts to run.
- **Forever:** This block is giving instruction to run the whole process forever (until giving stop command).
- **Set digital pin 27:** This block means that set the 27th to High or Low state (Logic state - 1 or Logic state - 0). '27' is the pin number according to the magicbit pin diagram. 
- **Wait :** This block is giving instructions to hold the previous instruction for iving time duration.

Example 02: Reading the state of a push button
===============================================

**->Introduction**

In this example you are learning how read a digital input from something like a button & use it to turn on and off a LED or any other digital device.

**->Learning Outcomes**

 From this example, you'll get an understanding about,

-  Digital Read
-  IF-ELSE conditions
-  Variables

**->Components**

- Magic Bit

**->Theory**

 A digital input allows you to read digital signals. Microcontroller recognizes the signal as 1(HIGH) when the signal is close to 3.3v (or 5v depending on the microcontroller) and recognizes as 0(LOW) when the signal is close to 0v. This reading can be used in the program to do various things. 

**->Methodology**

Magicbit equipped with two onboard push buttons in magicbit development board, Lets select the push button which is wired to D34. Buttons on the board are in pulled up internally (to learn more about pullups/pulldowns follow this link), which means when button is not pressed the status of the button is 1(HIGH), & when the button is pressed the status of the button is 0(LOW).

.. image:: https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/Pushbutton.png?raw=true

**->Coding (Live_mode**

.. image:: https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/Pushbutton_code.png?raw=true

**->Explanation**

- **If else block:** In this block when considering the if state it always obey the instruction as HIGH state of the pin reading (Eg: if digital pin 34 is high, then ...). And 'else' state is obey the LOW state of the pin reading (Eg: else digital pin 34 is low, then ...)

- **read digital pin block:** According to this block it is going to read the digital pin.





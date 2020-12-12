*********************
**Example Projects**
*********************

Example 01: Blinking LED
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

Magicbit equipped with four on-board leds in magicbit development board, Lets select red LED (which is wired to D27).

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

Magicbit equipped with two on-board push buttons in magicbit development board, Lets select the push button which is wired to D34. Buttons on the board are in pulled up internally (to learn more about pullups/pulldowns follow this link), which means when button is not pressed the status of the button is 1(HIGH), & when the button is pressed the status of the button is 0(LOW).

.. image:: https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/Pushbutton.png?raw=true

Also like in previous example we need to select an LED to indicate the change, lets select RED LED which is wired to pin D27.



Then we can use the variable as the condition of the if block, and if the button is pressed, the bulb should turn on, and the button is not pressed the light should turn off.

**->Coding (Live_mode**

.. image:: https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/Pushbutton_code.png?raw=true

**->Explanation**

- **If else block:** In this block when considering the if state it always obey the instruction as HIGH state of the pin reading (Eg: if digital pin 34 is high, then ...). And 'else' state is obey the LOW state of the pin reading (Eg: else digital pin 34 is low, then ...)

- **Read digital pin block:** According to this block it is going to read the digital pin.

Example 03:Working with Analog Write
=====================================

**->Introduction**

In this example you are learning how to turn on and off a LED or any other actuator which can be controlled by a digital output such as relay, bulb, motor.

**->Learning Outcomes**

From this example, you'll get an understanding about,

-  Pulse Width Modulation
-  Analog Write

**->Components**

- Magic Bit

**->Theory**

 To change the brightness of a LED we could change the voltage the LED is supplied with, but in a micro-controller, ability to change the voltage (converting a digital number to an analog voltage) is limited, so a method called PWM (Pulse Width Modulation) is used. What this does is pulsing on and off the pin in a high frequency. The length of the pulses creates the perception of brightness. 

 Duty cycle is a term used to describe the ratio between on and off times.


.. image:: https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/dutyCycle.png?raw=true


**->Methodology**

Lets select green LED (which is wired to D16). We will set various duty cycle values as PWM percentage. Then brightness of green led will change according to the changing value.

**->Code (Live_mode)**

.. image:: https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/pwm_led.png?raw=true

**->Explanation**

- **Set pin:** In here we can set any PWM pin (D16, D27 etc) which is connected to a LED. There are four LEDs on magicbit (D16 D17 D18 D27). In this example green color LED is tested. Output PWM percentage value can be set by user. This percentage value means the Duty Cycle of the PWM signal.

Example 04: Using Serial Protocol
==================================

**->Introduction**

In this example you are learning to use serial communication function.

**->Learning Outcomes**

 From this example, you'll get an understanding about,

-  Serial Protocol usage between Magic Bit & the PC

**->Components**

- Magicbit

**->Theory**

In microcontroller programming, communication between devices is essential. There are hundreds of protocols available, but most common & easy to use is Serial Protocol. Commonly used to communicate information between a microcontroller and a computer.



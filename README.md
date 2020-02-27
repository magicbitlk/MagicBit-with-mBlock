# MagicBit-with-mBlock
## Introduction
### What is mBlock

mBlock is a STEAM programming software tool designed for programming for kids. It is developed based on Scratch 3.0 and Arduino code.  It supports block-based and text-based programming languages.For more information click [here](http://www.mblock.cc/introduction-to-product/)

![alt text](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/images/MagicBit/mBlock.jpg "Logo Title Text 1")

### MagicBit with mBlock

MagicBit is supporting three different ways(C-programming, visual programming and IoT) of programming methods. Among them mBlock opensource software can use for visual programming. We built mBlock V3 compatible extension for magicbit users. Below are the steps for adding that extension for your mBlock IDE.

## Procedure

### Step 01 : Download and Install the mBlock IDE

Click [here](http://www.mblock.cc/mblock-software/) for install mblock 3 IDE for your PC. 

(NOTE : The MagicBit extension has been developed for mBlock 3 and Windows users to date)

![alt text](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/images/MagicBit/mblock3.png "Logo Title Text 1")

For installation supports , click [here](https://www.youtube.com/watch?v=TgtZkCzYPgc)

### Step 02 : Add MagicBit extension

1. After installation, search the word "mBlock" in the task bar and double click on the mblock icon.
2. After opening the mBlock IDE, go  Extensions -> Manage Extensions. There will appear the Manage Extensions window. 
3. In the Manage Extensions window, you can find the MagicBit extension by searching the word "Magicbit" or scrolling down the extensions list.
4. Just click on the "Download" button

![alt text](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/images/MagicBit/adding_extension.png "Logo Title Text 1")

You can check wheather the MagicBit extension has been added successfully by going to the Extensions section of the menu bar.Select the Magicbit extension like given in below.

![alt text](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/images/MagicBit/magicbit.png "Logo Title Text 1")

Now you are successfully added the MagicBit extension for your mBlock.

### Step 03 : Add MagicBit board

1. For add the MagicBit board to mBlock boards menu , click [here](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/setup/MagicBit%20Setup.EXE) and download the MagicBit.EXE file. 

![alt text](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/images/MagicBit/setup.png "Logo Title Text 1")

2. Then go to the downloaded path and run the "MagicBit Setup.EXE" file.
3. Provide a easily accessible location for place the extracted files.

![alt text](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/images/MagicBit/magicbit_setup.png "Logo Title Text 1")

4. Copy the "menu.xml" file among extracted files.

![alt text](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/images/MagicBit/menu.png "Logo Title Text 1")

5. Go to the mblock intalled location (etc- C:\Program Files\mBlock). Double click on "assets" folder. Replace the menu.xml file by copied one.

![alt text](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/images/MagicBit/assets.png "Logo Title Text 1")

6. Re-open mBlock IDE or go to Extensions->clear cache for Restart mBlock.  

7. Now go to the mBlock IDE,Boards section and check whether MagicBit board appears under MagicBlocks category.

![alt text](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/images/MagicBit/board_menu.png "Logo Title Text 1")

### Step 04 : Live Mode Configuration

1. Copy the remaining files in the extracted files( MagicBit_Firmware.ino file and Shapes.h file) in step 3-3. Paste them to your regular Arduino project file under a specific name.
(Both files should be in the same folder)

![alt text](https://github.com/magicbitlk/MagicBit-with-mBlock/blob/master/images/MagicBit/live_mode.png "Logo Title Text 1")

2. Then upload the MagicBit Firmware file to the MagicBit. (Pre-requrement : The Arduino IDE must be installed on your computer)

3. Configuration completed.

# Example projects

## Example Projects

### Example 01: Blinking LED

#### Introduction

In this example you are learning how to turn on and off a LED or any other actuator which can be controlled by a digital output such as relay, bulb, motor.


#### Learning Outcomes

From this example, you'll get an understanding about,

- Pin Mode

- Digital Write

- Delay Functions

#### Components

- Magic Bit

#### Theory

A digital output allows you to control a voltage with an electronic device. If the device instructs the output to be high, the output will produce a voltage (generally about 5 or 3.3 volts). If the device instructs the output to be low, it is connected to ground and produces no voltage.Here magicbit is the device and output voltage is either 3.3V for HIGH and 0V for LOW.

#### Methodology

Magicbit equipped with four on-board leds in magicbit development board, Lets select red LED (which is wired to D27).

![alt text](https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/image4.png "Logo Title Text 1")

#### Coding (Live_mode)

![alt text](https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/blink_led_new.png "Logo Title Text 1")

#### Explanation

- **When clicked:** After clicked the when clicked block with the green flag the program starts to run.
- **Forever:** This block is giving instruction to run the whole process forever (until giving stop command).
- **Set digital pin 27:** This block means that set the 27th to High or Low state (Logic state - 1 or Logic state - 0). '27' is the pin number according to the magicbit pin diagram. 
- **Wait :** This block is giving instructions to hold the previous instruction for iving time duration.

### Example 02: Reading the state of a push button


#### Introduction

In this example you are learning how read a digital input from something like a button & use it to turn on and off a LED or any other digital device.

#### Learning Outcomes

 From this example, you'll get an understanding about,

-  Digital Read
-  IF-ELSE conditions
-  Variables

#### Components

- Magic Bit

#### Theory

 A digital input allows you to read digital signals. Microcontroller recognizes the signal as 1(HIGH) when the signal is close to 3.3v (or 5v depending on the microcontroller) and recognizes as 0(LOW) when the signal is close to 0v. This reading can be used in the program to do various things. 

#### Methodology

Magicbit equipped with two on-board push buttons in magicbit development board, Lets select the push button which is wired to D34. Buttons on the board are in pulled up internally (to learn more about pullups/pulldowns follow this link), which means when button is not pressed the status of the button is 1(HIGH), & when the button is pressed the status of the button is 0(LOW).

![alt text](https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/Pushbutton.png "Logo Title Text 1")

Also like in previous example we need to select an LED to indicate the change, lets select RED LED which is wired to pin D27.

Then we can use the variable as the condition of the if block, and if the button is pressed, the bulb should turn on, and the button is not pressed the light should turn off.

#### Coding (Live_mode)

![alt text](https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/Pushbutton_code.png "Logo Title Text 1")

#### Explanation

- **If else block:** In this block when considering the if state it always obey the instruction as HIGH state of the pin reading (Eg: if digital pin 34 is high, then ...). And 'else' state is obey the LOW state of the pin reading (Eg: else digital pin 34 is low, then ...)

- **Read digital pin block:** According to this block it is going to read the digital pin.

### Example 03:Working with Analog Write


#### Introduction

In this example you are learning how to turn on and off a LED or any other actuator which can be controlled by a digital output such as relay, bulb, motor.

#### Learning Outcomes

From this example, you'll get an understanding about,

-  Pulse Width Modulation
-  Analog Write

#### Components

- Magic Bit

#### Theory

 To change the brightness of a LED we could change the voltage the LED is supplied with, but in a micro-controller, ability to change the voltage (converting a digital number to an analog voltage) is limited, so a method called PWM (Pulse Width Modulation) is used. What this does is pulsing on and off the pin in a high frequency. The length of the pulses creates the perception of brightness. 

 Duty cycle is a term used to describe the ratio between on and off times.


![alt text](https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/dutyCycle.png "Logo Title Text 1")


#### Methodology

Lets select green LED (which is wired to D16). We will set various duty cycle values as PWM percentage. Then brightness of green led will change according to the changing value.

#### Code (Live_mode)

![alt text](https://github.com/HarshaWeerasinghe/MagicBit-with-mBlock/blob/master/Example_Resources/Blinking_LED/pwm_led.png "Logo Title Text 1")

#### Explanation

- **Set pin:** In here we can set any PWM pin (D16, D27 etc) which is connected to a LED. There are four LEDs on magicbit (D16 D17 D18 D27). In this example green color LED is tested. Output PWM percentage value can be set by user. This percentage value means the Duty Cycle of the PWM signal.

### Example 04: Using Serial Protocol


#### Introduction

In this example you are learning to use serial communication function.

#### Learning Outcomes

 From this example, you'll get an understanding about,

-  Serial Protocol usage between Magic Bit & the PC

#### Components

- Magicbit

#### Theory

In microcontroller programming, communication between devices is essential. There are hundreds of protocols available, but most common & easy to use is Serial Protocol. Commonly used to communicate information between a microcontroller and a computer.



 A digital output allows you to control a voltage with an electronic device. If the device instructs the output to be high, the output will produce a voltage (generally about 5 or 3.3 volts). If the device instructs the output to be low, it is connected to ground and produces no voltage.Here magicbit is the device and output voltage is either 3.3V for HIGH and 0V for LOW.
 
 #### Methodology
 
 Magicbit equipped with four onboard leds in magicbit development board, Lets select red LED (which is wired to D27)
 



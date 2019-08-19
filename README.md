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


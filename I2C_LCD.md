#I2C_LCD
---------
##Introduction

I2C_LCD is an easy-to-use display module, It can make display easier. Using it can reduce the difficulty of make, so that makers can focus on the core of the work.<br />
We developed the Arduino library for I2C_LCD, user just need a few lines of the code can achieve complex graphics and text display features. It can replace the serial monitor of Arduino in some place, you can get running informations without a computer.<br />
More than that, we also develop the dedicated picture data convert software (bitmap converter)，now is available to support PC platform of windows, Linux, Mac OS. Through the bitmap convert software you can get your favorite picture displayed on I2C_LCD, without the need for complex programming.<br />
I2C_LCD can provide you with a very convenient way of make. Enjoy yourself！
<br />
<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_WIKI_1.jpg" width=500 />


##Features
* Only 2 Arduino pins are occupied (Use I2C interface).
* Supports standard I2C mode (100Kbit/s) and fast I2C mode (400Kbit/s).
* Compatible with multiple communication logic levels: 2.8~5VDC.
* Arduino library supported, use a line of code to complete the display.
* Integrate 7 sizes of ASCll fonts, 5 graphics functions.
* Provide dedicated picture data convert software (Bitmap Converter).
* Most of the complex operation is processed by I2C_LCD independent controller, saving user controller resources.
* Supports cursor function, can set up 16 cursor flicker frequency.
* Supports 128 level backlight brightness adjustment.
* Support 64 level screen contrast adjustment.
* Support device address modification.
* Supports 127 I2C_LCD work in parallel.
* When debugging code, it can take the place of the serial monitor to monitor the program running state.
* Two abnormal recovery methods are provided: reset and restore the factory settings.
* Compatible with Grove interface and 4Pin-100mil interface (under the Grove socket).
* 4 symmetrical fixed hole design for easy user installation.
* China style unique appearance.


##Platform Support

|Arduino|LinkIt|
|---------|-----|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/arduino_logo.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/linkit_logo.jpg)|


##Product Version

| Version 	| How to buy	|
|-----------|---------------|
|I2C_LCD (With universal Grove cable)|[![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/300px-Get_One_Now_Banner.png)](https://www.seeedstudio.com/I2C_LCD-(With-universal-Grove-cable)-p-2601.html)|
|I2C_LCD (With conversion Grove cable)|[![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/300px-Get_One_Now_Banner.png)](http://www.elecrow.com/i2c-lcd-with-female-jumper-cable.html)|


##Interface Function

<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_Board.jpg" width=700 />


##Specification
|Parameter|Value|
|---------|-------------|
|Screen Type|Dual color LCD|
|Screen Resolution|128*64 Pixels|
|Screen Active Area (L*W)| 47.1*26.5mm|
|Individual Pixel Size|0.33*0.33mm|
|Communication Mode|I2C(100Kbit/s and 400Kbit/s)|
|Controler|STM8S005KBT6|
|Operating Frequency|16 MHz|
|Weight|20g|

##Electrical Characteristics
|Parameter|Min.|Typical|MNax.|Unit|
|---------|------|------|------|------|
|Supply voltage（5V to GND）|4.5|5|5.5|V
|Logic Voltage（SCL/SDA）|2.8|5|5.5|V
|HBM ESD|-|5000|-|V
|Temperature|-20|25|70|℃




##How to use? 
**Step 1:** Install the latest version of Arduino IDE to your computer.
<br />
<img src="https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/arduino_logo.jpg"/>

**Step 2:** Download and install the I2C_LCD Library to Arduino IDE:

Open Arduino IDE, click Sketch -> Include Library -> Add .ZIP Library.

<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_InstalLib_1.jpg"/>

Find and select the I2C_LCD.zip file you just downloaded.

<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_InstalLib_2.jpg"/>

Restart the Arduino IDE.

**Step 3:** Chose the example project which you like. (Take "HelloWorld" project for example here.)<br />
Click File -> Examples -> I2C_LCD -> "HelloWorld".

<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_InstalLib_3.jpg" width=700 />

**Step 4:** Connect I2C_LCD to your Seeeduino Vx board with Grove cable. Then connect Seeeduino Vx board to your computer.

<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_InstalLib_4.jpg" width=700 />

**Step 5:** Select your board and serial port.<br />
Select the board: Click Tools -> Board -> Arduino Duemilanove or Diecimila(Seeeduino V3.0 Or early version), Arduino Uno(Seeeduino Lotus or Seeeduino V4.0).

<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_InstalLib_5.jpg"/>

Select the COM: Click Tools -> Serial Port -> COMX(which connected with your board.)

<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_InstalLib_6.jpg"/>

**Step 6:** Upload the program and enjoy yourself!

<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_InstalLib_7.jpg"/>


**PS:**<br />
1. For more details about library install please refer to http://www.arduino.cc/en/Guide/Libraries.<br />
2. If you encounter other problems during the use, please refer to the User Manual for help. If you can't solve it, please contact us.<br />
<br />
**Technical support:** Joney.s@foxmail.com <br />



##Version Tracker
**I2C_LCD Hardware:**

| Revision 	| Release Note	| Release Date	|
|-----------|---------------|---------------|
|I2C_LCD_v1.2| 1. Add production test point. |Sep 18, 2015|
|I2C_LCD_v1.1| 1. Modify the logo position. <br /> 2. Modify the board shape. <br /> 3. Modify the button position. |May 8, 2014|
|I2C_LCD_v1.0| 1. Modify the power circuit wiring. |Mar 1, 2014|
|I2C_LCD_v0.9b| 1. Initial public release. |Feb 15, 2014|

**I2C_LCD Library:**

| Revision 	| Release Note	| Release Date	|
|-----------|---------------|---------------|
|I2C_LCD_v1.21| 1. Support Linkit boards. |Aug 21, 2016|
|I2C_LCD_v1.20| 1. Reorganize I2C_LCD driver interface, make it easy to transplant to any other boards. |Apr 16, 2016|
|I2C_LCD_v1.12| 1. Modify the bug that can't dispaly bitmap when y coordinate is more than 16.|Sep 4, 2015|
|I2C_LCD_v1.11| 1. Modify the bug that '\t' can't print.|Jun 27, 2015|
|I2C_LCD_v1.10| 1. Add LCD print function. <br /> 2. Edit DeviceAddressConfig example.|Jun 25, 2015|
|I2C_LCD_v1.0| 1. Initial public release. |July 6, 2014|

##Resources

Keeping update the latest version.

The [repository of Arduino library hosted here](https://github.com/SparkingStudio/I2C_LCD_Library), if you have any good idea of the code, you can pull to us.

* [I2C_LCD Library](https://github.com/SparkingStudio/I2C_LCD/raw/master/resources/I2C_LCD_Library.zip)
* [I2C_LCD User Manual EN](https://github.com/SparkingStudio/I2C_LCD/blob/master/resources/I2C_LCD-UserManual_EN.zip)
* [I2C_LCD User Manual CN](https://github.com/SparkingStudio/I2C_LCD/blob/master/resources/I2C_LCD-UserManual_CN.zip)
* [BitmapConverter(ForWindows)](https://github.com/SparkingStudio/I2C_LCD/blob/master/resources/Bitmap Converter.rar)
* [BitmapConverter(ForMacOS)](https://github.com/SparkingStudio/I2C_LCD/blob/master/resources/Bitmap Converter.dmg)
* [BitmapConverter(ForLinux)](https://github.com/SparkingStudio/I2C_LCD/blob/master/resources/Bitmap Converter.tar.gz)
* [I2C_LCD_SourceFile](https://github.com/SparkingStudio/I2C_LCD/blob/master/resources/I2C_LCD12864_SourceFile.zip)
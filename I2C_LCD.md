#I2C_LCD

##Introduction
---

I2C_LCD is an easy-to-use display module, It can make display easier. Using it can reduce the difficulty of make, so that makers can focus on the core of the work.

We developed the Arduino library for I2C_LCD, user just need a few lines of the code can achieve complex graphics and text display features. It can replace the serial monitor of Arduino in some place, you can get running informations without a computer.

More than that, we also develop the dedicated picture data convert software (bitmap converter)，now is available to support PC platform of windows, Linux, Mac OS. Through the bitmap convert software you can get your favorite picture displayed on I2C_LCD, without the need for complex programming.

I2C_LCD can provide you with a very convenient way of make. Enjoy yourself！

<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_WIKI_1.jpg" width=700 />


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

###Platform Support

|Arduino|Wio|BeagleBone|Raspberry Pi|LinkIt|
|---------|-----|-----|------|------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/arduino_logo.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/wio_logo.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/bbg_logo.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Seeed-WiKi/master/docs/images/raspberry_pi_logo.jpg)|![...(line truncated)...

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

**Step 2:** Download and install the I2C_LCD Library to Arduino IDE:

Open Arduino IDE, click Sketch -> Include Library -> Add .ZIP Library.

<br />
<img src="https://raw.githubusercontent.com/SparkingStudio/I2C_LCD/master/images/I2C_LCD_InstalLib_1.jpg" width=700 />


Here we will show you how this Grove - Light Sensor works via a simple demo. First of all, you need to prepare the below stuffs:

| Seeeduino V4 | Grove - Light Sensor | Grove - LED Bar |
|--------------|----------------------|-----------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_1.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_2.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_3.jpg)|
|[Get ONE Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get ONE Now](http://www.seeedstudio.com/Grove-Light-Sensor%28P%29-p-1253.html)|[Get ONE Now](http://www.seeedstudio.com/Grove-LED-Bar-v2.0-p-2474.html)|


| Base Shield | micro USB cable | Grove cable |
|---------------|---------------|-------------|
|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_4.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_5.jpg)|![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/gs_6.jpg)|
|[Get ONE Now](http://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get ONE Now](http://www.seeedstudio.com/Micro-USB-Cable-100cm-p-1476.html)|[Get ONE Now](http://www.seeedstudio.com/Grove-Universal-4-Pin-20cm-Unbuckled-Cable-%285-PCs-Pack%29-p-749.html)|



###Connection 

Thanks to the benefit of Grove series module, you don't need to make soldering or bread board, what you need to do is connect the modules to the right port of Base Shield. For this demo, we have 2 Grove modules. 

* Grove - Light Sensor is an analog output module, we connect it to **A0** at this demo
* Grove - LED Bar is a digital input module with a 2-wire bus, we connect it to **D2**

![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/connect.jpeg)

###Download sketch

There's a sketchbook for Seeeduino Stalker V3.1, which is consist of:

* Example of read raw value of the sensor
* Example of this getting started
* Example of the secret box demo 
* LED Bar library

[![](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/sketch_download.png)](https://github.com/Seeed-Studio/Sketch_Grove_Light_Sensor)

Download the sketch and put it at anywhere, open Arduino IDE, **File > Reference**, and copy the location path to **Sketchbook location**, then click on OK. Reopen Arduino IDE, then the sketchbook is set. 

###Upload the code to Arduino

Open Arduino IDE, **File > Sketchbook > GettingStarted** to open the code for this part. 

Then choose the right Board and COM port, and then click on the Upload button, this process will take seconds. Then let's try to cover the light sensor with your hand, you will find LED Bar reduce its led. 

###Get Raw Data

If you don't need a Grove - LED Bar, there's another example you can try, Open Arduino IDE, **File > Sketchbook > RawData** to open the code, after uploaded the example to Seeeduino V4, click on **Serial > Plotter** to get the changing curve of the sensor. 

![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/raw_data.png)


###Project: Secret Box

Here we will show you a project made with Grove - Light Sensor - Secret Box. First you need a box, a paper box, wooden box, any box is ok. Put something in the box, because we named it secret box, that means we don't want anybody to open it, otherwise there will be an alarm to inform you. 

Here we use LinkIt ONE as the controller, which is an Arduino compatible board and consist of rich function. And you need things below:

* [LinkIt ONE](http://www.seeedstudio.com/LinkIt-ONE-p-2017.html)
* Grove - Light Sensor
* Grove - Base Shield
* A Sim Card

Let's connect Grove - Light Sensor to A0 or Base Shield, and open Arduino IDE, **File > Sketchbook > SecretBox**, what you need to do is upload the example to LinkIt ONE. Then someone open the box, the light will detect it, and send you a SMS. 

Have fun.

![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/secret_box.png)


###Version Tracker
This document applies to the following version of products:

| Version 	| Released Date	| How to buy	|
|-----------|---------------|---------------|
|Grove - Light Sensor 1.0 | Apr28, 2013|[![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/300px-Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Light-Sensor-p-746.html)|
|Grove - Light Sensor(P)| 2014 | [![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/300px-Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Light-Sensor(P)-p-1253.html)|
|Grove - Light Sensor(P) V1.1| Aug, 2016| [![enter image description here](https://raw.githubusercontent.com/SeeedDocument/Grove_Light_Sensor/master/images/300px-Get_One_Now_Banner.png)](http://www.seeedstudio.com/Grove-Light-Sensor(P)-p-1253.html)|

###Resources

* [Sketchbook for Light Sensor](https://github.com/Seeed-Studio/Sketch_Grove_Light_Sensor)
* [Eagle File for Grove - Light Sensor V1.0](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/resources/Grove%20-%20Light%20Sensor.zip)
* [Eagle File for Grove - Light Sensor(P) V1.0](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/resources/Grove%20-%20Light%20Sensor%28P%29.zip)
* [Eagle File for Grove - Light Sensor(P) V1.1](https://github.com/SeeedDocument/Grove_Light_Sensor/raw/master/resources/Grove%20-%20Light%20Sensor%28P%29%20v1.1.zip)
\ No newline at end of file
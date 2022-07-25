
# **Keyestudio EASY plug Control Board V2.0**

**![](KS0240/media/6f76d6d71880c51fd437b15b02182c7c.jpeg)**

## Introduction:

The processor used in keyestudio EASY plug control board V2.0 is ATmega328.

It has 5 single Digital ports labeled D5 to D9 (of which 3 can be used as PWM
outputs), 1 dual-digital interface (D3-D4), 4 analog inputs (A0-A3), a Joystick
interface (D2-A6-A7), a SPI communication, a serial port communication and an
IIC communication interface. Also with a USB connection, a power jack, two ICSP
headers and a reset button. It breaks out the IO ports with RJ11 6P6C plug.

Simply connect it to a computer with a USB cable or power it via a DC jack to
get started.

For convenience of wire connection, we simplify the pins GND and VCC into each
plug, so you only need one RJ11 6P6C connector wire to connect an external
sensor or module, no need to separately connect the VCC and GND.

So don't worry that the wrong wiring will damage the external products.

## Specifications:

| **Microcontroller**             | ATmega328P-AU                                        |
|---------------------------------|------------------------------------------------------|
| **Operating Voltage**           | 5V                                                   |
| **Input Voltage (recommended)** | DC7-12V                                              |
| **Single Digital Ports**        | 5 (D5-D9) (of which 3 provide PWM output)            |
| **PWM Digital Ports**           | D5, D6, D9                                           |
| **Analog Input Pins**           | 4 (A0-A3)                                            |
| **DC Current per I/O Pin**      | 20 mA                                                |
| **Flash Memory**                | 32 KB (ATmega328) of which 0.5 KB used by bootloader |
| **SRAM**                        | 2 KB                                                 |
| **EEPROM**                      | 1 KB                                                 |
| **Clock Speed**                 | 16 MHz                                               |

## Details:

-   PCB Dimensions: 100mm x 65mm x 18mm

-   Weight: 55.5g

![](KS0240/media/917d2fcd4039d68a3f306d3fad6aaa44.jpeg)

## Element and Interfaces:

![](KS0240/media/cacade94eb4487e28607dd45d176e904.jpeg)Here is an explanation of what
every element and interface of the board does:

## Detailed Use with ARDUINO Software as follows:

#### Step1\| Download the Arduino IDE

When you get the board, first you should install the Arduino software and
driver.

We usually use the Windows software Arduino 1.5.6 version. You can download it
from the link below:

[https://www.arduino.cc/en/Main/OldSoftwareReleases\##1.5.x](https://www.arduino.cc/en/Main/OldSoftwareReleases##1.5.x)

Or you can browse the ARDUINO website to download the latest version from this
link, <https://www.arduino.cc>, pop up the following interface.

![](KS0240/media/03bcbac0c292a11cc4969884a260c24e.png)

Then click the **SOFTWARE** on the browse bar, you will have two options ONLINE
TOOLS and DOWNLOADS.

![](KS0240/media/c4beb46eae68ef824353b8cc72a19768.png)

Click **DOWNLOADS**, it will appear the latest software version of ARDUINO 1.8.5
shown as below.

![](KS0240/media/95bb95aac8d2e5b92e8bfb5f6d3c3177.png)

In this software page, on the right side you can see the version of development
software for different operating systems. ARDUINO has a powerful compatibility.
You should download the software that is compatible with the operating system of
your computer.

We will take **WINDOWS system** as an example here. There are also two options
under Windows system, one is installed version, the other is non-installed
version.

For simple installed version, first click **Windows Installer**, you will get
the following page.

![](KS0240/media/87d68bf0f659efd12d5a2421f3b0985b.jpeg)

![](KS0240/media/81ed11f0705f918d1457cb772e41719f.png)

This way you just need to click JUST DOWNLOAD, then click the downloaded file to
install it.

For non-installed version, first click Windows ZIP file, you will also get the
pop-up interface as the above figure.

Click JUST DOWNLOAD, and when the ZIP file is downloaded well to your computer,
you can directly unzip the file and click the icon of ARDUINO software to start
it.

**Installing Arduino (Windows):**

Install Arduino with the exe. Installation package downloaded well.

![](KS0240/media/0410a9a2e63c51fee1d04b59041a2884.jpeg)

Click *“I Agree”* to see the following interface.

![](KS0240/media/7bbc90969d7a44f397e0d63428e87c82.jpeg)

Click *“Next”*. Pop up the interface below.

![](KS0240/media/567d62b3dfce772c3e969c653651f6ad.jpeg)

You can press Browse… to choose an installation path or directly type in the
directory you want. Then click “Install” to initiate installation.

![](KS0240/media/69d2c16b683d24d8c03109c853905f97.jpeg)

Wait for the installing process, if appear the interface of Window Security,
just continue to click Install to finish the installation.

![](KS0240/media/4201c1f8cfe13dad71fac63ae275820c.png)

**Introduction for Arduino IDE Toolbar:**

Double-click the icon of Arduino software downloaded, you will get the interface
shown below.

![](KS0240/media/2fbd15be3868df7eb1654b0981c34f79.png)

(Note: if the Arduino software loads in the wrong language, you can change it in
the preferences dialog. See [the environment
page](http://arduino.cc/en/Guide/Environment##languages) for details.)

![](KS0240/media/c9727104a8861d23c03723bd629509a1.png)

The functions of each button on the Toolbar are listed below:

<http://wiki.keyestudio.com/index.php/File:IDE.png>

![](KS0240/media/29f46713e687c2599b13e9f612d39bc9.png)

| **![](KS0240/media/4e25ec81facd0a9de45e48138cb17bbb.png)**  **Verify/Compile** | Check the code for errors                           |
|-------------------------------------------------------------------------|-----------------------------------------------------|
| **![](KS0240/media/e0a80f9e708873ec352697c610864b37.png)**  **Upload**         | Upload the current Sketch to the Arduino            |
| **![](KS0240/media/f1458edbef80c7786dd4c23a5af3f8e8.png)** **New**             | Create a new blank Sketch                           |
| **![](KS0240/media/1a16bf9f039e242fcceba567b52675d5.png)** **Open**            | Show a list of Sketches                             |
| **![](KS0240/media/258e5f7024d8d3e095499b67c72974ae.png)** **Save**            | Save the current Sketch                             |
| **![](KS0240/media/08794db4162e505053e39fafd259e971.png)** **Serial Monitor**  | Display the serial data being sent from the Arduino |

**Installing the Driver:**

Next, we will introduce the driver installation for the board. The driver
installation may have slight differences in different computer systems. So in
the following let’s move on to the driver installation in the WIN 7 system.

The Arduino folder contains both the Arduino program itself and the drivers that
allow the Arduino to be connected to your computer by a USB cable. Before we
launch the Arduino software, you are going to install the USB drivers.

![](KS0240/media/bd93889abeed8f6b1c70b145de108d7d.png)

Plug one end of your USB cable into the Arduino and the other into a USB socket
on your computer.

When you connect the board to your computer at the first time, right click the
icon of your *“Computer” —\>for “Properties”—\> click the “Device manager”*,
under “Other Devices”, you should see an icon for “Unknown device” with a little
yellow warning triangle next to it.

![](KS0240/media/27f6de2d3f0125ed978586e8b99b2033.png)

Then right-click on the device and select the top menu option (Update Driver
Software...) shown as the figure below.

![](KS0240/media/8ac7d3085c739ec9c9a89151be325dc9.png)

It will then be prompted to either “Search Automatically for updated driver
software” or “Browse my computer for driver software”. Shown as below. In this
page, select “Browse my computer for driver software”.

![](KS0240/media/31fdd7c7d5c23f2aced927993c8314cd.png)

After that, select the option to browse and navigate to the “drivers” folder of
Arduino installation.

![](KS0240/media/4a638bb3e87737db0a4795418dcf9cf3.jpeg)

Click “Next” and you may get a security warning, if so, allow the software to be
installed. Shown as below.

![](KS0240/media/3b743c92f153068c5417126e25e9ef88.png)

Installation completed, click “Close”.

![](KS0240/media/4ed2b0f5f38a5f9dbd667146f96740e3.png)

Up to now, the driver is installed well. Then you can right click *“Computer”
—\>“Properties”—\>“Device manager”*, you should see the device shown below.

![](KS0240/media/42b28476abc3d8b9b8845afb71a3a466.png)

#### 

#### Step2\| Connect the board

Connect the control board to your computer using the USB cable. The power LED
should go on.

![](KS0240/media/a55eadebdf25a1f81adfd9989896e19b.jpeg)

#### Step3\| Select the Arduino Board

Open the Arduino IDE, you’ll need to click the “Tools”, then select the Board
that corresponds to your Arduino.

![](KS0240/media/32f262f2016e7127e35dfca89ec28dab.png)

![](KS0240/media/2c4b7dd5761789848452e5148b850e66.png)

#### 

#### Step4\| Select your serial port

Select the serial device of the Arduino board from the **Tools \| Serial Port
menu**. **Note:** to avoid errors, the COM Port should keep the same as the
Ports shown on Device Manager.

![](KS0240/media/42b28476abc3d8b9b8845afb71a3a466.png)

![](KS0240/media/e1adb00d56f221204d6d81fc1be36b1a.png)

#### 

#### Step5\| Upload the Code

Below is an example code for displaying the Hello World!

Copy and paste the code to the Arduino environment IDE.

**///////////////////////////////////////////////////////////////////////////////////////////////**

int val;

int ledpin=13

void setup()

{

Serial.begin(9600);

pinMode(ledpin,OUTPUT);

}

void loop()

{

val=Serial.read();

if(val=='R')

{

digitalWrite(ledpin,HIGH);

delay(500);

digitalWrite(ledpin,LOW);

delay(500);

Serial.println("Hello World!");

}

}

**///////////////////////////////////////////////////////////////////////////////////////////////**

Then click verify button to check the errors. If compiling successfully, the
message "Done compiling" will appear in the status bar.

![](KS0240/media/44e8356462a29eccef8144f812ca640d.png)

After that, click the “Upload” button to upload the code. Wait a few seconds -
you should see the RX and TX leds on the board flashing. If the upload is
successful, the message "Done uploading" will appear in the status bar.

![](KS0240/media/44e8356462a29eccef8144f812ca640d.png)

#### Step6\|Open the Serial Monitor

After that, click the monitor button to open the serial monitor.

![](KS0240/media/3b5e49114b0ba399112a3c63836b8754.png)

Then set the baud rate as 9600, enter an “R” and click Send, you should see the
RX led on the board blink once, and then D13 led blink once, finally "Hello
World!" is showed on the monitor, and TX led blink once.

![](KS0240/media/ac92cfda71208d789cf0246a7da75c35.png)




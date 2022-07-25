# **Keyestudio KEYBOT Coding Robot Control Board**

![ks0384](KS0350/media/614f04db565c6cf7729ab25090a2f075.jpeg)

## Description:

The Keyestudio KEYBOT Coding Robot Control Board is particularly designed for
car robot control.

This control board has integrated the UNO R3 control board and a motor drive
board into one circuit board, which can directly drive two DC motors.

For the convenience of car design, this control board comes with a Bluetooth
interface (fully compatible with HC-06 Bluetooth module), 2 servo interfaces and
a passive buzzer.

For easy car control, this control board also comes with 2 slide switches and a
reset button. The large slide switch is used for an external power supply
control. While the small switch is used for the serial port communication of
Bluetooth module.

For simple connection, it extends all the digital and analog ports out as
telephone sockets. It also comes with a power interface. The telephone socket
integrates the digital and analog ports together, so you just need a cable to
connect it with sensor modules, pretty simple and convenient.

## Technical Details:

-   Main control chip: ATMEGA328P-AU

-   Motor drive chip: TB6612FNG

-   USB to serial chip: ATMEGA16U2-MU

-   Input voltage: DC 7-12V

-   Motor drive current: 1.2A (ave) / 3.2A (peak)

-   Standby current: 47mA

-   Comes with a passive buzzer: D13 control

-   Motor direction interface: D4 (motor A) and D7 (motor B)

-   Motor speed interface: D5 (motor A) and D6 (motor B)

-   Comes with 2 slide switches: power control switch (large one) and Bluetooth
    serial communication control switch (small one)

-   Comes with a Bluetooth interface: suitable for HC-06 Bluetooth, fixed
    direction, can not be connected if reversed.

-   Comes with 2 servo interfaces: D9 and D10 control respectively

-   Comes with a reset button

-   Comes with a power input interface

-   2 DC motor connection interfaces (labeled MA and MB)

-   It has 8 telephone sockets for external sensors and modules (internal with
    power interface). The control terminals are: D3 and D8, D9 and D10, D11,
    D12, D2 and A0, A1 A2 and A3, A4 and A5, A6 and A7.

## Dimensions:

-   105mm\*64mm\*18mm

![](KS0350/media/d08b6831e6e291631ff7a1b7c2bda069.png)

![KS0350 
(1)](KS0350/media/12c51db8946e090a12a59f7eb2f89ab1.jpeg)

## 

## Element and Interfaces:

Here is an explanation of what every element and interface of the board does:

![KS0350 -pinouts](KS0350/media/4faa50cb060fa90ba32976ad0c8848af.jpeg)

## ![KEYES70102370 schematics](KS0350/media/b0ef51aa0b5bca59f48893f9ba6b051e.png)Schematic Diagram:

## Detailed Test with ARDUINO Software as follows:

#### Step1 \| Download the Arduino environment (IDE)

When you get the board, first you should install the Arduino software and
driver.

We usually use the Windows software Arduino 1.5.6 version. You can download it
from the link below:

[https://www.arduino.cc/en/Main/OldSoftwareReleases\##1.5.x](https://www.arduino.cc/en/Main/OldSoftwareReleases##1.5.x)

Or you can browse the ARDUINO website to download the latest version from this
link, <https://www.arduino.cc>, pop up the following interface.

![](KS0350/media/03bcbac0c292a11cc4969884a260c24e.png)

Then click the **SOFTWARE** on the browse bar, you will have two options ONLINE
TOOLS and DOWNLOADS.

![](KS0350/media/c4beb46eae68ef824353b8cc72a19768.png)

Click **DOWNLOADS**, it will appear the latest software version of ARDUINO 1.8.5
shown as below.

![](KS0350/media/95bb95aac8d2e5b92e8bfb5f6d3c3177.png)

In this software page, on the right side you can see the version of development
software for different operating systems. You should download the software that
is compatible with the operating system of your computer.

We will take **WINDOWS system** as an example here. There are also two options
under Windows system, one is installed version, the other is non-installed
version.

For simple installed version, first click **Windows Installer**, you will get
the following page.

![operating system](KS0350/media/87d68bf0f659efd12d5a2421f3b0985b.jpeg)

![](KS0350/media/81ed11f0705f918d1457cb772e41719f.png)

This way you just need to click JUST DOWNLOAD, then click the downloaded file to
install it.

For non-installed version, first click Windows ZIP file, you will also get the
pop-up interface as the above figure.

Click JUST DOWNLOAD, and when the ZIP file is downloaded well to your computer,
you can directly unzip the file and click the icon of ARDUINO software to
install it.

#### Installing Arduino (Windows):

Install Arduino with the exe. Installation package downloaded well.

![Arduino Setup 1](KS0350/media/0410a9a2e63c51fee1d04b59041a2884.jpeg)

Click *“I Agree”* to see the following interface.

![Arduino Setup 2](KS0350/media/7bbc90969d7a44f397e0d63428e87c82.jpeg)

Click *“Next”*. Pop up the interface below.

![Arduino Setup 3](KS0350/media/567d62b3dfce772c3e969c653651f6ad.jpeg)

You can press Browse… to choose an installation path or directly type in the
directory you want. Then click “Install” to initiate installation.

![Arduino Setup 4](KS0350/media/69d2c16b683d24d8c03109c853905f97.jpeg)

Wait for the installing process, if appear the interface of Window Security,
just continue to click Install to finish the installation.

![Arduino1.5.6- setup 5](KS0350/media/4201c1f8cfe13dad71fac63ae275820c.png)

#### Installing Driver:

The driver installation may have slight differences in different computer
systems. So in the following let’s move on to the driver installation in the WIN
7 system.

The Arduino folder contains both the Arduino program itself and the drivers that
allow the Arduino to be connected to your computer by a USB cable. Before we
launch the Arduino software, you are going to install the USB drivers.

![](KS0350/media/bd93889abeed8f6b1c70b145de108d7d.png)

Plug one end of your USB cable into the keyestudio coding robot control board
and the other into a USB socket on your computer.

When you connect keyestudio coding robot control board to your computer at the
first time, right click the icon of your *“Computer” —\>for “Properties”—\>
click the “Device manager”*, under “Other Devices”, you should see an icon for
“Unknown device” with a little yellow warning triangle next to it.

![](KS0350/media/27f6de2d3f0125ed978586e8b99b2033.png)

Then right-click on the device and select the top menu option (Update Driver
Software...) shown as the figure below.

![](KS0350/media/8ac7d3085c739ec9c9a89151be325dc9.png)

It will then be prompted to either “Search Automatically for updated driver
software” or “Browse my computer for driver software”. Shown as below. In this
page, select “Browse my computer for driver software”.

![](KS0350/media/31fdd7c7d5c23f2aced927993c8314cd.png)

After that, select the option to browse and navigate to the “drivers” folder.

![A}ZM5FU2XKL(5GSSBWT0KGX](KS0350/media/4a638bb3e87737db0a4795418dcf9cf3.jpeg)

Click “Next” and you may get a security warning, if so, allow the software to be
installed. Shown as below.

![](KS0350/media/3b743c92f153068c5417126e25e9ef88.png)

Installation completed, click “Close”.

![](KS0350/media/4ed2b0f5f38a5f9dbd667146f96740e3.png)

![](KS0350/media/42b28476abc3d8b9b8845afb71a3a466.png)Up to now, the driver is
installed well. Then you can right click *“Computer” —\>“Properties”—\>“Device
manager”*, you should see the device shown below.

#### Introduction for Arduino IDE Toolbar:

Double-click the icon of Arduino software downloaded well, you will get the
interface shown below.

![software](KS0350/media/2fbd15be3868df7eb1654b0981c34f79.png)

(Note: if the Arduino software loads in the wrong language, you can change it in
the preferences dialog. See [the environment
page](http://arduino.cc/en/Guide/Environment##languages) for details.)

![](KS0350/media/c9727104a8861d23c03723bd629509a1.png)

The functions of each button on the Toolbar are listed below:
<http://wiki.keyestudio.com/index.php/File:IDE.png>

![IDE](KS0350/media/29f46713e687c2599b13e9f612d39bc9.png)

| **![IDE 1](KS0350/media/4e25ec81facd0a9de45e48138cb17bbb.png)**  **Verify/Compile** | Check the code for errors                           |
|------------------------------------------------------------------------------|-----------------------------------------------------|
| **![IDE 2](KS0350/media/e0a80f9e708873ec352697c610864b37.png)**  **Upload**         | Upload the current Sketch to the Arduino            |
| **![IDE 3](KS0350/media/f1458edbef80c7786dd4c23a5af3f8e8.png)** **New**             | Create a new blank Sketch                           |
| **![IDE 4](KS0350/media/1a16bf9f039e242fcceba567b52675d5.png)** **Open**            | Show a list of Sketches                             |
| **![IDE 5](KS0350/media/258e5f7024d8d3e095499b67c72974ae.png)** **Save**            | Save the current Sketch                             |
| **![IDE 6](KS0350/media/08794db4162e505053e39fafd259e971.png)** **Serial Monitor**  | Display the serial data being sent from the Arduino |

#### Step2\| Drive Two DC Motors

Below is an example code, you can copy and paste it on [Arduino
IDE](http://wiki.keyestudio.com/index.php/Download_Arduino_IDE).

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

const int PWMA = 5; // define the left motor speed control of pin D5

const int PWMB = 6; // define the right motor speed control of pin D6

const int INT_A = 4; // define the left motor control of pin D4

const int INT_B = 7; // define the right motor control of pin D7

void setup()

{

pinMode(PWMA,OUTPUT); // set the pin of motor control as output

pinMode(PWMB,OUTPUT);

pinMode(INT_A,OUTPUT);

pinMode(INT_B,OUTPUT);

}

void loop()

{

digitalWrite(INT_A,HIGH); // the left motor rotates forward

digitalWrite(INT_B,HIGH); // the right motor rotates forward

analogWrite(PWMA,200); // the speed of left motor（PWM=200)

analogWrite(PWMB,200); // the speed of right motor（PWM=200)

delay(2000);

analogWrite(PWMA,0); // the speed of left motor（PWM=0)

analogWrite(PWMB,0); // the speed of right motor（PWM=0)

delay(2000);

digitalWrite(INT_A,LOW); // the left motor rotates backward

digitalWrite(INT_B,LOW); // the right motor rotates backward

analogWrite(PWMA,200); // the speed of left motor（PWM=200)

analogWrite(PWMB,200); // the speed of right motor（PWM=200)

delay(2000);

}

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

#### Step3\| Upload the Code

Open the Arduino IDE, you’ll need to click the “Tools”, then select the Board
that corresponds to your Arduino and the serial port.

![ks0350-图片1](KS0350/media/fa8b9231e2010424e37a67d54d1c1a17.png)

Then click the compile button, if compiling successfully, the message "Done
compiling." will appear in the status bar. Shown below.

![](KS0350/media/8a12bc83218261c825a70f6b0894c39a.png)

![](KS0350/media/580ac1e127ffa994b1ae15f468da271d.png)After that, click the “Upload”
button, if the upload is successful, the message "Done uploading." will appear
in the status bar.

#### Step4\| What You Should See

Done uploading, connect two DC motors to the control board, then supply DC 7-12V
power for the control board. Turn on the large slide switch, you should see the
two motors rotate forward for 2 seconds, stop 2 seconds then backward for 2
seconds, circularly.

**![IMG_0195](KS0350/media/de8fde65e5a322c03fb6908af528714d.jpeg)**


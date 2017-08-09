# Compile and Deploy

## Pre-reqs 

Assuming you are using Windows 10 and have an internet connection...

1) RaspberryPi 2/3 
1) [Windows 10 IoT Core Dashboard](https://developer.microsoft.com/en-us/windows/iot/docs/iotdashboard "Dashboard") installed on SD Card.
    -  Formated SD card, faster the better (16 GB Samsung EVO, class 10 works excellent).
    -  The installation image of Windows 10 IoT Core will be automatically installed through the Dashboard.
1) [Visual Studio IDE 2017 Community Edition](https://www.visualstudio.com/ "Visual Studio 2017")
    - UWP Tools (will be a package option during install)
    - Windows 10 SDK 10.0.15063 (will be installed by default during install)

### Installation

+ Insert your SD card in the Raspberry Pi 3.
+ Connect the wires as shown in the frizting diagram located in the Schematics Folder.
+ When everything is connected, turn on the Raspberry Pi 3, connect to a monitor (HDMI cable) and with an Ethernet Cable to a Router or Access Point to make sure that is connected to the Internet.
+ Follow the steps according to they appear on the screen (First booting will take longer than usually due to the installation of the Windows 10 IoT Core (10+ minutes).
+ Once installation is complete, a screen with the model of the device, IP address, devices connected to the Raspberry Pi 3 and so on will appear.
+ Now, it is necessary to return to the Dashboard and check whether the Raspberry is found within the "My devices" tab or not.
+ If the device is not found after more than 20 minutes, reboot Raspberry Pi 3. 
+ Once the aforementioned is checked, open Visual Studio 2017 and load the project code fro mthis repo-- the code of the Facial Recognition Door (FRD). 
+ Notes for Visual Studio 2017:
    - Click on Debug- ARM- and on the green arrow (Remote Machine) is Local Machine by default, so it is necessary to change it.
    - Within Remote Machine Option, if the Raspberry has not been found by Visual Studio, put the IP address manually otherwise the IP address will have been found automatically. 
    - Do not forget to select Universal(Unencrypted Protocol).
    - Finally, if everything has been well, the main page of the program will have to appear on the monitor and from that very moment you could enjoy and open the door with your face!.

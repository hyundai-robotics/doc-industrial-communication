# Hi6 Robot Controller Function Manual - Industrial Communication

{% hint style="warning" %}
The information provided in this product manual is the property of Hyundai Robotics.

It can neither be reproduced nor redistributed in whole or in part without written consent from Hyundai Robotics, and it cannot be provided to a third party or used for other purposes.



This manual can be changed without prior notice.



**Copyright ⓒ 2020 by Hyundai Robotics**
{% endhint %}
# 1. CIFX PCI Communication

This is Industrial Communication manual using CIFX PCI.
# 1.1 CIFX PCI - Installing Programs

This chapter details how to install programs related to industrial communications.
# 1.1.1 Installing SYCON.net

SYCON.net is a program (Provided by Hilscher.) that can create communication configurations for peripheral component interconnect (PCI) communication cards.

<br>

##### 1. Path for downloading the latest version of SYCON.net

{% hint style="info" %}
\.      Click **[https://hilscher.atlassian.net/](https://hilscher.atlassian.net/wiki/spaces/HILKB/overview?mode=global) -> Software -> SYCON.net**.
{% endhint %}

<br>

![[Figure 1.1.1-1 SYCON.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_1.png>)

<br>

![[Figure 1.1.1-2 SYCON.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_2.png>)

<br>

{% hint style="info" %}
\.      Select and download the current version.
{% endhint %}

<br>

![[Figure 1.1.1-3 SYCON.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_3.png>)

<br>

![[Figure 1.1.1-4 SYCON.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_4.png>)

<br>

{% hint style="info" %}
\.      Run the downloaded SYCON.net Setup.exe file to install the program.
{% endhint %}

<br>

![[Figure 1.1.1-5 SYCON.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_5.png>)

<br>

![[Figure 1.1.1-6 SYCON.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_6.png>)

<br>

{% hint style="info" %}
\.      Run the installed SYCON.net program to check whether the installation was completed normally.
{% endhint %}

<br>

![[Figure 1.1.1-7 SYCON.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_7.png>)

<br>


##### 2. Downloading the program from the Hyundai Robotics website

{% hint style="info" %}
Download “**SYCON.net** from [www.hyundai-robotics.com](http://www.hyundai-robotics.com) -> Industrial Robot pages -> Customer support -> Application software.
{% endhint %}

<br>

{% hint style="info" %}
\.      Unzip -> Run the downloaded SYCON.net Setup.exe file to install the program.
{% endhint %}

<br>

{% hint style="info" %}
\.      The SYCON.net program, available on our website, may be different from the latest version.
{% endhint %}


<br># 1.2 CIFX PCI - Installing and Setting Industrial Communication Cards

 A PCI communication card (from Hilscher) is required for industrial communications. Set the communication cards and connect the connectors based on the required communications.
# 1.2.1 Industrial PCI Communication Card


<br>

##### 1. Install the purchased PCI communication card into the Hi6Com (collaborative robot: Hi6Com Mini) inside the controller.

<br>

##### 2. Set the slot number by rotating the PCI communication card's rotary switch.

<br>

##### 3. Set the slot number within a range from 1 to 3 for each PCI communication card.
  (If multiple PCI communication cards are used, each slot number must be different.)

![[Figure 1.2.1-1 PCI Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_2.png>)

{% hint style="warning" %}
**\[Caution]**: Set a different rotary switch number for each PCI card.
{% endhint %}

# 1.2.2 Connectors

<br>

##### Use the appropriate connectors and cables for industrial communication modes.

![[Figure 1.2.2-1 Industrial Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector/image_2.png>)

{% hint style="info" %}
\.      DeviceNet terminating resistance: 120 ohms

\.      CC-Link terminating resistance: 110 ohms
{% endhint %}# 1.2.3 LED Description

<br>

### PCI LED Description

<br>

![[Figure 1.2.3-1 PCI Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_2.png>)

<br>

![[Figure 1.2.3-3 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_3.png>)

<br>

![[Figure 1.2.3-4 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_4.png>)

<br>

![[Figure 1.2.3-5 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_5.png>)

<br>

![[Figure 1.2.3-6 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_6.png>)

<br>

![[Figure 1.2.3-7 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_7.png>)

<br>

![[Figure 1.2.3-8 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_8.png>)

<br>

![[Figure 1.2.3-9 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_9.png>)

<br>

![[Figure 1.2.3-10 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_10.png>)

<br>

![[Figure 1.2.3-11 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_11.png>)

<br>

![[Figure 1.2.3-12 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_12.png>)

<br>

![[Figure 1.2.3-13 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_13.png>)

<br>

![[Figure 1.2.3-14 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_14.png>)

<br>

![[Figure 1.2.3-15 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_15.png>)

<br>

![[Figure 1.2.3-16 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_16.png>)

<br>

![[Figure 1.2.3-17 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_17.png>)

<br>

![[Figure 1.2.3-18 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_18.png>)

<br>

![[Figure 1.2.3-19 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_19.png>)

<br>

![[Figure 1.2.3-20 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_20.png>)

<br>
# 1.3 CIFX PCI - Setting Industrial Communication

To utilize industrial communications, installing a PCI communication card, then setting up the card using the teach pendant and SYCON.net program, will be necessary. 
# 1.3.1 Setting CIFX PCI Slot

Set the CIFX PCI slot communication method. After the settings are completed, restarting the controller's power to apply the settings will be necessary.

<br>

##### 1. Click the menu to enter the slot setting screen.
**\[System > 2: Control Parameter > 11: Industrial Communication > 1: PCI Slot Setting > 1 Channel]**


<br>

##### 2. By referring to the screens shown below, select the slot, communication mode (master/slave), and protocol.
   * The slot number is the rotary switch number of the PCI communication card.
   * If you do not want to set the communication firmware, click the **\[OK]** button to end the process.

{% hint style="warning" %}
**\[Caution]**: Clicking the **\[Clear]** or **\[Apply]** buttons will initialize the PCI slot information on the tab you are currently viewing. Note that the Config file will be also initialized.  
{% endhint %}

![[Figure 1.3.1-1 PCI Slot Setting]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[Figure 1.3.1-2 PCI Slot Setting (master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[Figure 1.3.1-3 PCI Slot Setting (slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

##### 3. Complete the slot settings. 
Click on the **\[Apply]** button.

![[Figure 1.3.1-4 PCI Slot Setting]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[Caution]**

<1>. When you finish setting up the slot by clicking the **\[Apply]** button, all Config files set in the corresponding slots will be deleted. When required to change the communication during use, back up the current Config settings separately.

<2>. If you click the **\[OK]** button without clicking the **\[Apply]** button first, the set will not be applied.
{% endhint %}

<br>

##### 4. Repeat steps 2 and 3 for each slot to set.

<br>

##### 5. Reboot the Controller for the setting to be applied.
Click the menu under **\[Service > 19: Industrial Communication Monitoring]** to check if the set communication has been applied.

![[Figure 1.3.1-5 Industrial Communication Setting Screen]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[Caution]**: When you set the use of the slot, you must Reboot Controller to apply the settings to the system.
{% endhint %}
# 1.3.2 Setting SYCON.net

If the industrial communications of the Hi6 controller will be be used, communications should be set using the “**SYCON.net**” program. The installation methods are as follows (refer to “[**1.1 Installing SYCON.net**](../../1-cifx-pci-install-program/1-sycon-net.md)” for installation).

<br>

##### 1. The following communication setting methods are for your reference.
Refer to the files inside **\“SYCON.net v1.0500\DVD\_2018-12-1\_1\_0500\Documentation\4. Training Material\EN.”**
   *   reference files

       1\) EtherNetIP Scanner - Configuration and Testing TM 02 EN.pdf

       2\) PROFIBUS DP Master - Configuration and Testing TM 02 EN.pdf

       3\) PROFINET IO Controller - Configuration and Testing TM 02 EN.pdf

<br>

##### 2. Connect the PC, where SYCON.net is installed, to the universal LAN port of the robot controller. (Not PCI LAN Port)
Press the menu under **\[System > 2: Control Parameter > 9: Network]** to check the IP of the universal LAN port, then perform a ping test to determine whether a connection has been established.

![[Figure 1.3.2-1 Network IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_1.png>) 
![[Figure 1.3.2-2 Network IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_2.png>) 

{% hint style="info" %}
\.      The IP address can be changed according to the User settings.
{% endhint %}

<br>

##### 3. Run SYCON.net.

![[Figure 1.3.2-3 SYCON.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_3.png>)

<br>

##### 4. In the device catalog on the right side of the screen, click the item that fits the set communication protocol, then drag and drop it on the bus line at the center. 

![[Figure 1.3.2-4 SYCON.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_4.png>)
![[Figure 1.3.2-5 SYCON.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_5.png>)

<br>

##### 5. Double-click the imported item to set it.

{% hint style="info" %}
\.      “Double click” the CIFX PCI card (figure.)

\.      Settings -> Driver 

\.      Select netX Driver
{% endhint %}

![[Figure 1.3.2-6 SYCON.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_6.png>)

{% hint style="info" %}
\.     Settings -> Driver -> netX Driver -> TCP Connection 

\.     IP Address: Input the universal LAN Port IP Address of the connected controller.
{% endhint %}

![[Figure 1.3.2-7 SYCON.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_7.png>)

{% hint style="info" %}
\.      Select Device Assignment -> Click Scan

\.      Select communication (check the channel protocol), then press the “Apply” and “OK” buttons.
{% endhint %}

{% hint style="warning" %}
**\[Caution]**: The channel protocol and slot number must be checked.
{% endhint %}

{% hint style="warning" %}
**\[Caution]**: If scan does not work, check the status of the Cable connection with the controller and the firmware's settings.
{% endhint %}

![[Figure 1.3.2-8 SYCON.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_8.png>)


{% hint style="info" %}
\.      right-click the CIFX PCI figure -> Download
{% endhint %}

![[Figure 1.3.2-9 SYCON.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_9.png>)# 1.3.2.1 SYCON.NET "help"



<br>

##### When using "SYCON.net", Please refer to the "help" function for any parts that are not explained in this manual.

<br>

![[Figure 1.3.2.1-1 SYCON.net help]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/1-Help-SYCON/image_1.png>) 

<br>

![[Figure 1.3.2.1-2 SYCON.net help]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/1-Help-SYCON/image_2.png>) 

<br># 1.3.3 EtherNet/IP

This chapter describes the characteristics of the EtherNet/IP master (scanner) and slave (adapter) and the methods to set them.

<br>

##### EtherNet/IP Overview

EtherNet/IP is an Ethernet-based, open industrial communications protocol developed by ControlNet International (CI) and the Open DeviceNet Vendors Association (ODVA).

In a factory, various devices, such as sensors, remote IOs, motor drivers, human-machine interfaces (HMIs), programmable logic controllers (PLCs), and robot controllers, can be connected to one EtherNet/IP network regardless of the manufacturer.

![[Figure 1.3.3-1 EtherNet/IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/image_1.png>)

<br>

EtherNet/IP can be classified into following classes according to communication functions.

##### Scanner Class
   * The products of this class correspond to existing fieldbus masters and can send requests for I/O data connections to an EtherNet/IP adapter or EtherNet/IP scanner.

<br>

##### Adapter Class
  * The products of this class correspond to existing fieldbus slaves. They also correspond to the targets of the connection of real-time I/O data requested by an EtherNet/IP scanner.
    
  * Without relying on a scanner, an adapter cannot send/receive real-time I/O data by itself. 

<br>

##### Messaging Class
   * The products of this class can send and receive explicit messages for products of all classes and do not support the sending and receiving of real-time I/O data.
   
   * For example, products of this class may include computer interface cards for program uploads/downloads and network configuration tools.


# 1.3.3.1 Specifications of an EtherNet/IP Scanner

<br>

##### Protocol Characteristics

| **Classification**                  | **Specification**             |
| :---                                | :---                           |
| Maximum connectable slave count     | 64                             |
| Maximum input byte size             | 1200 Bytes (FB Block Max)      |
| Maximum output byte size            | 1200 Bytes (FB Block Max)      |
| Maximum input byte size (1 slave)   | 504 bytes                      |
| Maximum output byte size (1 slave)  | 504 bytes                      |
| IO connection                       | Cyclic                         |
| Minimum IO cycle time               | 1 ms                           |
| Communication speed                 | 10 or 100 Mbit/s               |
| Auto negotiation                    | Supported                      |
| Quick connect                       | Supported                      |
| Topology                            | Tree, Line, Ring               |
| Device Level Ring (DLR)             | Beacon-based "Ring Node"       |
| Additional functions                | DHCP, BOOTP, and ACD-supported |


<br>

##### Network Characteristics

| **Classification**                  | **Specification**       |
| :---                                | :---                     |
| Network slave scan                  | Not supported            |
| Data transport layer                | Ethernet II, IEEE 802.3  |
| Hub                                 | Can be used              |
| Switch                              | Can be used              |# 1.3.3.2 Setting an EtherNet/IP Scanner

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” and “[**1.3.2 Setting SYCON.net**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      When using "SYCON.net", Please refer to  ""[**1.3.2 Help SYCON.NET**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)""
{% endhint %}

<br>

##### 1. Select the EtherNet/IP master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.3.2-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication. 

![[Figure 1.3.3.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the EtherNet/IP scanner PCI device using SYCON.net. 

![[Figure 1.3.3.2-3 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_3.png>)
![[Figure 1.3.3.2-4 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan a PCI device and apply the EtherNet/IP scanner.

![[Figure 1.3.3.2-5 SYCON.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

##### 5. Download the settings.

![[Figure 1.3.3.2-6 EtherNet/IP Scanner Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare an adapter (slave) module that is to be connected to the EtherNet/IP scanner.
   * In this example, the M9289 EtherNet/IP adapter of Crevis will be used. 
   * Activate the module by supplying system power and field power.

![[Figure 1.3.3.2-7 Crevis M9289]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

##### 7. Set the IP address of the adapter (slave) for EtherNet/IP communication connection.

{% hint style="info" %}
\.      Set an IP address by using the DIP switches.
{% endhint %}

![[Figure 1.3.3.2-8 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
\.      How to set an IP address using BootpSvr.exe.
{% endhint %}

<br>

##### 8. (Example of Bootp) Set the IP address of the slave device using Bootp.
   * Change the No. 9 DIP switch to the On state.

![[Figure 1.3.3.2-9 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_9.png>)

   * Connect the PC to the M9289 adapter's LAN port.

![[Figure 1.3.3.2-10 Crevis M9289 LAN Port]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

##### 9. Run BootpSvr.exe on the PC.
   * The program is provided by Crevis (download IO Guide Pro from the website and install it)

![[Figure 1.3.3.2-11 Crevis IO Guide Pro]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_11.png>)

![[Figure 1.3.3.2-12 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
\.      While pressing Start Bootp, disconnect the power of the M9289 module and apply the power again to reboot.
{% endhint %}

![[Figure 1.3.3.2-13 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

##### 10. When the adapter device reboots, the device's information will appear in the BootpSvr.exe program.

![[Figure 1.3.3.2-14 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

##### 11. Select a device and set an IP.

![[Figure 1.3.3.2-15 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_15.png>)![[Figure 1.3.3.2-16 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

##### 12. Change all DIP switches of the adapter, where the IP settings are completed, to the Off state, then reboot the device.

{% hint style="info" %}
\.      The status of the DIP switches and whether the adapter has rebooted must be checked.
{% endhint %}

![[Figure 1.3.3.2-17 Crevis DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

##### 13. Register the electronic data sheet (EDS) files of the slave device.

{% hint style="info" %}
\.      EDS files are required to use a device that is not registered at SYCON.net.

\.     The EDS files of the M9289 adapter can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.3.2-18 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
\.      Register the downloaded EDS files on SYCON.net.

\.     When registering the EDS files, check the industrial communication protocol (EtherNet/IP.)
{% endhint %}

![[Figure 1.3.3.2-19 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_19.png>)![[Figure 1.3.3.2-20 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_20.png>)
![[Figure 1.3.3.2-21 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_21.png>)

![[Figure 1.3.3.2-22 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

##### 14. Perform a network scan.

{% hint style="info" %}
\.      The EtherNet/IP scanner does not support the network scan function.
{% endhint %}

<br>

##### 15. Perform a slave (adapter) device configuration.

{% hint style="info" %}
\.      Import the registered device and place it on the EtherNet/IP master's bus line.
{% endhint %}

![[Figure 1.3.3.2-23 Sycon.net Bus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      Double-click the relevant device (adapter) to proceed to the settings.

\.      Set the input/output byte count appropriately for the IO devices mounted on the relevant device.

\.      In this example, the settings are as follows:
{% endhint %}

<br>

![[Figure 1.3.3.2-24 Adapter Device Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.        O -> T: Originator (Master) -> Target (Slave)

\.        Output : EtherNet/IP Scanner  -> M9289

\.        [Output Module]     
\.         1. M225F (2Bytes)   
\.         **=> 2Bytes**   
{% endhint %}

<br>

![[Figure 1.3.3.2-25 Adapter Device Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.        T -> O: Target (Slave) -> Originator (Master)

\.        Input : M9289 -> EtherNet/IP Scanner

\.        [Input Module]   
\.         1. M7001  (1Byte)   
\.         2. M12DF  (2Bytes)   
\.         **=> 3Bytes**   
{% endhint %}

<br>

##### 16. Perform a master (scanner) device configuration.
    

{% hint style="info" %}
\.        Right-click the master device to disconnect it.
{% endhint %}

![[Figure 1.3.3.2-26 Adapter Device Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Double-click the master device. 

\.        Set the IP address of the master device.
{% endhint %}

![[Figure 1.3.3.2-27 Adapter Device Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.        Set the IP address of the slave device.
{% endhint %}

![[Figure 1.3.3.2-28 Scanner Device Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.        Set the scan time of the slave device.

\.        Set an appropriate communication speed by adjusting the relevant value.
{% endhint %}

![[Figure 1.3.3.2-29 Scanner Device Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.        Check the settings of the slave device in the address table.

\.        Check the input/output IO byte count and the start address.
{% endhint %}

![[Figure 1.3.3.2-30 Scanner Device Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
\.        [Quick Connect]

\.        EtherNet/IP supports the quick connect function.  
{% endhint %}

{% hint style="info" %}
\.        The following conditions should be met to use the quick connect function.

\.        (1) Products that support the master and slave quick connect function are necessary.  
\.        (2) The quick connect function cannot be used when using the auto negotiation function.  
\.        (3) The quick connect function cannot be used when using the auto MDI-X function.  
\.        (4) 100 Mbit/s and full duplex should be made available.  
{% endhint %}

{% hint style="info" %}
\.        When the settings are established, proceed the download.
{% endhint %}

![[Figure 1.3.3.2-31 Scanner Device Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

##### 17. Check the communication status. 

{% hint style="info" %}
\.        The communications status should be checked in SYCON.net and the teach pendant.

\.        Refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.
{% endhint %}

{% hint style="info" %}
\.      Double-clicking the connected master device will allow you to check the communication status.
{% endhint %}

![[Figure 1.3.3.2-32 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_32.png>)

![[Figure 1.3.3.2-33 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
\.        Using the diagnosis function of SYCON.net will allow you to monitor the IO's input and output status along with the communication status.
{% endhint %}

![[Figure 1.3.3.2-34 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_34.png>)

<br>

##### 18. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.3.3 Specifications of an EtherNet/IP Adapter

<br>

##### Protocol Characteristics

| **Classification**           | **Specification**                             |
| :---                         | :---                                           |
| Maximum input byte size      | 240 bytes (TP) / 504 bytes (SYCON.net)         |
| Maximum output byte size     | 240 bytes (TP) / 504 bytes (SYCON.net)         |
| IO connection (implicit)     | 1 exclusive Owner, 1 Listen only, 1 Input Only |
| IO connection                | Cyclic, Application Trigger, Change of State   |
| Minimum IO cycle time        | 1 ms                                           |
| Communication speed          | 10 or 100 Mbit/s                               |
| Auto negotiation             | Supported                                      |
| Quick connect                | Supported                                      |
| Topology                     | Tree, Line, Ring                               |
| DLR V2 (Ring Topology)       | Supported                                      |
| Additional functions         | DHCP, BOOTP, and ACD-supported                 |


<br>

##### Network Characteristics

| **Classification**           | **Specification**        |
| :---                         | :---                      |
| Data transport layer         | Ethernet II, IEEE 802.3   |
| Hub                          | Can be used               |
| Switch                       | Can be used               |# 1.3.3.4 Setting an EtherNet/IP Adapter

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” and proceed with the following methods.

<br>

{% hint style="info" %}
\.      **[EtherNet/IP Adapter EDS File Download]**

\.      Refer to “[**5. Slave Device Description Files**](../../../5-slave-config-file.md)".
{% endhint %}

<br>

##### 1. By using the teach pendant, select an EtherNet/IP slave in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.3.4-1 Firware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication. 

![[Figure 1.3.3.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If the Config file set using SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave PCI Slot Configuration >  EtherNet/IP Slave]**

![[Figure 1.3.3.4-3 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.3.4-4 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of Each Item

{% hint style="info" %}
\.      [IP setting]

\.      Fixed IP: For setting the IP address, subnet mask, and gateway information.

\.      DHCP: For receiving an IP address from the dynamic host configuration protocol (DHCP) server.
{% endhint %}

{% hint style="info" %}
\.      [Action in Bus Error]

\.      Clear: For initializing all inputs to 0 when a communication error occurs.

\.      Hold: For retaining the last valid input values when a communication error occurs.
{% endhint %}

{% hint style="info" %}
\.      (Error Allowed Time)

\.      For outputting a field bus error signal and an alarm if the communication error lasts for a specified allowable time.
{% endhint %}

{% hint style="info" %}
\.      [Input Bytes]

\.      Input Bytes: Master -> For setting the size of the data to be inputted from the master to the slave.

\.      O -> T: Originator (Master) -> Target (Slave)
{% endhint %}

{% hint style="info" %}
\.      [Output Bytes]

\.      Output Bytes: Slave -> For setting the size of the data to be outputted from the slave to the master.

\.      T -> O: Target (Slave) -> Originator (Master)
{% endhint %}

{% hint style="info" %}
\.      [Run/Idle Header]

\.      The CIFX-50 RE EtherNet/IP Adapter applied to the controller uses a 32-bit Run/Idle Header when exchanging IOs with the scanner (default).

\.      Depending on the specifications of the scanner, properly set whether to use the Input and Out 32-bit Run/Idle Header where appropriate.
{% endhint %}

<br>

{% hint style="info" %}
\.        [Quick Connect]

\.        EtherNet/IP supports the quick connect function.

\.        When using the quick connect function is necessary, set the EtherNet/IP adapter using SYCO.net.

\.        (1) Products that support the master and slave quick connect function are needed.  
\.        (2) The quick connect function cannot be used when using the auto negotiation function.  
\.        (3) The quick connect function cannot be used when using auto MDI-X function.  
\.        (4) 100 Mbit/s and full duplex need to be used.  
{% endhint %}

<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.

Refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communications status in the teach pendant.

![[Figure 1.3.3.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_5.png>) 

<br>

##### 6. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.3.5 Actions for an EtherNet/IP Error

This section describes the solutions for major errors that may occur while setting up the EtherNet/IP.

Errors can be identified using the diagnosis function of SYCON.net

<br>

Refer to "[**1.4.1 ERROR Code.**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"

<br>

##### 1. Communication Cable Disconnection Error

{% hint style="info" %}
\.      Check the connection status of the LAN cable.

\.      Check whether the adapter device power is switched on.
{% endhint %}

![[Figure 1.3.3.5-1 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_1.png>) 


<br>

##### 2. IP Address Setting Error

{% hint style="info" %}
\.      Master - Check the IP addresses of the master and slave devices.

\.      An error will occur if the IP address set for the adapter device and the value inputted in SYCON.net are different. 

{% endhint %}

![[Figure 1.3.3.5-2 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_2.png>) 

![[Figure 1.3.3.5-3 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_3.png>) 


# 1.3.4 PROFINET IO

This chapter describes the characteristics of the PROFINET IO master (controller) and slave (device) and the methods to set them.

<br>

##### PROFINET IO Overview

PROFINET IO is an Ethernet-based, open industrial communication protocol developed progressively from PROFIBUS-DP and the industrial Ethernet.

![[Figure 1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>) 

<br>

PROFINET IO follows the provider and consumer model for data exchange and can be divided into the three following classes of products.

##### IO Controller Class
   * The products of this class correspond to existing PROFIBUS-DP class 1 masters and are similar to PLCs inside, which are run by an automation program.

   * The IO controller supplies output data to the IO devices set for itself and consumes input data.

<br>

##### IO Device Class
  * The products of this class correspond to existing PROFIBUS-DP slaves. They are connected to IO controllers, such as PLCs, via PROFINET IO.
    
  * The IO device supplies output data, provides input data to the IO controller, and consumes the output data.

<br>

##### IO Supervisor Class
   * The products of this class correspond to existing PROFIBUS-DP class 2 masters and are similar to programming devices, PCs, HMIs, etc., which are designed for configuring and diagnosing networks. 
# 1.3.4.1 Specifications of the PROFINET IO Controller

<br>

##### Protocol Characteristics

| **Classification**                     | **Specification**        |
| :---                                   | :---                      |
| Maximum connectable slave count        | 128                       |
| Maximum input byte size                | 1200 Bytes (FB Block Max) |
| Maximum output byte size               | 1200 Bytes (FB Block Max) |
| Maximum input byte size (1 slave)      | 1024 bytes                |
| Maximum output byte size (1 slave)     | 1024 bytes                |
| IO connection                          |                           |
| Minimum IO cycle time                  | 1 ms                      |
| Communication speed                    | 100 Mbit/s (Full-Duplex)  |
| Auto negotiation                       | Not supported             |
| Quick connect                          | Not supported             |
| Topology                               | Tree, Line                |
| DCP                                    | Supported                 |



<br>

##### Network Characteristics

| **Clssification**                      | **Specification**        |
| :---                                   | :---                      |
| Network slave scan                     | Supported                 |
| Data transport layer                   | Ethernet II, IEEE 802.3   |
| Hub                                    | Cannot be used            |
| Switch                                 | Limited use is allowed (Priority Tagging and Link Layer Discovery Protocol (LLDP) need to be supported)       |# 1.3.4.2 Setting a PROFINET IO Controller

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” and “[**1.3.2 Setting SYCON.net**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      When using "SYCON.net", Please refer to  ""[**1.3.2 Help SYCON.NET**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)""
{% endhint %}

<br>

##### 1. Select the PROFINET IO master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.4.2-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication. 

![[Figure 1.3.4.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

##### 3. Select a PROFINET IO controller PCI device using SYCON.net. 

![[Figure 1.3.4.2-3 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_3.png>)
![[Figure 1.3.4.2-4 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan a PCI device and apply the PROFINET IO controller.


![[Figure 1.3.4.2-5 SYCON.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

##### 5. Download the settings.

![[Figure 1.3.4.2-6 PROFINET IO Controller Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare a device (slave) module that is to be connected to the PROFINET IO controller.
   * In this example, the M9287 PROFINET IO device of Crevis will be used. 
   * Activate the module by supplying system power and field power.

![[Figure 1.3.4.2-7 Crevis M9287]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
\.      How to set the name of the PROFINET IO device using the DIP switch.

\.      M9287-XX: The number set using the DIP switch

\.      In this example, the name was set as M9287-01 using the No. 1 DIP switch.
{% endhint %}

<br>

##### 7. (Example of using a DIP switch) Set the name of the slave device by using the DIP switch.
   * Change only the No. 1 DIP switch to On mode.


![[Figure 1.3.4.2-8 Crevis M9287 Dip Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      After the DIP switches are set, reboot the device.
{% endhint %}

<br>

##### 8. Register the general station description markup language (GSDML) files of the slave device.

{% hint style="info" %}
\.      GSDML files are necessary to use a device that is not registered to SYCON.net.

\.      The GSDML files of the M9287 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.4.2-9 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      Register the downloaded EDS files on SYCON.net.

\.      When registering the GSDML files, check the industrial communication protocol (PROFINET IO).
{% endhint %}

![[Figure 1.3.4.2-10 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_10.png>)![[Figure 1.3.4.2-11 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_11.png>)
![[Figure 1.3.4.2-12 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_12.png>)

![[Figure 1.3.4.2-13 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_13.png>)


<br>

##### 9. Perform a network scan.

{% hint style="info" %}
\.      The PROFINET IO controller supports the network scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the PROFINET IO master device and then click the network scan menu.
{% endhint %}

![[Figure 1.3.4.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      If there is no registered GSDML file, the slave information will appear when a network scan is performed, but registration will not be possible.
{% endhint %}

![[Figure 1.3.4.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      If the GSDML files are normally registered, slave devices can be added through the network scan function.
{% endhint %}

![[Figure 1.3.4.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_16.png>)

![[Figure 1.3.4.2-17 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_17.png>)

![[Figure 1.3.4.2-18 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

##### 10. Perform a slave (device) configuration.

{% hint style="info" %}
\.      Click the disconnect button of the master device to perform the configuration of the slave device.
{% endhint %}

![[Figure 1.3.4.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 1.3.4.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Add a slot connected to M9287 to set a PROFINET IO slave (device).

\.      Slot 1: M7001  
\.      Slot 2: M12DF  
\.      Slot 3: M225F  
{% endhint %}

![[Figure 1.3.4.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_21.png>)

![[Figure 1.3.4.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

##### 11. Performa a master (controller) device configuration.

{% hint style="info" %}
\.      Double-click the master device.
{% endhint %}

![[Figure 1.3.4.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      Set the IP addresses of the master and slave devices.

\.      Set the IP address of the PROFINET IO slave device in the master.

\.      Ensure that the IP addresses of the master and slave devices do not overlap with each other within the same band.
{% endhint %}

![[Figure 1.3.4.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_24.png>)

![[Figure 1.3.4.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      Check whether the slot information of the slave device is correct in the master device.
{% endhint %}

![[Figure 1.3.4.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address of the slave slot in the address table.
{% endhint %}

![[Figure 1.3.4.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.      Set the IO communication speed of PROFINET IO. 
{% endhint %}

![[Figure 1.3.4.2-28 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.      When the settings are completed, proceed with the download.
{% endhint %}

![[Figure 1.3.4.2-29 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

##### 12. Check the communication status.

{% hint style="info" %}
\.        The communication's status needs to be checked on SYCON.net and the teach pendant.

\.        Refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.
{% endhint %}

{% hint style="info" %}
\.      Double-clicking the connected master device will enable you to check the communication status.
{% endhint %}

![[Figure 1.3.4.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_30.png>)

![[Figure 1.3.4.2-31 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
\.        Using the diagnosis function of SYCON.net will enable you to monitor the IO's input and output status along with the communication status.
{% endhint %}

![[Figure 1.3.4.2-32 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_32.png>)

<br>

##### 13. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.4.3 Specifications of a PROFINET IO Device

<br>

##### Protocol Characteristics

| **Classification**           | **Specification**                     |
| :---                         | :---                                   |
| Maximum input byte size      | 256 bytes (TP) / 1024 Bytes (SYCON.net)|
| Maximum output byte size     | 256 bytes (TP) / 1024 Bytes (SYCON.net)|
| IO connection(implicit)      |                                        |
| IO connection                |                                        |
|  Minimum IO cycle time       | 1 ms                                   |
|  Communication speed         | 100 Mbit/s                             |
| Auto negotiation             | Not supported                          |
| Quick connect                | Not supported                          |
| Topology                     | Tree, Line                             |
| DCP                          | Supported                              |


<br>

##### Network Characteristics

| **Classification**           | **Specification**                  |
| :---                         | :---                                |
| Data transport layer         | Ethernet II, IEEE 802.3             |
| Hub                          | Cannot be used                      |
| Switch                       | Limited use is allowed (Priority Tagging and LLDP need to be supported) |

# 1.3.4.4 Setting a PROFINET IO Device

Perform settings according to the preocedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      **[PROFINET IO Device GSDML File Download]**

\.      Please refer to “[**5. Slave Device Description Files**](../../../5-slave-config-file.md)"
{% endhint %}

<br>

##### 1. By using the teach pendant, select a PROFINET IO slave in the section for setting the industrial commuication firmware and reboot the robot controller.

![[Figure 1.3.4.4-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication. 

![[Figure 1.3.4.4-2 Industrial Communications Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If the Config file set via SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave PCI Slot Configuration > PROFINET IO Slave]**

![[Figure 1.3.4.4-3 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[Figure 1.3.4.4-4 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of Each Item

{% hint style="info" %}
\.      [Station Name]

\.      PROFINET IO identifies a slave via the station name.

\.      Naming Rule
\.       > The names of the devices connected through PROFINET IO should not be duplicated.  
\.       > The name can only have up to 240 characters.  
\.       > For special characters, "." and "-" can be used.  
\.       > For characters, English lowercase and numerical characters can be used.  
\.       > The name should start and end with an English lowercase character or number.

{% endhint %}

{% hint style="info" %}
\.      [Input Bytes]

\.      Input Bytes: For setting the size of the data to be inputted from the master to the slave
{% endhint %}

{% hint style="info" %}
\.      [Output Bytes]

\.      Output Bytes: For setting the size of the data to be outputted from the slave to the master
{% endhint %}

{% hint style="info" %}
\.      When setting slots in the master

\.      Designating slots in a way that matches the individually set byte count is required.

\.      4, 8, 16, 32, and 64 bytes -> Designate the slots to match each byte count  
\.      128, 256 bytes -> Designate multiple 64-byte slots (2, 4)  

\.      The input slots are placed before the output slots.
{% endhint %}

![[Figure 1.3.4.4-5 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_5.png>) 


<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.

Please refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

![[Figure 1.3.4.4-6 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_6.png>) 

<br>

##### 6. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.4.5 Actions for a PROFINET IO Error

<br>

Please refer to "[**1.4.1 ERROR Code.**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"



# 1.3.5 EtherCAT

This chapter describes the characteristics of EtherCAT masters and slaves and the methods to set them.

<br>

##### EtherCAT Overview

EtherCAT is an Ethernet-based Fieldbus system developed by Beckhoff Automation.

The EtherCAT protocol provides functions for very fast IO data updates and accurate synchronization.

<br>

##### EtherCAT Master
   * The product corresponds to the existing Fieldbus master and can make a request for IO data connection to the EtherCAT slaves

<br>

##### EtherCAT Slave
   * The products of this class correspond to the existing Fieldbus slaves and are connected to EtherCAT master devices.
# 1.3.5.1 Specifications of the EtherCAT Master

<br>

##### Protocol Characteristics

| **Classification**                    | **Specification**                                             |
| :---                                  | :---                                                          |
| Maximum connectable slave count       | 200                                                           |
| Maximum input byte size               | 1200 Bytes (FB Block Max)                                     |
| Maximum output byte size              | 1200 Bytes (FB Block Max)                                     |
| Maximum input byte size (1 slave)     | 256 bytes                                                     |
| Maximum output byte size (1 slave)    | 256 bytes                                                     |
| IO connection                         |                                                               |
| Minimum IO cycle time                 | 250 us (1 ms recommended)                                     |
| Communication speed                   | 100 Mbit/s (Full-Duplex)                                      |
| Auto negotiation                      | Not supported                                                 |
| Quick connect                         | Not supported                                                 |
| Topology                              | Line, Ring                                                    |
| Redundance                            | Supported (cannot be applied together with synchronization)   |
| Synchronization                       | Distributed Clocks                                            |

<br>

##### Network Characteristics

| **Classification**            | **Specification**                                         |
| :---                          | :---                                                      |
| Network slave scan            | Supported                                                 |
| Data transport layer          | Ethernet II, IEEE 802.3                                   |
| Hub                           | Cannot be used                                            |
| Switch                        | Limited use is allowed (between the master and slave 1)   |
# 1.3.5.2 Setting the EtherCAT Master

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” and “[**1.3.2 Setting SYCON.net**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      When using "SYCON.net", Please refer to  ""[**1.3.2 Help SYCON.NET**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)""
{% endhint %}

<br>

##### 1. Select the EtherCAT master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.5.2-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication. 

![[Figure 1.3.5.2-2  Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the EtherCAT master PCI device using SYCON.net.

![[Figure 1.3.5.2-3 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_3.png>)
![[Figure 1.3.5.2-4 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan a PCI device and apply the EtherCAT master.

![[Figure 1.3.5.2-5 SYCON.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_5.png>) 

<br>

##### 5. Download the settings.

![[Figure 1.3.5.2-6 EtherCAT Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare a slave module that is to be connected to the EtherCAT master.
   * In this example, the M9386 EtherCAT slave of Crevis will be used. 
   * Activate the module by supplying the system power and field power.

![[Figure 1.3.5.2-7 Crevis M9386]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_7.png>) 

<br>

##### 7. Set the station address of the slave device.

{% hint style="info" %}
\.      The station address of the EtherCAT slave device should be set in the master.
{% endhint %}

<br>

##### 8. Register the extensible markup language (XML) files of the slave device.

{% hint style="info" %}
\.      XML files are necessary to use a device that is not registered on SYCON.net.

\.      The XML files of the M9386 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.5.2-8 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      Register the downloaded XML files on SYCON.net.

\.      When registering XML files, check the industrial communication protocol (EtherCAT).
{% endhint %}

![[Figure 1.3.5.2-9 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_9.png>)

<br>

![[Figure 1.3.5.5-10 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.5.2-11 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_11.png>)

<br>

![[Figure 1.3.5.2-12 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_12.png>)


<br>

##### 9. Perform a network scan.

{% hint style="warning" %}
\.      **For EtherCAT, the applicable cable topology and ports are designated.**

\.      **For smooth communication connection, you must check (“[**1.3.5.5 EtherCAT cable topology.**](../5-EtherCAT/5-EtherCAT-Topology.md)”)**
{% endhint %}

{% hint style="info" %}
\.      The EtherCAT master supports the network scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the EtherCAT master device and then click the network scan menu.
{% endhint %}

![[Figure 1.3.5.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      If there is no registered XML file, the slave information will appear when a network scan is performed, but registration will not be possible.
{% endhint %}

{% hint style="info" %}
\.      If XML files are normally registered, slave devices can be added through the network scan function.
{% endhint %}

![[Figure 1.3.5.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_14.png>)

<br>

##### 10. Perform a slave device configuration.

{% hint style="info" %}
\.      Click the disconnect button of the master device to perform the configuration of the slave device.
{% endhint %}

![[Figure 1.3.5.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 1.3.5.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      Add a slot connected to M9386 to set an EtherCAT slave.

\.      Slot 1 : M7001  
\.      Slot 2 : M12DF  
\.      Slot 3 : M225F  
{% endhint %}

![[Figure 1.3.5.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_17.png>)

![[Figure 1.3.5.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_18.png>)


<br>

##### 11. Perform a master device configuration.

{% hint style="info" %}
\.      Double-click the master device.
{% endhint %}

![[Figure 1.3.5.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      Synchronization : To choose between Freerun and Distributed Clocks (DC)

\.      Redundancy : Whether to use redundancy (cannot be used together with Distributed Clocks)

\.      Bus Cycle Time : Can support at least 250 us (1 ms or above is recommended)
{% endhint %}

<br>

{% hint style="info" %}
\.      The station address of each slave can be set.
{% endhint %}

![[Figure 1.3.5.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address of the slave slot in the address table.
{% endhint %}

![[Figure 1.3.5.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_21.png>)


{% hint style="info" %}
\.      When the settings are completed, proceed with the download.
{% endhint %}

![[Figure 1.3.5.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_22.png>)

<br>

##### 12. Check the communication status.

{% hint style="info" %}
\.        The communication status needs to be checked in SYCON.net and teach pendant.

\.        Please refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.
{% endhint %}

{% hint style="info" %}
\.      Double-clicking the connected master device will enable you to check the communication status.
{% endhint %}

![[Figure 1.3.5.2-23 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_23.png>)

![[Figure 1.3.5.2-24 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.        Using the diagnosis function of SYCON.net will enable you to monitor the IO’s input and output status along with communication status.
{% endhint %}

![[Figure 1.3.5.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_25.png>)

<br>

##### 13. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.5.3 Specifications of an EtherCAT Slave

<br>

##### Protocol Characteristics

| **Classification**            | **Specification**  
| :---                          | :---                          |
| Maximum input byte size       | 256 bytes                     |
| Maximum output byte size      | 256 bytes                     |
| IO connection (implicit)      |                               |
| IO connection                 |                               |
| Minimum IO cycle time         | 250 us (1 ms is recommended)  |
| Communication speed           | 100 Mbit/s                    |
| Auto negotiation              | Not supported                 |
| Quick connect                 | Not supported                 |
| Topology                      | Line, Ring                    |
| Synchronization               | Distributed Clocks            |


<br>

##### Network Characteristics

| **Classification**         | **Specification**                                        |
| :---                       | :---                                                     |
| Data transport layer       | Ethernet II, IEEE 802.3                                  |
| Hub                        | Cannot be used                                           |
| Switch                     | Limited us is allowed (between the master and slave 1)   |
# 1.3.5.4 Setting an EtherCAT Slave

The preparation of the manual is in progress.

<br>

{% hint style="info" %}
\.      **[EtherCAT Slave ESI File Download]**

\.      Please refer to “[**5. Slave Device Description Files**](../../../5-slave-config-file.md)”
{% endhint %}
# 1.3.5.5 Cable Topology of EtherCAT

<br>

For EtherCAT, there are restrictions in cable topology and usable Ethernet ports, which are different from existing industrial communication methods.

##### 1. Ethernet Port

{% hint style="info" %}
\.      When the EtherCAT master needs to be connected to a slave, port 0 should be used.
{% endhint %}

![[Figure 1.3.5.5-1 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
\.      When connecting one slave to the master
{% endhint %}

![[Figure 1.3.5.5-2 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
\.      When connecting two slaves or more to the master

\.      Connect port 1 of a slave to port 0 of the next slave.
{% endhint %}

![[Figure 1.3.5.5-3 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_3.png>) 

<br>

##### 2. Redundancy 

{% hint style="info" %}
\.      When using the redundancy function in the master

\.      The last slave’s port 1 and the master’s port 1 need to be connected to form a ring structure.
{% endhint %}

![[Figure 1.3.5.5-4 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_4.png>) 


<br>

##### 3. Cable Topology Error


Please refer to “[**1.4.1 ERROR Code.**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)” 

<br>

{% hint style="info" %}
\.     When the network scan function does not work

\.      Check the port and cable connected to the master.
{% endhint %}

![[Figure 1.3.5.5-5 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
\.      Topology Error (error with configuration)

\.      Check the topology of cables connected between the master and slaves.
{% endhint %}

![[Figure 1.3.5.5-6 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
\.      Topology Error 2 (configuration is normal, but diagnosis shows an error)

\.      Check the topology of cables connected between the master and slaves.

\.      Check the topology of cables connected between the slaves.
{% endhint %}

![[Figure 1.3.5.5-7 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_7.png>)

![[Figure 1.3.5.5-8 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
\.      Mandatory Slave Missing Error

\.      Check the topology of cables connected between the slaves.
{% endhint %}

![[Figure 1.3.5.5-9 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_9.png>)# 1.3.6 PROFIBUS-DP

This chapter describes the characteristics of PROFIBUS-DP masters and slaves and the methods to set them.

<br>

##### Fieldbus Overview

Fieldbus is an open industry standard for operating devices such as sensors, buttons, motor drivers, and operation interfaces in a factory by connecting them to a PLC using a single cable.

Fieldbus provides intelligent services such as monitoring the status of the entire network or reconfiguring it from a central location.

For example, Fieldbus makes it possible to set detailed information, operation, and modes of sensors and switches, not just their simple on/off operations.

The use of a single cable helps reduce the time and cost of wiring and makes the configuration simple, which is advantageous for maintenance. 

Moreover, unlike other protocols that have characteristics of the non-deterministic response of general communication, Fieldbus guarantees data response speed, satisfying industrial applications where the characteristics of critical time are important.

![[Figure 1.3.6-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/image_1.png>) 

<br>

One master and multiple slaves can be connected to one Fieldbus network.
The master device searches/manages the entire network and exchanges data with slave devices.

In general, a PLC is a master device, and other devices such as sensors, buttons, and controllers can be configured as slave devices.# 1.3.6.1 Specifications of the PROFIBUS-DP Master

<br>

##### Protocol Characteristics

| **Classification**                        | **Specification**         |
| :---                                      | :---                      |
| Maximum connectable slave count           | 125                       |
| Maximum input byte size                   | 1200 Bytes (FB Block Max) |
| Maximum output byte size                  | 1200 Bytes (FB Block Max) |
| Maximum input byte size (1 slave)         | 244 bytes                 |
| Maximum output byte size (1 slave)        | 244 bytes                 |
| IO connection                             |                           |
| Minimum IO cycle time                     |                           |
| Communication speed                       | 9.6–12000 Kbit/s          |
| Auto baud rate detection                  | Not supported             |
| Quick connect                             | None                      |
| Topology                                  |                           |



<br>

##### Network Characteristics

| **Classification**             | **Specification**     |
| :---                           | :---                  |
| Network slave scan             | Supported             |
| Data transport layer           | PROFIBUS FDL          |
| Hub                            | None                  |
| Switch                         | None                  |
# 1.3.6.2 Setting the PROFIBUS-DP Master


Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” and “[**1.3.2 Setting SYCON.net**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      When using "SYCON.net", Please refer to  ""[**1.3.2 Help SYCON.NET**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)""
{% endhint %}

<br>

##### 1. Select the PROFIBUS-DP master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.6.2-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 1.3.6.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the PROFIBUS-DP master PCI device using SYCON.net.

![[Figure 1.3.6.2-3 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[Figure 1.3.6.2-4 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan a PCI device and apply the PROFIBUS-DP master.

![[Figure 1.3.6.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>


##### 5. Download the settings.

![[Figure 1.3.6.2-6 PROFIBUS-DP Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare a slave module that is to be connected to the PROFIBUS-DP master.
   * In this example, the GN-9222 PROFIBUS-DP slave of Crevis will be used. 
   * Activate the module by supplying the system power and field power.

![[Figure 1.3.6.2-7 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_7.png>) 


<br>

##### 7. Set the slave device.

{% hint style="info" %}
\.      Set the node number and termination for the PROFIBUS-DP slave device.
{% endhint %}

![[Figure 1.3.6.2-8 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_8.png>) 


{% hint style="info" %}
\.      Termination: Set the termination with the DIP switches (example: turning the termination to the On state).

\.      Node ID (station number): Set the ID with the DIP switches (example: Node 3).
{% endhint %}

<br>

##### 8. Register the general station description (GSD) files of the slave device.

{% hint style="info" %}
\.      GSD files are necessary to use a device that is not registered on SYCON.net.


\.      The GSD files of the GN-9222 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.6.2-9 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      Register the downloaded GSD files on SYCON.net.

\.      When registering GSD files, check the industrial communication protocol (PROFIBUS-DP).
{% endhint %}

![[Figure 1.3.6.2-10 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.6.5-11 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_11.png>)

![[Figure 1.3.6.5-12 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_12.png>)



<br>

##### 9. Perform a network scan.

{% hint style="warning" %}
\.      **The following items must be checked when performing a network scan.**

\.      **(1) Whether the cable is connected**  
\.      **(2) Whether the terminating DIP switches are used**  
{% endhint %}

{% hint style="info" %}
\.      The PROFIBUS-DP master supports the network scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the PROFIBUS-DP master device and then click the network scan menu.
{% endhint %}

![[Figure 1.3.6.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      If there is no registered GSD file, the slave information will appear when a network scan is performed, but registration will not be possible.
{% endhint %}

{% hint style="info" %}
\.      If GSD files are normally registered, slave devices can be added through the network scan function.
{% endhint %}

![[Figure 1.3.6.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

##### 10. Perform a slave device configuration.

{% hint style="info" %}
\.      Click the disconnect button of the master device to perform the configuration of the slave device.
{% endhint %}

![[Figure 1.3.6.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 1.3.6.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      Check the settings of the PROFIBUS-DP slave.

\.      Slot 1: GN-9222  
\.      Slot 2: GT-12DF (Input 2 bytes)  
\.      Slot 3: GT-227F (Output 2 bytes)  
\.      Slot 4: GT-3154 (Input 8 bytes)  
\.      Slot 5: GT-4254 (Output 8 bytes)  
{% endhint %}

![[Figure 1.3.6.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_17.png>)

<br>

![[Figure 1.3.6.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_18.png>)


<br>

##### 11. Perform a master device configuration.

{% hint style="info" %}
\.      Double-click the master device.
{% endhint %}

![[Figure 1.3.6.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_19.png>)


{% hint style="info" %}
\.      Set the communication speed of PROFIBUS-DP.

\.      9.6–12000 Kbit/s 
{% endhint %}

![[Figure 1.3.6.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.     Check the slot information of the slave device in the master.
{% endhint %}

![[Figure 1.3.6.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address of the slave slot in the address table.
{% endhint %}

![[Figure 1.3.6.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
\.      Check in the station table whether each device is in an activated state.
{% endhint %}

![[Figure 1.3.6.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      When the settings are completed, proceed with the download.
{% endhint %}

![[Figure 1.3.6.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

##### 12. Check the communication status.

{% hint style="info" %}
\.        The communication status needs to be checked in SYCON.net and teach pendant.

\.        Please refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.
{% endhint %}

{% hint style="info" %}
\.      Double-clicking the connected master device will enable you to check the communication status.
{% endhint %}

![[Figure 1.3.6.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[Figure 1.3.6.2-26 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Using the diagnosis function of SYCON.net will enable you to monitor the IO’s input and output status along with communication status.
{% endhint %}

![[Figure 1.3.6.2-27 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_27.png>)

<br>

##### 13. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.6.3 Specifications of a PROFIBUS-DP Slave

<br>

##### Protocol Characteristics

| **Classification**        | **Specification**     |
| :---                      | :---                  |
| Maximum input byte size   | 244 bytes             |
| Maximum output byte size  | 244 bytes             |
| IO connection (implicit)  |                       |
| IO connection             |                       |
| Minimum IO cycle time     |                       |
| Communication speed       | 9.6–12000 Kbit/s      |
| Auto baud rate detection  | Supported             |
| Quick connect             | None                  |
| Topology                  |                       |


<br>

##### Network Characteristics

| **Classification**             | **Specification**    |
| :---                           | :---                 |
| Data transport layer           | PROFIBUS FDL         |
| Hub                            | None                 |
| Switch                         | None                 |# 1.3.6.4 Setting a PROFIBUS-DP Slave

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      **[PROFIBUS-DP Slave GSD File Download]**

\.      Please refer to “[**5. Slave Device Description Files**](../../../5-slave-config-file.md).”
{% endhint %}

<br>

##### 1. By using the teach pendant, select the PROFIBUS-DP slave in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.6.4-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 1.3.6.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**:  If the Config file set using SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave PCI Slot Configuration >  PROFIBUS-DP Slave]**

![[Figure 1.3.6.4-3 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.6.4-4 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of Each Item

{% hint style="info" %}
\.      [Station Address]

\.      PROFIBUS-DP identifies a slave via the station address.
{% endhint %}

{% hint style="info" %}
\.      [Input Bytes]

\.      Input Bytes: To set the size of data to be inputted from the master to the slave
{% endhint %}

{% hint style="info" %}
\.      [Output Bytes]

\.      Output Bytes: To set the size of data to be outputted from the slave to the master
{% endhint %}

{% hint style="info" %}
\.      When setting the modules in the master

\.      Required to designate the modules in a way to match the individually set byte count

\.      Order: Input (64–1) -> Output (64–1)

\.      EX) Input 109 bytes: 64 bytes + 32 bytes + 8 bytes + 4 bytes + 1 byte

\.      EX) Output 120 bytes: 64 bytes + 32 bytes + 16 bytes + 8 bytes

\.      EX) Output 200 bytes: 64 bytes + 64 bytes + 64 bytes + 8 bytes

\.      EX) Input 12 bytes: 8 bytes + 4 bytes

\.      Input modules are placed before the output modules.
{% endhint %}

![[Figure 1.3.6.4-5 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>) 


<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.


Please refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

![[Figure 1.3.6.4-6 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>) 

<br>

##### 6. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.6.5 Actions for a PROFIBUS-DP Error

<br>

Please refer to “[**1.4.1 ERROR Code.**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md).”
# 1.3.7 DeviceNet

This chapter describes the characteristics of DeviceNet masters and slaves and the methods to set them.

<br>

##### Fieldbus Overview

Fieldbus is an open industry standard for operating devices such as sensors, buttons, motor drivers, and operation interfaces in a factory by connecting them to a PLC using a single cable.

Fieldbus provides intelligent services such as monitoring the status of the entire network or reconfiguring it from a central location.

For example, Fieldbus makes it possible to set detailed information, operation, and modes of sensors and switches, not just their simple on/off operations.

The use of a single cable helps reduce the time and cost of wiring and makes the configuration simple, which is advantageous for maintenance. 

Moreover, unlike other protocols that have characteristics of the non-deterministic response of general communication, Fieldbus guarantees data response speed, satisfying industrial applications where the characteristics of critical time are important.

![[Figure 1.3.7-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/image_1.png>) 

<br>

One master and multiple slaves can be connected to one Fieldbus network.
The master device searches/manages the entire network and exchanges data with slave devices.

In general, a PLC is a master device, and other devices such as sensors, buttons, and controllers can be configured as slave devices.# 1.3.7.1 Specifications of the DeviceNet Master

<br>

##### Protocol Characteristics

| **Classification**                    | **Specification**                         |
| :---                                  | :---                                      |
| Maximum connectable slave count       | 63                                        |
| Maximum input byte size               | 1200 Bytes (FB Block Max)                 |
| Maximum output byte size              | 1200 Bytes (FB Block Max)                 |
| Maximum input byte size (1 slave)     | 255 bytes                                 |
| Maximum output byte size (1 slave)    | 255 bytes                                 |
| IO connection                         | Bit Strobe, Change of State, Cyclic, Poll |
| Minimum IO cycle time                 |                                           |
| Communication speed                   | 125–500 Kbit/s                            |
| Auto baud rate detection              | Not supported                             |
| Quick connect                         | Supported                                 |
| Topology                              |                                           |



<br>

##### Network Characteristics

| **Classification**             | **Specification**    |
| :---                           | :---                 |
| Network slave scan             | Supported            |
| Data transport layer           | CAN frames           |
| Hub                            | None                 |
| Switch                         | None                 |
# 1.3.7.2 Setting the DeviceNet Master

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” and “[**1.3.2 Setting SYCON.net**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      When using "SYCON.net", Please refer to  ""[**1.3.2 Help SYCON.NET**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)""
{% endhint %}

<br>

{% hint style="info" %}
\.      Refer to the following for the connection of the DeviceNet connector.

\.      (“[**1.2.2 Connectors**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)”)
{% endhint %}

<br>

##### 1. Select the DeviceNet master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.7.2-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 1.3.7.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the DeviceNet master PCI device using SYCON.net.

![[Figure 1.3.7.2-3 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_3.png>)
![[Figure 1.3.7.2-4 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan a PCI device and apply the DeviceNet master.

![[Figure 1.3.7.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_5.png>) 

<br>

##### 5. Set the communication speed.

{% hint style="warning" %}
\.      If the communication speeds of the master and slaves are different, the network scan will not be performed normally.
{% endhint %}

![[Figure 1.3.7.2-6 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_6.png>) 

<br>

##### 6. Download the settings.

![[Figure 1.3.7.2-7 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_7.png>) 

<br>

##### 7. Prepare a slave module that is to be connected to the DeviceNet master.
   * In this example, the NA-9211 DeviceNet slave of Crevis will be used. 
   * Activate the module by supplying the system power and field power.

![[Figure 1.3.7.2-8 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_8.png>) 

<br>

##### 8. Set the slave device.

{% hint style="info" %}
\.      Set the node number and terminating resistance for the DeviceNet slave device.
{% endhint %}

![[Figure 1.3.7.2-9 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_9.png>) 

![[Figure 1.3.7.2-10 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_10.png>)

{% hint style="info" %}
\.      [Example of setting]

\.      Terminating resistance: Install terminating resistance at the cable for use (the terminating DIP switches in the Off state).

\.      MAC ID (station number): Set it to 4 (only DIP switch 3 in the On state).

\.      Baud Rate: Set it to the Auto state (DIP switches 7 and 8 in the On state).
{% endhint %}

<br>

##### 9. Register the EDS files of the slave device.

{% hint style="info" %}
\.      EDS files are necessary to use a device that is not registered on SYCON.net.

\.      The EDS files of the NA-9211 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.7.2-11 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_11.png>)

{% hint style="info" %}
\.      Register the downloaded EDS files on SYCON.net.

\.      When registering EDS files, check the industrial communication protocol (DeviceNet).
{% endhint %}

![[Figure 1.3.7.2-12 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_12.png>)

<br>

![[Figure 1.3.7.2-13 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_13.png>)



<br>

##### 10. Perform a network scan.

{% hint style="warning" %}
\.      **The following items must be checked when performing a network scan.**

\.      **(1) Whether the cable is connected**  
\.      **(2) Whether the terminating resistance is connected or the terminating DIP switches are used**  
\.      **(3) Whether the communication speed between the master and slave is set**  

\.      **Must check with (“[**1.3.7.5 Actions for an DeviceNet error**](../7-DeviceNet/5-Error-DeviceNet.md)”) for smooth communication connection**
{% endhint %}

{% hint style="info" %}
\.      The DeviceNet master supports the network scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the DeviceNet master device and then click the network scan menu.
{% endhint %}

![[Figure 1.3.7.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      If there is no registered EDS file, the slave information will appear when a network scan is performed, but registration will not be possible.
{% endhint %}

{% hint style="info" %}
\.      If EDS files are normally registered, slave devices can be added through the network scan function.
{% endhint %}

![[Figure 1.3.7.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_15.png>)

![[Figure 1.3.7.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_16.png>)

<br>

##### 11. Perform a slave device configuration.

{% hint style="info" %}
\.      Click the disconnect button of the master device to perform the configuration of the slave device.
{% endhint %}

![[Figure 1.3.7.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 1.3.7.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_18.png>)


<br>

{% hint style="info" %}
\.      Set the slave device's Connection Type.

\.      Select the message transmission method fot DeviceNet communication connection.

\.      ** If UCMM is not checked, it is set to Default (GROUP 2) **   

\.      UCMM GROUP 1 : IO Message   
\.      UCMM GROUP 2 : When Resetting the Network, Master - Slave Connection Message (Default)   
\.      UCMM GROUP 3 : Explicit Message   

\.      For certain devices, UCMM GROUP 3 can be used, so Please Check the product specifications before proceeding.
{% endhint %}

![[그림 3.7.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_19.png>)

<br>

{% hint style="info" %}
\.      When using Crevis NA-9211, Proceed after UCMM is not checked. (Group2 Default)
{% endhint %}

![[그림 3.7.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_20.png>)

<br>


{% hint style="info" %}
\.      Check the settings of the DeviceNet slave.

\.      Output: ST-2318 (1 byte)  
\.      Input: ST-1218 (1 byte)  
{% endhint %}

<br>

{% hint style="info" %}
\.      Settings required depending on Connection method (Poll, Change of State, Cyclic, Bit-Strobe)  
{% endhint %}

<br>

![[Figure 1.3.7.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_21.png>)

<br>

{% hint style="info" %}
\.      [Production Inhibit Time]

\.      Set the new IO data production cycle (ms) of the slave device.  
\.      ex) 10ms  :  Update IO every 10ms  
\.      ex) 0ms   :  Update IO as fast as possible  

\.      Shorter update cycles can place greater load on slave device
{% endhint %}

<br>

{% hint style="info" %}
\.      [Expected Packet Rate]

\.      IO Data update time between master and slave device.  
{% endhint %}

<br>

![[Figure 1.3.7.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_22.png>)



<br>

##### 12. Perform a master device configuration.

{% hint style="info" %}
\.      Double-click the master device.
{% endhint %}

![[Figure 1.3.7.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      Set the communication speed of DeviceNet (to be the same as that of the slave). 
{% endhint %}

![[Figure 1.3.7.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address of the slave slot in the address table.
{% endhint %}

![[Figure 1.3.7.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      Set whether to use the quick connect function.
{% endhint %}

![[Figure 1.3.7.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_26.png>)


{% hint style="info" %}
\.      When the settings are completed, proceed with the download.
{% endhint %}

![[Figure 1.3.7.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_27.png>)

<br>

##### 13. Check the communication status.

{% hint style="info" %}
\.        The communication status needs to be checked in SYCON.net and teach pendant.

\.        Please refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.
{% endhint %}

{% hint style="info" %}
\.      Double-clicking the connected master device will enable you to check the communication status.
{% endhint %}

![[Figure 1.3.7.2-28 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_28.png>)

![[Figure 1.3.7.2-29 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.        Using the diagnosis function of SYCON.net will enable you to monitor the IO’s input and output status along with the communication status.
{% endhint %}

![[Figure 1.3.7.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_30.png>)

<br>

##### 14. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.7.3 Specifications of a DeviceNet Slave


<br>

##### Protocol Characteristics

| **Classification**        | **Specification**         |
| :---                      | :---                      |
| Maximum input byte size   | 255 bytes                 |
| Maximum output byte size  | 255 bytes                 |
| IO connection (implicit)  |                           |
| IO connection             | Bit Strobe, Change of State, Cyclic, Poll |
| Minimum IO cycle time     |                           |
| Communication speed       | 125–500 Kbit/s            |
| Auto baud rate detection  | Not supported             |
| Quick connect             |                           |
| Topology                  |                           |


<br>

##### Network Characteristics

| **Classification**             | **Specification**    |
| :---                           | :---                 |
| Data transport layer           | CAN frames           |
| Hub                            | None                 |
| Switch                         | None                 |# 1.3.7.4 Setting a DeviceNet Slave

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      **[DeviceNet Slave EDS File Download]**

\.      Please refer to “[**5. Slave Device Description Files**](../../../5-slave-config-file.md).”
{% endhint %}

<br>

{% hint style="info" %}
\.      Refer to the following for the connection of the DeviceNet connector.

\.      (“[**1.2.2 Connectors**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)”)
{% endhint %}

<br>

##### 1. By using the teach pendant, select the DeviceNet slave in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.7.4-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 1.3.7.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If the Config file set using SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave PCI Slot Configuration > DeviceNet Slave]**

![[Figure 1.3.7.4-3 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_3.png>) 

![[Figure 1.3.7.4-4 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of Each Item.

{% hint style="info" %}
\.      [Station Address = Mac ID]

\.      DeviceNet identifies a slave via the station address (MAC ID) (1–63).
{% endhint %}

{% hint style="info" %}
\.      [Baudrate]

\.      Select among 125 Kbit/s, 250 Kbit/s, and 500 Kbit/s.
{% endhint %}

{% hint style="info" %}
\.      [Input Bytes]

\.      Input Bytes: To set the size of data to be inputted from the master to the slave
{% endhint %}

{% hint style="info" %}
\.      [Output Bytes]

\.      Output Bytes: To set the size of data to be outputted from the slave to the master
{% endhint %}


<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.

Please refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

![[Figure 1.3.7.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_5.png>) 

<br>

##### 6. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.7.5 Actions for a DeviceNet Error

<br>

Please refer to “[**1.4.1 ERROR Code.**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md).”

<br>

##### 1. DeviceNet Terminating Resistance

{% hint style="info" %}
\.      When connecting the cable for DeviceNet, it is necessary to add resistance to the termination.

\.      If the network scan does not work, check the terminating resistance.

\.      DeviceNet terminating resistance: 120 ohms
{% endhint %}

{% hint style="info" %}
\.      As shown in the figure below, if the CIFX-50 DN PCI is the termination of DeviceNet, add terminating resistance.
{% endhint %}

![[Figure 1.3.7.5-1 DeviceNet Terminating Resistance]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_1.png>) 

{% hint style="info" %}
\.      As shown in the figure below, if the DeviceNet remote IO is the termination, add terminating resistance or operate the DIP switches.
{% endhint %}

![[Figure 1.3.7.5-2 DeviceNet Terminating Resistance]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_2.png>) 

<br>

##### 2. Communication Speed

{% hint style="info" %}
\.      If the communication speeds of the DeviceNet master and slave are different from each other, the network scan may not be performed.

\.      If the network scan does not work, check the communication speed.
{% endhint %}

![[Figure 1.3.7.5-3 DeviceNet Baudrate]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_3.png>) 

<br>

##### 3. DeviceNet Error

{% hint style="info" %}
\.      If there is no power supply of 24 V to the cable of DeviceNet, the following error will appear.

\.      Check the power supply of 24 V.
{% endhint %}

![[Figure 1.3.7.5-4 DeviceNet Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_4.png>) # 1.3.7.6 Object of DeviceNet


<br>

##### 1. Object


The device is Modeled as a collection of objects. Object modeling organizes related data and procedures into one entity : the object.

<br>

![[Figure 1.3.7.6-1 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_1.png>) 


<br>

Object is identified by class code.

<br>

![[Figure 1.3.7.6-2 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_2.png>)

<br>

Inside the object, it consists of an Instance number and a Attribute ID.

<br>

You can access the Attribute of a specific Instance through the "Explicit Message"  from the DeviceNet Master.

<br>

{% hint style="info" %}
\.      EX) Object of "Crevis GN-9212" (You can check this data through the Company "user manual".)

\.      Identity Object (Class Code 0x01) - Read Vendor ID 

\.      Instance : 1

\.      Attribute ID : 1

\.      Access : Get (Read Only)
{% endhint %}


![[Figure 1.3.7.6-3 DeviceNet Object Crevis GN-9212]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_3.png>)


<br>

Each object and its Internal Instance / Attribute have access rights. 

<br>

{% hint style="info" %}
\.      Access

\.      Get : Read

\.      Set : Write

\.      Attribute Single : Only one Attribute can be accessed at a time.

\.      Attribute All : Access all Attributes at once.
{% endhint %}

<br># 1.3.8 CC-Link

This chapter describes the characteristics of CC-Link slaves and the methods to set them.


<br>

##### Fieldbus Overview

Fieldbus is an open industry standard for operating devices such as sensors, buttons, motor drivers, and operation interfaces in a factory by connecting them to a PLC using a single cable.

Fieldbus provides intelligent services such as monitoring the status of the entire network or reconfiguring it from a central location.

For example, Fieldbus makes it possible to set detailed information, operation, and modes of sensors and switches, not just their simple on/off operations.

The use of a single cable helps reduce the time and cost of wiring and makes the configuration simple, which is advantageous for maintenance. 

Moreover, unlike other protocols that have characteristics of the non-deterministic response of general communication, Fieldbus guarantees data response speed, satisfying industrial applications where the characteristics of critical time are important.

![[Figure 1.3.8-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/image_1.png>) 

<br>

One master and multiple slaves can be connected to one Fieldbus network.
The master device searches/manages the entire network and exchanges data with slave devices.

In general, a PLC is a master device, and other devices such as sensors, buttons, and controllers can be configured as slave devices.# 1.3.8.1 Specifications of a CC-Link Slave

<br>

##### Protocol Characteristics

| **Classification**         | **Specification**  (Version 1.11)    | **Specification**  (Version 2.0)  |
| :---                       | :---                                 | :---                              |
| Maximum input byte size    | 48 bytes                             | 368 bytes                         |
| Maximum output byte size   | 48 bytes                             | 368 bytes                         |
| IO station input           | 4 bytes(RY)                          | Not supported                     |
| IO station output          | 4 bytes(RX)                          | Not supported                     |
| Station                    | 1–4                                  | 1–4                               |
| Extension cycle            | Not supported                        | 1, 2, 4, and 8                    |
| Remote device input        | 16 bytes (RY), 32 bytes (RWw)        | 112 bytes (RY), 256 bytes (RWw)   |
| Remote device output       | 16 bytes (RX), 32 bytes (RWr)        | 112 bytes (RY), 256 bytes (RWr)   |
| Communication speed        | 156 Kbit/s–10000 Kbit/s              | 156 Kbit/s–10000 Kbit/s           |



<br>

##### Network Characteristics

| **Classification**            | **Specification**     |
| :---                          | :---                  |
| Data transport layer          |                       |
| Hub                           | None                  |
| Switch                        | None                  |


<br>

##### CC-Link IO Mapping

<br>

{% hint style="info" %}
\.        CC-Link Version 1
{% endhint %}

<br>

![[Figure 1.3.8.1-1 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Single
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Double
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Quadruple
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Octuple
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_5.png>)

<br># 1.3.8.2 Setting a CC-Link Slave

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” first and proceed with the following methods.
<br>

{% hint style="info" %}
\.      Refer to the following for the connection of the CC-Link connector.

\.      (“[**1.2.2 Connectors**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)”)
{% endhint %}

<br>

##### 1. By using the teach pendant, select the CC-Link slave in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.8.4-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 1.3.8.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If the Config file set using SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave PCI Slot Configuration > CC-Link Slave]**

![[Figure 1.3.8.4-3 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>) 

![[Figure 1.3.8.4-4 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of Each Item

{% hint style="info" %}
\.      [Station Address]

\.      CC-Link identifies a slave via the station address (1–64).
{% endhint %}

{% hint style="info" %}
\.      [Baud Rate]

\.      Can be selected among 156 Kbit/s, 625 Kbit/s, 2500 Kbit/s, 5000 Kbit/s, and 10000 Kbit/s
{% endhint %}

{% hint style="info" %}
\.      [CC-Link Version]

\.      Version 1: An IO station can be used. The extension cycle function cannot be used.

\.      Version 2: An IO station cannot be used. The extension cycle function can be used.
{% endhint %}

{% hint style="info" %}
\.      [Number of Station]

\.      IO Station: One IO station is occupied.

\.      Remote Device: Can select 1 to 4 devices

\.      Depending on Number of Station, the size of the IO byte area to be assigned will vary.
{% endhint %}

{% hint style="info" %}
\.      [Extension Cycle]

\.      Can be used in Version 2

\.      Remote Device: Can select among Single, Double, Quadruple, and Octuple

\.      Depending on Extension Cycle, the size of the IO byte area to be assigned will vary. 
{% endhint %}

<br>

{% hint style="info" %}
\.      **For the IO byte area, please refer to the following link.**

\.      **(“[**1.3.8.1 Specifications of a CC-Link slave**](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md)”)**
{% endhint %}

<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.

Please refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

<br>

##### 6. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.8.3 Actions for a CC-Link Slave Error

<br>

Please refer to “[**1.4.1 ERROR Code.**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md).”

<br>

##### 1. CC-Link Terminating Resistance

{% hint style="info" %}
\.      When connecting the cable for CC-Link, it is necessary to add resistance to the termination.

\.      If communication is not connected, check the terminating resistance.

\.      CC-Link terminating resistance: 110 ohms
{% endhint %}

{% hint style="info" %}
\.      As shown in the figure below, if the CIFX-50 CC PCI is the termination of CC-Link, add terminating resistance.
{% endhint %}

![[Figure 1.3.8.5-1 CC-Link Terminating Resistance]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/5-Error/image_1.png>) 



##### 2. CC-Link Error

{% hint style="info" %}
\.      For communication connection, there should be a power supply of 24 v to the CC-Link cable.

\.      If communication is not connected, check the power supply of 24 V.
{% endhint %}
# 1.3.9 CC-Link IE Field

The preparation of the manual is in progress.
# 1.3.10 EtherNet/IP - Connection of a Standard Remote IO

<br>

This chapter describes how to connect several standard remote IO modules selected by our company using the EtherNet/IP scanner (master).

<br>

{% hint style="info" %}
\.      For the EtherNet/IP scanner (master), the CIFX-50 real-time Ethernet PCI is used.


\.     For the remote IO module, the M9289 EtherNet/IP network adapter of Crevis is used.
{% endhint %}

# 1.3.10.1 EtherNet/IP - Setting the Connection of a Standard Remote IO

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” first and proceed with the following methods.

<br>

##### 1. Select the EtherNet/IP Master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.10.1-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 1.3.10.1-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

##### 3. For communication, connect the cables for the PCI and remote IOs and check their status.

![[Figure 1.3.10.1-3 Hardware Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[Figure 1.3.10.1-4 Hardware Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

<br>

{% hint style="info" %}
\.      Connect the PCI and remote IO using the LAN cable.

\.      Set all DIP switches of the remote IO to the Off state.

\.      Connect every remote IO power and field power (24 V DC).
{% endhint %}

<br>

{% hint style="info" %}
\.      The factory set IP address of the remote IO M9289 of the Crevis is 192.168.100.99. 

\.      For the communication to be connected, the IP address of the remote IO should be set as 192.168.100.99.

\.      “[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)”
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave PCI Slot Configuration > EtherNet/IP Remote IO Setting]**

![[Figure 1.3.10.1-5 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>) 

![[Figure 1.3.10.1-6 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>) 

<br>

{% hint style="info" %}
\.      The IP address is set as a fixed value.

\.      Check the Input Bytes and Output Bytes.

\.      The number of selected inputs and outputs should be equal to or less than the number of IOs of the cards mounted in the remote IO slot.
{% endhint %}

<br>

{% hint style="info" %}
\.      Input Module  
\.      M12DF: Digital 16 points  
\.      M3534: Analog 4 points  
{% endhint %}

{% hint style="info" %}
\.      Output Module  
\.      M225F: Digital 16 points  
\.      M226F: Digital 16 points  
\.      M2768: Digital 8 points  
\.      M4534: Analog 4 points  
{% endhint %}

{% hint style="info" %}
\.      Special Module   
\.      M5112: Conveyer I/F 
{% endhint %}

<br>

##### 5. After the settings are completed, reboot the controller.

![[Figure 1.3.10.1-7 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>) 

![[Figure 1.3.10.1-8 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
\.      After the settings are completed, reboot the controller.
{% endhint %}

<br>

##### 6. Check whether the set values are reflected and then check the communication status.

![[Figure 1.3.10.1-9 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>) 

Please refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

![[Figure 1.3.10.1-10 Industrial Commuication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>) 

{% hint style="info" %}
\.      If the communication is not connected, check the IP address of the remote IO.

\.      Check according to the following (if not 192.168.100.99).

\.      “[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)”
{% endhint %}

![[Figure 1.3.10.1-11 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>) 

![[Figure 1.3.10.1-12 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>) 

<br>

##### 7. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}# 1.3.10.2 Setting the Remote IO IP Address

This shows how to set the IP address of the Crevis M9289 EtherNet/IP network adapter.

<br>

{% hint style="info" %}
\.      The factory set IP address of the remote IO M9289 of the Crevis is 192.168.100.99.

\.      If the IP address of the remote IO is not known or needs to be changed, comply with the following.
{% endhint %}

<br>

##### 1. Connect the PC and remote IO directly using the LAN cable.

![[Figure 1.3.10.2-1 LAN Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

##### 2. Change only the DIP switch 9 of the remote IO adapter to the On state.

![[Figure 1.3.10.2-2 DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

##### 3. Run the Bootpsvr.exe program.
   * The program is to be provided by Crevis. (Download IO Guide Pro from the company’s website and install it.)

![[Figure 1.3.10.2-3 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[Figure 1.3.10.2-4 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
\.      While pressing the Start BootP button, disconnect the power of the M9289 module and apply it again to reboot it.
{% endhint %}

![[Figure 1.3.10.2-5 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>


##### 4. When the adapter device is rebooted, the device information will appear in the BootSvr.exe program.

![[Figure 1.3.10.2-6 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

##### 5. Select a device and set the IP address.

![[Figure 1.3.10.2-7 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[Figure 1.3.10.2-8 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

##### 6. After changing all DIP switches of the adapter whose IP settings are complete to the Off state, reboot the device.

{% hint style="info" %}
\.      You must check the status of the DIP switches and whether the adapter is rebooted.
{% endhint %}

![[Figure 1.3.10.2-9 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

##### 7. Check the IP address by using some methods such as a ping test in the PC.

![[Figure 1.3.10.2-10 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

##### 8. If the IP address is normally changed, proceed with the settings.

{% hint style="info" %}
\.      Please proceed with settings according to the  procedures of “[**1.3.10.1 EtherNet/IP - Setting the Connection of a Standard remote IO**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md).”
{% endhint %}
# 1.4 CIFX PCI - Monitoring Industrial Communication

After setting the communication according to the procedures of “[**1.2 CIFX PCI - Installing and Setting Industrial Communication Cards**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)” and “[**1.3 CIFX PCI - Setting Industrial Communication**](../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md),” you can check the operations in the following screens.

You can enter the screens by touching **\[Service > 19: Industrial Communication Monitoring]**, and check the details such as the set firmware information, communication status, and communication configuration in relevant screens.

{% hint style="info" %}
\.      The industrial communication of the relevant PCI communication card can be restarted using the **\[Restart]** button.

\.      Check the status of the slot, firmware, and devices.

\.      When it comes to the master, check the slave configuration and whether the configured slaves are the same as the active slaves in the number. 
{% endhint %}

![[Figure 1.4-1 Industrial Communication Monitoring]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_1.png>)


# 1.4.1 ERROR Code

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>

<br>

<table class="tg">
<thead>
	<tr>
		<th>Error Code</th>
		<th>Description</th>
		<th>Action</th>
	</tr>
</thead>

<tbody>
	<tr>
		<td>0x00000000</td>
		<td>No Error</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xC000000C</td>
		<td>Watchdog Timeout between PCI and Robot Controller</td>
		<td>Check PCI and robot controller status. It can be reset by restarting communication.</td>
	</tr>
    <tr>
		<td>0xC0000123</td>
		<td>Insufficient License</td>
		<td>Check whether PCI master license exists</td>
	</tr>
    <tr>
		<td>0xC0000140</td>
		<td>Communication fault</td>
		<td>Check for any inactive device or check the connection status.</td>
	</tr>
    <tr>
		<td>0xC0000141</td>
		<td>Connection closed</td>
		<td>Check for any inactive device or check the connection status.</td>
	</tr>
    <tr>
		<td>0xC0000142</td>
		<td>Connection timeout</td>
		<td>Check for any inactive device or check the connection status.</td>
	</tr>
    <tr>
		<td>0xC0000144</td>
		<td>Duplicate IP address</td>
		<td>Change any duplicated IP address.</td>
	</tr>
    <tr>
		<td>0xC0000145</td>
		<td>Cable disconnected</td>
		<td>Check the cable connection status.</td>
	</tr>
    <tr>
		<td>0xC0000180</td>
		<td>Bus Off Flag is Set</td>
		<td>Reset the device.</td>
	</tr>
    <tr>
		<td>0xC0470298</td>
		<td>DevieNet 24V Power Missing</td>
		<td>Check DeviceNet network 24V power</td>
	</tr>
    <tr>
		<td>0xC062002C</td>
		<td>DevieNet Slave 24V Power Missing</td>
		<td>Check DeviceNet network 24V power</td>
	</tr>
</tbody>
</table>

# 3. EtherCAT Master IO

<br>

This chapter describes how to connect several standard remote IO modules selected by our company using the EtherCAT Master.

<br>

##### EtherCAT Overview

EtherCAT is an Ethernet-based Fieldbus system developed by Beckhoff Automation.

The EtherCAT protocol provides functions for very fast IO data updates and accurate synchronization.

<br>

##### EtherCAT Master IO
   * The product corresponds to the existing Fieldbus master and can make a request for IO data connection to the EtherCAT slaves

<br>

{% hint style="info" %}
\.      For the EtherCAT master, Use the LAN port of the Controller.


\.     For the remote IO module, the M9386 EtherCAT network adapter of Crevis is used.
{% endhint %}


# 3.1 Setting the EtherCAT Master IO

<br>

##### 1. Click the menu to enter the setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 4: EtherCAT Master Settings]**

<br>

![[Figure 3.1-1 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_1.png>) 

<br>

{% hint style="info" %}
\.      Check the controller LAN port number on ther EtherCAT Master Settings screen.
{% endhint %}

##### 2. For communication, connect the cables for the controller LAN port and remote IOs and check their status.

<br>

![[Figure 3.1-2 Cable Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_2.png>) 
![[Figure 3.1-3 Cable Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_3.png>) 

<br>

{% hint style="info" %}
\.      Connect the controller LAN port and remote IO using the LAN cable.

\.      Set all DIP switches of the remote IO to the Off state.

\.      Connect every remote IO power and field power (24 V DC).
{% endhint %}

<br>

##### 3. Select whether to use EtherCAT Master to ON in the settings screen.

<br>

![[Figure 3.1-4 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_4.png>) 

<br>

{% hint style="info" %}
\.      Select the communication cycle time.

\.      Supported 1ms, 2ms, 5ms
{% endhint %}

<br>

##### 4. On the settings screen, Select configured module from the slave device list.

<br>

![[Figure 3.1-5 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_5.png>)

<br>

{% hint style="info" %}
\.      Check the Input Bytes and Output Bytes.
{% endhint %}

<br>

{% hint style="info" %}
\.      Input Module  
\.      M12DF: Digital 16 points  
\.      M3534: Analog 4 points  
{% endhint %}

{% hint style="info" %}
\.      Output Module  
\.      M225F: Digital 16 points  
\.      M226F: Digital 16 points  
\.      M2768: Digital 8 points  
\.      M4534: Analog 4 points  
{% endhint %}

{% hint style="info" %}
\.      Special Module   
\.      M5112: Conveyer I/F 
{% endhint %}

<br>

![[Figure 3.1-6 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_6.png>) 

<br>

##### 5. After the settings are completed, reboot the controller.

![[Figure 3.1-7 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_7.png>) 

<br>

![[Figure 3.1-8 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_8.png>) 

<br>

{% hint style="info" %}
\.      After the settings are completed, reboot the controller.
{% endhint %}

<br>

##### 6. Check whether the set values are reflected and then check the communication status.

![[Figure 3.1-9 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_9.png>) 

<br>

{% hint style="info" %}
\.      Please check the communication connection status and error.
{% endhint %}

<br>

![[Figure 3.1-10 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_10.png>)

<br>

{% hint style="info" %}
\.      Please check ther LED on the Remote IO Module if communication is working properly.
{% endhint %}

<br>

{% hint style="info" %}
\.      **If error occurs, Please check the following : (“[**3.2 Action for the EtherCAT Master IO Error**](../3-ethercat-master-io/2-Error-EtherCAT-Master.md)”)**
{% endhint %}

<br>

##### 7. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../4-io-block-allocation.md)”)**
{% endhint %}

# 3.2 Action for the EtherCAT Master IO Error

This section describes the solutions for major errors that may occur while setting up the EtherCAT Master IO.

<br>

![[Figure 3.2-1 EtherCAT Master Status]](<../_assets/3-ethercat-master-io/2-Error/image_1.png>) 

{% hint style="info" %}
\.      Check the connection status of the LAN cable.

\.      Check whether the adapter device power is switched on.

\.      Please make sure Settings and Remote IO Devices are the same.
{% endhint %}

<br>
# 4. Setting IO Block Allocation of the Industrial Communication

This section shows how to allocate IO blocks for communication with the controller after completing industrial communication settings.

Those blocks should be allocated within the range from fb0 to fb9 to use industrial communication IO.

<br>

##### 1. Select the menu for allocating the IO blocks.
   Touch the menu **\[System > 2: Control Parameter > 2: Input/Output Signal Setting > 6: FB Block Allocation.]** 

<br>

##### 2. Designate the industrial communication type in the desired fb area.
   After designating it, touch the **\[OK]** button.

![[Figure 4-1]](<_assets/4-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[Caution]**: When used together with an embedded PLC, check the IO attributes and DI/DO - X/Y. 
{% endhint %}
# 5. Slave Device Description Files

To configure slave communication in the industrial communication master, the slave device description files for each protocol are to be used.

<br>

The slave description files can be downloaded from our company’s website.
Go to [www.hyundai-robotics.com](http://www.hyundai-robotics.com) -> Industrial Robot pages -> Customer Support -> Application software and then download “**Hi6 Fieldbus Config.**”

<br>

{% hint style="info" %}
\.      EtherNet/IP: EDS files

\.      PROFINET IO: GSDML (.XML) files

\.      EtherCAT: ESI (.XML) files

\.      PROFIBUS-DP: GSD files

\.      DeviceNet: EDS files

\.      CC-Link IE Field: CSPP files

\.      CC-Link IE Basic: CSPP files
{% endhint %}

<br>

# ${cont_model} Robot Controller Function Manual - Industrial Communication

{% hint style="warning" %}
The information provided in this product manual is the property of HD Hyundai Robotics.

Without written consent from HD Hyundai Robotics, all or part may not be reproduced or redistributed without permission, nor may it be provided to third parties or used for other purposes.



This manual may be changed without prior notice.



**Copyright © 2020 by Hyundai Robotics**
{% endhint %}
# 1. CIFX PCI Communication

This is a manual for the industrial communication that uses a CIFX PCI. 
# 1.1 CIFX PCI Program Installation

This is the method for installing programs related to industrial communication.
# 1.1.1 SYCON.net Installation

"Sycon.net" is a program provided by Hilscher for configuring the PCI communication card.

<br>

##### 1. SYCON.net Latest Version Download Path

{% hint style="info" %}
\.      Click **[https://hilscher.atlassian.net/](https://hilscher.atlassian.net/wiki/spaces/HILKB/overview?mode=global) -> Software -> SYCON.net**.
{% endhint %}

<br>

![[Figure 1.1.1-1 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_1.png>)

<br>

![[Figure 1.1.1-2 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_2.png>)

<br>

{% hint style="info" %}
\.      Select the latest version (current release) and download it.
{% endhint %}

<br>

![[Figure 1.1.1-3 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_3.png>)

<br>

![[Figure 1.1.1-4 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_4.png>)

<br>

{% hint style="info" %}
\.      Execute the downloaded SYCON.NET Setup.exe file to install the program.
{% endhint %}

<br>

![[Figure 1.1.1-5 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_5.png>)

<br>

![[Figure 1.1.1-6 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_6.png>)

<br>

{% hint style="info" %}
\.      Execute the installed SYCON.NET program to check that the installation has been completed successfully.
{% endhint %}

<br>

![[Figure 1.1.1-7 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_7.png>)

<br>


##### 2. Download the Program from the Hyundai Robotics Website.

{% hint style="info" %}
\.      Download "**Sycon.net**" from [www.hd-hyundairobotics.com](https://hd-hyundairobotics.com/) -> Industrial Robot Website -> Customer Support -> Application Software.
{% endhint %}

<br>

{% hint style="info" %}
\.      Extract -> Execute the SYCON.NET Setup.exe file to install the program.
{% endhint %}

<br>

{% hint style="info" %}
\.      The SYCON.net program provided on our website may differ from the latest version.
{% endhint %}

<br># 1.2 CIFX PCI Communication Card Installation and Settings

To use industrial communication, a PCI communication card (from Hilscher) is required. Set the communication card and wire the connectors according to the required communication.
# 1.2.1 PCI Industrial Communication Card


<br>

##### 1. Install the purchased PCI communication card inside the controller's Main Module.

<br>

##### 2. Rotate the rotary switch of the PCI communication card to set the Slot number.

<br>

{% hint style="warning" %}
**\[Caution]**: The physical location of the PCI slot is independent of the rotary switch settings on the communication card.
{% endhint %}

<br>

##### 3. Set the slot number separately for each PCI communication card within the number ranging 1 \~ 3.
  (When multiple PCI communication cards are used, individual numbers should be set differently.)

![[Figure 1.2.1-1 PCI Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_2.png>)

<br>

![[Figure 1.2.1-2 PCI Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_3.png>)

{% hint style="warning" %}
**\[Caution]**: Please set the rotary switch number differently for each PCI card.
{% endhint %}

# 1.2.2 Connector

<br>

##### Use connectors and cables suitable for the industrial communication method.

![[Figure 1.2.2-1 Industrial Communication Connector]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector/image_2.png>)

{% hint style="info" %}
\.      DeviceNet termination resistor: 120 ohms

\.      CC-Link termination resistor: 110 ohms
{% endhint %}

<br>

{% hint style="warning" %}
**\[Caution]**: Please use separate power sources for the communication cable and the IO.
{% endhint %}

<br># 1.2.3 LED Description

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
# 1.3 CIFX PCI Communication Settings

To use industrial communication, install a PCI communication card, and proceed with settings using the teach pendant and Sycon.net program.
# 1.3.1 CIFX PCI Slot Settings.

Configure the communication method for the CIFX PCI slot. To apply the settings, please disconnect the controller power and then supply it again.

<br>

Refer to "[**1.2.1 PCI Industrial Communication Card**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" and proceed with the method below.

<br>

##### 1. Touch the menu to enter the slot settings screen.
**\[System > 2: Control Parameters > 11: Industrial Communication > 1: PCI Slot Settings > Channel 1]** 


<br>

##### 2. Refer to the screen below to select the slot, communication method (master/slave), and protocol.
   * The slot number is the rotary switch number of the PCI communication card.
   * If you do not want to change the communication settings, touch the **\[OK]** button to exit.

{% hint style="warning" %}
**\[Caution]**: Touching the **\[Initialize]** or **\[Apply]** button will initialize the slot information on the current tab. The Config file will also be initialized, so please be aware.
{% endhint %}

![[Figure 1.3.1-1 PCI Slot Settings]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[Figure 1.3.1-2 PCI Slot Settings (master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[Figure 1.3.1-3 PCI Slot Settings (Slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

##### 3. Complete the slot settings.
Touch the **\[Apply]** menu.

![[Figure 1.3.1-4 PCI Slot Settings]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[Caution]**

<1>. When applying the settings by touching the **\[Apply]** button, all CONFIG files applied to the corresponding slot will be deleted and changed. It is recommended to keep a separate backup of existing settings when changing communication.

<2>. If you touch the **\[OK]** button without touching the **\[Apply]** button, the selected communication will not be applied.
{% endhint %}

<br>

##### 4. Repeat steps 2. \~ 3. for each slot.

<br>

##### 5. Reboot the controller to apply the set communication.
Touch the **\[Service > 19: Industrial Communication Monitoring]** menu to check if the set communication has been applied.

![[Figure 1.3.1-5 Industrial Communication Settings Screen]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[Caution]**: Settings are applied when the controller is rebooted after slot settings.
{% endhint %}
# 1.3.2 SYCON.NET Settings

For the PCI communication card, proceed with industrial communication settings using the "**Sycon.net**" program. The setting method is as follows. (Please install by referring to "[**1.1 Sycon.net Installation**](../../1-cifx-pci-install-program/1-sycon-net.md)".)

<br>

##### 1. Connect the PC with Sycon.net installed and the general LAN port of the robot controller (not the PCI LAN port).
Touch the **\[System > 2: Control Parameters > 9: Network]** menu to check the IP of the general LAN port. Please check the connection status through a ping test, etc.

![[Figure 1.3.2-1 Network IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_1.png>)
![[Figure 1.3.2-2 Network IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_2.png>) 

{% hint style="info" %}
\.      IP Address can be changed according to user settings.
{% endhint %}

<br>

##### 2. Execute Sycon.net.

![[Figure 1.3.2-3 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_3.png>)

<br>

##### 3. In the Device Catalog menu on the right side of the screen, click the item matching the set communication protocol and place it on the bus line in the center by dragging and dropping it.

![[Figure 1.3.2-4 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_4.png>)
![[Figure 1.3.2-5 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_5.png>)

<br>

##### 4. Double-click the imported item to set it.

{% hint style="info" %}
\.      "Double-click" the imported CIFX PCI (figure).

\.      Settings -> Driver

\.      Select netX Driver.
{% endhint %}

![[Figure 1.3.2-6 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_6.png>)

{% hint style="info" %}
\.     Setting -> Driver -> netX Driver -> TCP Connection

\.     IP Address: Please enter the general LAN port IP address of the connected controller.
{% endhint %}

![[Figure 1.3.2-7 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_7.png>)

{% hint style="info" %}
\.      Device Assignment -> Click Scan

\.      Select communication (check the channel protocol) then "Apply" and "OK."
{% endhint %}

{% hint style="warning" %}
**\[Caution]**: Please be sure to check the Channel Protocol and Slot number.
{% endhint %}

{% hint style="warning" %}
**\[Caution]**: If scan is not working, check the status of the cable connection with the controller and also the firmware settings.
{% endhint %}

![[Figure 1.3.2-8 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_8.png>)


{% hint style="info" %}
\.      Right-click the CIFX PCI figure -> Download
{% endhint %}

![[Figure 1.3.2-9 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_9.png>)# 1.3.2.1 SYCON.NET Help



<br>

##### When using SYCON.net, if there are insufficient explanations in the manual, please refer to the "help" function below.

<br>

![[Figure 1.3.2.1-1 SYCON.net help]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/1-Help-SYCON/image_1.png>) 

<br>

![[Figure 1.3.2.1-2 SYCON.net help]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/1-Help-SYCON/image_2.png>) 

<br># 1.3.3 EtherNet/IP

This chapter describes the characteristics of the EtherNet/IP master (scanner) and slave (adapter) and how to set them. 

<br>

##### EtherNet/IP Overview

EtherNet/IP is an Ethernet-based open industrial communication protocol developed by CI (ControlNet International) and ODVA (Open DeviceNet Vendors Association).

In the factory, various devices such as sensors, remote IOs, motor drivers, HMIs, PLCs, and robot controllers can be connected to one EtherNet/IP network regardless of manufacturer.

![[Figure 1.3.3-1 EtherNet/IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/image_1.png>)


<br>

EtherNet/IP is classified as follows according to the communication function.

##### Scanner Class
   * Products that correspond to existing fieldbus masters and can ask the EtherNet/IP adapters or scanners to perform I/O data connection.

<br>

##### Adapter Class
  * Products that correspond to existing fieldbus slaves and are the targets of Real-Time I/O data connections requested by EtherNet/IP scanners.

  * An adapter cannot send and receive Real-Time I/O data on their own without the scanner.

<br>

##### Messaging Class
   * Products that can send and receive explicit messages for the products of all classes, but do not support Real-Time I/O data transmission and reception.

   * For example, the products can be computer interface cards for program upload/download and network setting tools, etc.# 1.3.3.1 EtherNet/IP Scanner Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Maximum Connectable Slave Count</td>
		<td>64</td>
	</tr>
    <tr>
		<td>Maximum Input Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Input Size (1 slave)</td>
		<td>504 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size (1 slave)</td>
		<td>504 bytes</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td>Cyclic</td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td>Min. 1ms</td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Tree, Line, Ring</td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>DLR (Device Level Ring)</td>
		<td>Beacon based 'Ring Node'</td>
	</tr>
    <tr>
		<td>Additional Features</td>
		<td>DHCP, BOOTP, ACD supported</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>10 or 100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>Allowed</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>Allowed</td>
	</tr>
</tbody>
</table>
<br>

##### Connection

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Cable</td>
		<td>Minimum of Cat5, STP</td>
	</tr>
	<tr>
		<td>length</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>
# 1.3.3.2 EtherNet/IP Scanner Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[**1.3.2 SYCON.NET Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
\.      When using SYCON.net, if there are insufficient explanations in the manual, please refer to the "[**1.3.2 SYCON.NET Help**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" function.
{% endhint %}

<br>

##### 1. Select EtherNet/IP Master in the PCI slot settings and reboot the robot controller.

![[Figure 1.3.3.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_1.png>)

<br>

##### 2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.

<br>

{% hint style="info" %}
\.        For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.3.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the EtherNet/IP scanner PCI device by using Sycon.net.

![[Figure 1.3.3.2-3 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_3.png>)
![[Figure 1.3.3.2-4 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan the PCI device and apply the EtherNet/IP scanner.

![[Figure 1.3.3.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

##### 5. Download the settings.

![[Figure 1.3.3.2-6 EtherNet/IP Scanner Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare the adapter (slave) module to be connected to the EtherNet/IP scanner.
   * In this example, we use the M9289 EtherNet/IP adapter from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.3.2-7 Crevis M9289]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

##### 7. Set the IP address of the adapter (slave) for EtherNet/IP communication connection.

{% hint style="info" %}
\.      Setting an IP address using the dip switch.
{% endhint %}

![[Figure 1.3.3.2-8 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
\.      How to set an IP address using BootpSvr.exe
{% endhint %}

<br>

##### 8. (Bootp example) Set the slave device IP address using Bootp.
   * Change only DIP switch 9 to ON.

![[Figure 1.3.3.2-9 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_9.png>)

   * Connect the PC to the M9289 adapter LAN port.

![[Figure 1.3.3.2-10 Crevis M9289 LAN Port]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

##### 9. Execute BootpSvr.exe on the PC.
   * This program is provided by Crevis. (Download and install IO Guide Pro from the website.)

![[Figure 1.3.3.2-11 Crevis IO Guide Pro]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_11.png>)

![[Figure 1.3.3.2-12 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
\.      With Start BootP being pressed, disconnect and reapply power to the M9289 module to reboot it.
{% endhint %}

![[Figure 1.3.3.2-13 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

##### 10. When the adapter device is rebooted, the device information will appear in the BootpSvr.exe program.

![[Figure 1.3.3.2-14 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

##### 11. Select the device and set the IP.

![[Figure 1.3.3.2-15 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_15.png>)![[Figure 1.3.3.2-16 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

##### 12. After setting the IP, turn all DIP switches of the adapter to OFF and reboot the device.

{% hint style="info" %}
\.      Be sure to check the DIP switch status and whether the adapter is rebooted.
{% endhint %}

![[Figure 1.3.3.2-17 Crevis DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

##### 13. Register the slave device EDS file.

{% hint style="info" %}
\.      An EDS file is required to use a device not registered in Sycon.net.

\.      The EDS file for M9289 adapter can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.3.2-18 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
\.      Register the downloaded EDS file in Sycon.net.

\.      When registering an EDS file, please check the industrial communication protocol (EtherNet/IP).
{% endhint %}

![[Figure 1.3.3.2-19 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_19.png>)![[Figure 1.3.3.2-20 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_20.png>)
![[Figure 1.3.3.2-21 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_21.png>)

![[Figure 1.3.3.2-22 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

##### 14. Network Scan

{% hint style="info" %}
\.      The EtherNet/IP scanner does not support the Network Scan function.
{% endhint %}

<br>

##### 15. Configure the slave (adapter) device

{% hint style="info" %}
\.      Drag the registered device and place it on the EtherNet/IP master bus line.
{% endhint %}

![[Figure 1.3.3.2-23 Sycon.net Bus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      Double-click the device (adapter) to proceed with settings.

\.      Set the input/output byte count appropriate for the IO device installed in that device.

\.      In this example, settings were made as follows.
{% endhint %}

<br>

![[Figure 1.3.3.2-24 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.        O -> T : Originator(Master) -> Target (Slave)

\.        Output : EtherNet/IP Scanner  -> M9289

\.        [Output Module]   
\.         1. M225F (2Bytes)   
\.         **=> 2Bytes**   
{% endhint %}

<br>

![[Figure 1.3.3.2-25 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.        T -> O : Target (Slave) -> Originator(Master)

\.        Input : M9289 -> EtherNet/IP Scanner

\.        [Input Module]
\.         1. M7001  (1Byte)
\.         2. M12DF  (2Bytes)
\.         **=> 3Bytes**


\.         1.M7002 (0Byte)
\.         2.M12DF (2Bytes)
\.         **=> 2Bytes**  
{% endhint %}

<br>

##### 16. Configure the master (scanner) device.


{% hint style="info" %}
\.        Right-click the master device to disconnect it.
{% endhint %}

![[Figure 1.3.3.2-26 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Double-click the master device.

\.        Set the master device IP address. 
{% endhint %}

![[Figure 1.3.3.2-27 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.      Set the slave device IP address.
{% endhint %}

![[Figure 1.3.3.2-28 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.        Set the slave device scan time. 

\.        Please adjust the corresponding values to set an appropriate communication speed.
{% endhint %}

![[Figure 1.3.3.2-29 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.        Check the slave device settings in the address table.

\.        Check the input/output IO byte count and start address.
{% endhint %}

![[Figure 1.3.3.2-30 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
\.        [Quick Connect]

\.        EtherNet/IP supports the Quick Connect function.
{% endhint %}

{% hint style="info" %}
\.        The following conditions should be met to use the Quick Connect function.

\.        (1) Products that support the Quick Connection function for the master and slaves are required  
\.        (2) Quick Connect cannot be used when using Auto Negotiation  
\.        (3) Quick Connect cannot be used when using Auto MDI-X  
\.        (4) 100 Mbit/s, Full Duplex required  
{% endhint %}

{% hint style="info" %}
\.        After completing the settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.3.2-31 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

##### 17. Check the communication status

{% hint style="info" %}
\.      Check the communication status in Sycon.net and TP.

\.        For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
\.      Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.3.2-32 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_32.png>)

![[Figure 1.3.3.2-33 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
\.        Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.3.2-34 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_34.png>)

<br>

##### 18. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}# 1.3.3.3 EtherNet/IP Adapter Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>Maximum Input Size</td>
		<td>240 bytes (TP) / 504 bytes (Sycon.net)</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>240 bytes (TP) / 504 bytes (Sycon.net)</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td>1 exlusive Owner <br>1 Listen Only <br>1 Input Only</td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td>Min. 1ms</td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Tree, Line, Ring</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>DLR V2 (Device Level Ring)</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>Additional Features</td>
		<td>DHCP, BOOTP, ACD supported</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>10 or 100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>Allowed</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>Allowed</td>
	</tr>
</tbody>
</table>
<br>

##### Connection

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Cable</td>
		<td>Minimum of Cat5, STP</td>
	</tr>
	<tr>
		<td>length</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>
# 1.3.3.4 EtherNet/IP Adapter Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
\.      **[EtherNet/IP Adapter EDS File Download]**

\.      Please refer to "[**5. Slave Device Description File**](../../../5-slave-config-file.md)".
{% endhint %}

<br>

##### 1. Using the TP, select an EtherNet/IP slave in the industrial communication firmware settings and reboot the robot controller.

![[Figure 1.3.3.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the current communication protocol readiness status in industrial communication monitoring menu.

![[Figure 1.3.3.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

##### 3. Touch the menu to enter the slave settings screen.
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > EtherNet/IP Slave]**

![[Figure 1.3.3.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.3.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of each item

{% hint style="info" %}
\.      [IP Setting]

\.      Fixed IP: User sets the IP address, subnet mask, and gateway information.

\.      Dynamic Allocation (DHCP): An IP address is assigned from the DHCP server.
{% endhint %}

{% hint style="info" %}
\.      [Input Upon Communication Error (Action in Bus Error)]

\.      Clear: Initializes all inputs to 0 when a communication error occurs.

\.      Hold: Maintains the last valid input value when a communication error occurs.
{% endhint %}

{% hint style="info" %}
\.      [Communication Error Allowable Time (Error Allowed Time)]

\.      If a communication error persists for the specified allowed time, a fieldbus error signal and alarm are output.
{% endhint %}

{% hint style="info" %}
\.      [Input Byte Count (Input Byte)]

\.      Input Byte Count: Sets the size of the data input from the master -> slave.

\.      O -> T: Originator(Master) -> Target (Slave)
{% endhint %}

{% hint style="info" %}
\.      [Output Byte Count (Output Byte)]

\.      Output Byte Count: Sets the size of the data output from the slave -> master.

\.      T -> O: Target (Slave) -> Originator (Master)
{% endhint %}

{% hint style="info" %}
\.      [Run / Idle Header]

\.      The CIFX-50 RE EtherNet/IP Adapter applied to the controller uses 32-bit Run/Idle header when exchanging IO with the scanner (default).

\.      Please set whether to use the input and output 32-bit Run/Idle Header appropriately according to the scanner specifications.
{% endhint %}

<br>

{% hint style="info" %}
\.        [Quick Connect]

\.        EtherNet/IP supports the Quick Connect function.

\.        If the Quick Connect function is required, please set the EtherNet/IP Adapter using Sycon.net.

\.        (1) Products that support the Quick Connection function for the master and slaves are required  
\.        (2) Quick Connect cannot be used when using Auto Negotiation  
\.        (3) Quick Connect cannot be used when using Auto MDI-X  
\.        (4) 100 Mbit/s, Full Duplex required  
{% endhint %}

<br>

##### 5. After completing the settings, check the communication status according to the procedure below.

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.3.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_5.png>)

<br>

##### 6. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}# 1.3.3.5 EtherNet/IP Error Handling

This is a method for resolving major errors that may occur during EtherNet/IP settings.

Errors can be checked using the diagnosis function of Sycon.Net.

<br>

Please refer to "[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

<br>

##### 1. Communication cable disconnection error

{% hint style="info" %}
\.      Please check the connection status of the LAN cable.

\.      Check if the adapter device power is on.
{% endhint %}

![[Figure 1.3.3.5-1 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_1.png>) 


<br>

##### 2. IP Address setting error

{% hint style="info" %}
\.      Please check the IP addresses of the master and slave devices.

\.      An error occurs if the set IP address of the adapter device differs from the value entered in Sycon.net.

{% endhint %}

![[Figure 1.3.3.5-2 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_2.png>) 

![[Figure 1.3.3.5-3 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_3.png>) 


# 1.3.4 PROFINET IO

This chapter describes the characteristics of the PROFINET IO master (controller) and slave (device) and how to set them. 

<br>

##### PROFINET IO Overview

PROFINET IO is an Ethernet-based open industrial communication protocol that has progressively evolved from PROFIBUS-DP and industrial Ethernet.

![[Figure 1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>) 

<br>

It follows the Provider-Consumer model for data exchange and can be classified into the following three classes of products.

##### IO Controller Class
   * Products that correspond to existing PROFIBUS-DP class 1 masters and are types of products in which automation programs such PLCs are running.

   * An IO controller supplies output data to the IO devices set to it and consumes the input data from them.

<br>

##### IO Device Class
  * Products that correspond to existing PROFIBUS-DP slaves and are connected to IO controllers such as PLCs through PROFINET IO.

  * An IO device supplies output data to the IO controller, provides input data, and consumes output data.

<br>

##### IO Supervisor Class
   * Products that correspond to existing PROFIBUS-DP class 2 masters and include those programming devices, PCs, HMIs that are designed for network configuration and diagnosis.
# 1.3.4.1 PROFINET IO Controller Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Maximum Connectable Slave Count</td>
		<td>128</td>
	</tr>
    <tr>
		<td>Maximum Input Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Input Size (1 slave)</td>
		<td>1024 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size (1 slave)</td>
		<td>1024 bytes</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td>Min. 1ms</td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>100 Mbit/s (Full-duplex)</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Tree, Line</td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>DCP</td>
		<td>Supported</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>Forbidden</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>Only allowed if the switch supports, Priority Tagging and LLDP</td>
	</tr>
</tbody>
</table>
<br>

##### Connection

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Cable</td>
		<td>Minimum of Cat5, STP</td>
	</tr>
	<tr>
		<td>length</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br># 1.3.4.2 PROFINET IO Controller Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[**1.3.2 SYCON.NET Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
\.      When using SYCON.net, if there are insufficient explanations in the manual, please refer to the ""[**1.3.2 SYCON.NET Help**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" function.
{% endhint %}

<br>

##### 1. Select the PROFINET IO master in the PCI slot settings and reboot the robot controller.

![[Figure 1.3.4.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.

<br>

{% hint style="info" %}
\.        For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.4.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the PROFINET IO controller PCI device by using Sycon.net.

![[Figure 1.3.4.2-3 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_3.png>)
![[Figure 1.3.4.2-4 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan the PCI device and apply the PROFINET IO controller.

![[Figure 1.3.4.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

##### 5. Download the settings.

![[Figure 1.3.4.2-6 PROFINET IO Controller Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare the device (slave) module to be connected to the PROFINET IO controller.
   * In this example, we use the M9287 PROFINET IO device from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.4.2-7 Crevis M9287]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
\.      How to set the PROFINET IO device name using the DIP switch

\.      M9287-XX: Number set using the DIP switch

\.      In this example, the name was set to M9287-01 using DIP switch 1.
{% endhint %}

<br>

##### 7. (DIP switch use example) Set the slave device name using the DIP Switch.
   * Change only DIP Switch 1 to ON.


![[Figure 1.3.4.2-8 Crevis M9287 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      Please reboot the device after setting the DIP switch.
{% endhint %}

<br>

##### 8. Register the slave device GSDML file.

{% hint style="info" %}
\.      A GSDML file is required to use a device not registered in Sycon.net.

\.      The GSDML file for the M9287 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.4.2-9 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      Register the downloaded GSDML file in Sycon.net.

\.      When registering a GSDML file, please check the industrial communication Protocol (PROFINET IO).
{% endhint %}

![[Figure 1.3.4.2-10 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_10.png>)![[Figure 1.3.4.2-11 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_11.png>)
![[Figure 1.3.4.2-12 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_12.png>)

![[Figure 1.3.4.2-13 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_13.png>)


<br>

##### 9. Network Scan

{% hint style="info" %}
\.      The PROFINET IO controller supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the PROFINET IO master device and click Network Scan.
{% endhint %}

![[Figure 1.3.4.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      If there is no GSDML file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

![[Figure 1.3.4.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      If a GSDML file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.4.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_16.png>)

![[Figure 1.3.4.2-17 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_17.png>)

![[Figure 1.3.4.2-18 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

##### 10. Configure the slave (device).

{% hint style="info" %}
\.      Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.4.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 1.3.4.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Add a slot connected to M9287 to set the PROFINET IO slave (device).

\.      Slot 1 : M7001  
\.      Slot 2 : M12DF  
\.      Slot 3 : M225F  
{% endhint %}

![[Figure 1.3.4.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_21.png>)

![[Figure 1.3.4.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

##### 11. Configure the master (controller) device

{% hint style="info" %}
\.      Double-click the Master device.
{% endhint %}

![[Figure 1.3.4.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      Set the IP addresses of the master and slave devices.

\.      The slave IP address of the PROFINET IO Device is to be set from the master.

\.      Please ensure that the IP addresses of the master and slave do not overlap within the same band.
{% endhint %}

![[Figure 1.3.4.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_24.png>)

![[Figure 1.3.4.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      Check from the master device if the slot information of the slave device is correct.
{% endhint %}

![[Figure 1.3.4.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.4.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.      Set the IO communication speed for the PROFINET IO.
{% endhint %}

![[Figure 1.3.4.2-28 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.      After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.4.2-29 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

##### 12. Check the communication status.

{% hint style="info" %}
\.      Check the communication status in Sycon.net and TP.

\.        For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
\.      Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.4.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_30.png>)

![[Figure 1.3.4.2-31 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
\.        Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.4.2-32 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_32.png>)

<br>

##### 13. Assign IO blocks after completing the settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}# 1.3.4.3 PROFINET IO Device Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>Maximum Input Size</td>
		<td>256 bytes (TP) / 1024 bytes (Sycon.net)</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>256 bytes (TP) / 1024 bytes (Sycon.net)</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td>Min. 1ms</td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>100 Mbit/s (Full-duplex)</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Tree, Line</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>DCP</td>
		<td>Supported</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>Forbidden</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>Only allowed if the switch supports, Priority Tagging and LLDP</td>
	</tr>
</tbody>
</table>
<br>

##### Connection

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Cable</td>
		<td>Minimum of Cat5, STP</td>
	</tr>
	<tr>
		<td>length</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>
# 1.3.4.4 PROFINET IO Device Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
\.      **[PROFINET IO Device GSDML File Download]**

\.      Please refer to "[**5. Slave Device Description File**](../../../5-slave-config-file.md)".
{% endhint %}

<br>

##### 1. Using the TP, select a PROFINET IO slave in the industrial communication firmware settings and reboot the robot controller.

![[Figure 1.3.4.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_1.png>)

<br>

##### 2. Check the current communication protocol readiness status in industrial communication monitoring menu.

![[Figure 1.3.4.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

##### 3. Touch the menu to enter the slave settings screen.
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > PROFINET IO Slave]**

![[Figure 1.3.4.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[Figure 1.3.4.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of each item

{% hint style="info" %}
\.      [Station Name]

\.      The PROFINET IO identifies a slave through the station name.

\.      Naming Rule
\.       > Device names connected by PROFINET IO cannot be duplicated.  
\.       > A name can be set up to 240 characters.  
\.       > Special characters "." and "-" can be used.  
\.       > Lowercase English letters and numbers can be used.  
\.       > Names should start and end with lowercase English letters or numbers.  
{% endhint %}

{% hint style="info" %}
\.      [Input Byte Count (Input Byte)]

\.      Input Byte Count: Sets the size of the data input from the master -> slave.
{% endhint %}

{% hint style="info" %}
\.      [Output Byte Count (Output Byte)]

\.      Output Byte Count: Sets the size of the data output from the slave -> master.
{% endhint %}

<br>

{% hint style="info" %}
\.      [**When Setting a Slot from the Master**]

\.      Master Input (32byte)  <--  Slave Output (32bytes)

\.      Master Output (256bytes = 64bytes * 4)  -->  Slave Input (256bytes)

\.      4, 8, 16, 32, and 64 Bytes -> Specify the slot matching each byte count  
\.      128 and 256 Bytes -> Specify multiple 64-byte slots (2, 4)

\.      The input slot is located before the output slot.
{% endhint %}

<br>

![[Figure 1.3.4.4-5 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_5.png>) 


<br>

##### 5. After completing the settings, check the communication status according to the procedure below.

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.4.4-6 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_6.png>)

<br>

##### 6. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}# 1.3.4.5 PROFINET IO Error Handling

<br>

Please refer to "[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".



# 1.3.5 EtherCAT

This chapter describes the characteristics of EtherCAT master and slave and how to set them.

<br>

##### EtherCAT Overview

EtherCAT is an Ethernet-based fieldbus system developed by Beckhoff Automation.

The EtherCAT protocol provides functions for very fast IO data updates and precise synchronization. 

<br>

##### EtherCAT Master
   * Products that correspond to existing fieldbus masters and can ask EtherCAT slave devices to perform I/O data connection.

<br>

##### EtherCAT Slave
   * Products that correspond to existing fieldbus slaves and are connected to the EtherCAT master device.
# 1.3.5.1 EtherCAT Master Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Maximum Connectable Slave Count</td>
		<td>200</td>
	</tr>
    <tr>
		<td>Maximum Input Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Input Size (1 slave)</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size (1 slave)</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td>Min. 250us (1ms Recommended)</td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>100 Mbit/s (Full-duplex)</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Line, Ring</td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Redendance</td>
		<td>Supported (Cannot be applied simultaneously with synchronization)</td>
	</tr>
    <tr>
		<td>Synchronization</td>
		<td>DC (Distributed Clocks)</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>Forbidden</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>Only allowed between Master and 1st Slave</td>
	</tr>
</tbody>
</table>
<br>

##### Connection

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Cable</td>
		<td>Minimum of Cat5, STP</td>
	</tr>
	<tr>
		<td>length</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br># 1.3.5.2 EtherCAT Master Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[**1.3.2 SYCON.NET Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
\.      When using SYCON.net, if there are insufficient explanations in the manual, please refer to the "[**1.3.2 SYCON.NET Help**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" function.
{% endhint %}

<br>

##### 1. Select the EtherCAT master in the PCI slot settings and reboot the robot controller.

![[Figure 1.3.5.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.

<br>

{% hint style="info" %}
\.        For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.5.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the EtherCAT master PCI device by using Sycon.net.

![[Figure 1.3.5.2-3 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_3.png>)
![[Figure 1.3.5.2-4 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan the PCI device and apply the EtherCAT master.

![[Figure 1.3.5.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_5.png>) 

<br>

##### 5. Download the settings.

![[Figure 1.3.5.2-6 EtherCAT Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare the slave module to be connected to the EtherCAT master.
   * In this example, we use the M9386 EtherCAT slave from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.5.2-7 Crevis M9386]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_7.png>) 

<br>

##### 7. Slave device station address

{% hint style="info" %}
\.      The station address of the EtherCAT slave device is set by the master.
{% endhint %}

<br>

##### 8. Register the slave device XML file.

{% hint style="info" %}
\.      An XML file is required to use a device not registered in Sycon.net.

\.      The XML file for the M9386 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.5.2-8 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      Register the downloaded XML file in Sycon.net.

\.      When registering an XML File, please check the industrial communication Protocol (EtherCAT).
{% endhint %}

![[Figure 1.3.5.2-9 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_9.png>)

<br>

![[Figure 1.3.5.5-10 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.5.2-11 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_11.png>)

<br>

![[Figure 1.3.5.2-12 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_12.png>)


<br>

##### 9. Network Scan

{% hint style="warning" %}
\.      **For EtherCAT, the available cable connections and ports are specified.**

\.      **For smooth communication connection, be sure to check ("[**1.3.5.5 EtherCAT Cable Wiring**](../5-EtherCAT/5-EtherCAT-Topology.md)").**
{% endhint %}

{% hint style="info" %}
\.      The EtherCAT master supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the EtherCAT master device and click Network Scan.
{% endhint %}

![[Figure 1.3.5.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      If there is no XML file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

{% hint style="info" %}
\.      If an XML file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.5.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_14.png>)

<br>

##### 10. Configure the slave device.

{% hint style="info" %}
\.      Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.5.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 1.3.5.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      Add a slot connected to M9386 to set the EtherCAT slave.

\.      Slot 1 : M7001  
\.      Slot 2 : M12DF  
\.      Slot 3 : M225F  
{% endhint %}

![[Figure 1.3.5.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_17.png>)

![[Figure 1.3.5.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_18.png>)


<br>

##### 11. Configure the master device.

{% hint style="info" %}
\.      Double-click the Master device.
{% endhint %}

![[Figure 1.3.5.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      Synchronization: Select Freerun/DC (Distributed Clocks).

\.      Whether to use Redundancy (cannot be used together with Distributed Clocks)

\.      Bus Cycle Time: At least 250 us is supported. (1 ms or more is recommended.)
{% endhint %}

<br>

{% hint style="info" %}
\.      You can set the station address for each slave.
{% endhint %}

![[Figure 1.3.5.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.5.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_21.png>)


{% hint style="info" %}
\.      After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.5.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_22.png>)

<br>

##### 12. Check the communication status.

{% hint style="info" %}
\.        Check the communication status in Sycon.net and TP.

\.        For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
\.      Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.5.2-23 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_23.png>)

![[Figure 1.3.5.2-24 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.        Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.5.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_25.png>)

<br>

##### 13. Assign IO blocks after completing the settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}# 1.3.5.3 EtherCAT Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>Maximum Input Size</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td>Min. 250us (1ms Recommended)</td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>100 Mbit/s (Full-duplex)</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Line, Ring</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Synchronization</td>
		<td>DC (Distributed Clocks)</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>Forbidden</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>Only allowed between Master and 1st Slave</td>
	</tr>
</tbody>
</table>
<br>

##### Connection

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Cable</td>
		<td>Minimum of Cat5, STP</td>
	</tr>
	<tr>
		<td>length</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>
# 1.3.5.4 EtherCAT Slave Settings

The manual is in preparation.

<br>

{% hint style="info" %}
\.      **[EtherCAT Slave ESI File Download]**

\.      Please refer to "[**5. Slave Device Description File**](../../../5-slave-config-file.md)".
{% endhint %}
# 1.3.5.5 EtherCAT Cable Wiring (Topology)

<br>

Unlike existing industrial communications, EtherCAT has restrictions in cable wiring and usable Ethernet Ports.

##### 1. Ethernet Port

{% hint style="info" %}
\.      When connecting the EtherCAT master and slave, port 0 should be used.
{% endhint %}

![[Figure 1.3.5.5-1 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
\.      When one slave is connected to the master
{% endhint %}

![[Figure 1.3.5.5-2 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
\.      When two or more slaves are connected to the master

\.      Connect from the slave port 1 to the next slave port 0.
{% endhint %}

![[Figure 1.3.5.5-3 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_3.png>)

<br>

##### 2. Redundancy

{% hint style="info" %}
\.      When using the Redundancy function in the master 

\.      Connect port 1 of the last slave and port 1 of the master to form a ring structure.
{% endhint %}

![[Figure 1.3.5.5-4 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_4.png>) 


<br>

##### 3. Cable wiring error


Please refer to "[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

<br>

{% hint style="info" %}
\.      If the Network scan function is not working.

\.      Please check the port and cable connected to the master.
{% endhint %}

![[Figure 1.3.5.5-5 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
\.      Topology Error (Error in Configuration)

\.      Please check the cable wiring between the master and slave.
{% endhint %}

![[Figure 1.3.5.5-6 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
\.      Topology error 2 (normal during configuration but there is an error during diagnosis)

\.      Please check the cable wiring between the master and slave.

\.      Please check the cable wiring between slaves.
{% endhint %}

![[Figure 1.3.5.5-7 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_7.png>)

![[Figure 1.3.5.5-8 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
\.      Mandatory Slave Missing Error

\.      Please check the cable wiring between slaves.
{% endhint %}

![[Figure 1.3.5.5-9 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_9.png>)# 1.3.6 PROFIBUS-DP

This chapter describes the characteristics of the PROFIBUS-DP master and slave and how to set them. 

<br>

##### Fieldbus Overview

Fieldbus is an industry standard that has been opened for connecting devices such as sensors, buttons, motor drivers, and operation interfaces to PLCs (Programmable Logic Controllers) with a single cable and operating them in factories.

Fieldbus provides intelligent services such as central monitoring of the status of the entire network and reconfiguration of the network.

For example, it is possible to set detailed information, operations, and modes for sensors and switches, not just simple On/Off.

Using a single cable reduces time and costs for wiring, simplifies the configuration, and provides advantage in maintenance.

Also, unlike protocols with non-deterministic response characteristics of general communications, fieldbuses guarantee data response speed to satisfy industrial applications where critical time characteristics are important.

![[Figure 1.3.6-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/image_1.png>) 

<br>

One fieldbus network connects one master device and multiple slave devices.
The master device searches and manages the entire network and exchanges data with slave devices.

Generally, a PLC is a master device, while sensors, buttons, controllers, etc. can be configured as slave devices.# 1.3.6.1 PROFIBUS-DP Master Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Maximum Connectable Slave Count</td>
		<td>125</td>
	</tr>
    <tr>
		<td>Maximum Input Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Input Size (1 slave)</td>
		<td>244 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size (1 slave)</td>
		<td>244 bytes</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>9.6 ~ 12,000 Kbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Auto Baudrate Detection</td>
		<td>Not supported</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>PROFIBUS FDL</td>
	</tr>
</tbody>
</table>
<br># 1.3.6.2 PROFIBUS-DP Master Settings


Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[**1.3.2 SYCON.NET Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
\.      When using SYCON.net, if there are insufficient explanations in the manual, please refer to the ""[**1.3.2 SYCON.NET Help**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" function.
{% endhint %}

<br>

##### 1. Select the PROFIBUS-DP master in the PCI slot settings and reboot the robot controller.

![[Figure 1.3.6.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.

<br>

{% hint style="info" %}
\.        For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.6.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_2.png>)

<br>

##### 3. Select the PROFIBUS-DP master PCI device by using Sycon.net.

![[Figure 1.3.6.2-3 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[Figure 1.3.6.2-4 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan the PCI device and apply the PROFIBUS-DP master.

![[Figure 1.3.6.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>


##### 5. Download the settings.

![[Figure 1.3.6.2-6 PROFIBUS-DP Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare the slave module to be connected to the PROFIBUS-DP Master.
   * In this example, we use the GN-9222 PROFIBUS-DP slave from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.6.2-7 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_7.png>) 


<br>

##### 7. Set the slave device

{% hint style="info" %}
\.      Set the node number and termination of the PROFIBUS-DP slave device.
{% endhint %}

![[Figure 1.3.6.2-8 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_8.png>) 


{% hint style="info" %}
\.      Termination: To be set using the DIP switch (Example: Termination processing ON)

\.      Node ID (station number): To be set using the DIP switch (Example: Node 3)
{% endhint %}

<br>

##### 8. Register the slave device GSD file.

{% hint style="info" %}
\.      A GSD file is required to use a device not registered in Sycon.net.

\.      The GSD file for the GN-9222 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.6.2-9 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      Register the downloaded GSD file in Sycon.net.

\.      When registering a GSD file, please check the industrial communication protocol (PROFIBUS-DP).
{% endhint %}

![[Figure 1.3.6.2-10 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.6.5-11 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_11.png>)

![[Figure 1.3.6.5-12 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_12.png>)



<br>

##### 9. Network Scan

{% hint style="warning" %}
\.      **When performing the Network Scan function, be sure to check the following.**

\.      **(1) Whether a cable is connected.**  
\.      **(2) Whether a termination DIP switch is used.**  
{% endhint %}

{% hint style="info" %}
\.      PROFIBUS-DP master supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the PROFIBUS-DP master device and click Network Scan.
{% endhint %}

![[Figure 1.3.6.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      If there is no GSD file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

{% hint style="info" %}
\.      If a GSD file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.6.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

##### 10. Configure the slave device

{% hint style="info" %}
\.      Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.6.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 1.3.6.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      Check the PROFIBUS-DP slave settings.

\.      Slot 1 : GN-9222  
\.      Slot 2 : GT-12DF (Input 2 Byte)  
\.      Slot 3 : GT-227F (Output 2 Byte)  
\.      Slot 4 : GT-3154 (Input 8 Byte)  
\.      Slot 5 : GT-4254 (Output 8 Byte)  
{% endhint %}

![[Figure 1.3.6.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_17.png>)

<br>

![[Figure 1.3.6.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_18.png>)


<br>

##### 11. Configure the master device.

{% hint style="info" %}
\.      Double-click the Master device.
{% endhint %}

![[Figure 1.3.6.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_19.png>)


{% hint style="info" %}
\.      Set the PROFIBUS-DP communication speed.

\.      9.6 - 12000 Kbit/s 
{% endhint %}

![[Figure 1.3.6.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Check from the master device if the slot information of the slave device is correct.
{% endhint %}

![[Figure 1.3.6.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.6.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
\.      Check if each device in the station table is in active status.
{% endhint %}

![[Figure 1.3.6.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.6.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

##### 12. Check the communication status.

{% hint style="info" %}
\.        Check the communication status in Sycon.net and TP.

\.        For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
\.      Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.6.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[Figure 1.3.6.2-26 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Using Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.6.2-27 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_27.png>)

<br>

##### 13. Assign IO blocks after completing the settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}
# 1.3.6.3 PROFIBUS-DP Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>Maximum Input Size</td>
		<td>244 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>244 bytes</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>9.6 ~ 12,000 Kbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Auto Baudrate Detection</td>
		<td>Supported</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>PROFIBUS FDL</td>
	</tr>
</tbody>
</table>
<br>

# 1.3.6.4 PROFIBUS-DP Slave Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
\.      **[PROFIBUS-DP Slave GSD File Download]**

\.      Please refer to "[**5. Slave Device Description File**](../../../5-slave-config-file.md)".
{% endhint %}

<br>

##### 1. Using the TP, select a PROFIBUS-DP slave in the industrial communication firmware settings and reboot the robot controller.

![[Figure 1.3.6.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the current communication protocol readiness status in industrial communication monitoring menu.

![[Figure 1.3.6.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

##### 3. Touch the menu to enter the slave settings screen.
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > PROFIBUS-DP Slave]**

![[Figure 1.3.6.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.6.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of each item

{% hint style="info" %}
\.      [Station Address]

\.      The PROFIBUS-DP identifies a slave through the station address.
{% endhint %}

{% hint style="info" %}
\.      [Input Byte Count (Input Byte)]

\.      Input Byte Count: Sets the size of the data input from the master -> slave.
{% endhint %}

{% hint style="info" %}
\.      [Output Byte Count (Output Byte)]

\.      Output Byte Count: Sets the size of the data output from the slave -> master.
{% endhint %}

{% hint style="info" %}
\.      [**When Setting a Module from the Master**]

\.      Modules should be specified from the master to match the set byte count.

\.      Order: Master Input (64–1) -> Master Output (64–1)

\.      EX) Master Input 109 bytes  <---  Slave Output 109 bytes   
\.          Input 109 Bytes : 64Byte + 32Byte + 8Byte + 4Byte + 1 Byte

\.      EX) Master Output 120 bytes  --->  Slave Input 120 bytes   
\.          Output 120 Bytes : 64Byte + 32Byte + 16Byte + 8Byte


\.      EX) Master Input 12 bytes  <---  Slave Output 12 bytes   
\.          Input 12 Bytes : 8Byte + 4Byte

\.      EX) Master Output 200 bytes  --->  Slave Input 200 bytes   
\.          Output 200 Bytes : 64Byte + 64Byte + 64Byte + 8Byte

\.      The input module is located before the output module.
{% endhint %}

![[Figure 1.3.6.4-5 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>)


<br>

##### 5. After completing the settings, check the communication status according to the procedure below.

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.6.4-6 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>)

<br>

##### 6. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}# 1.3.6.5 PROFIBUS-DP Error Handling

<br>

Please refer to "[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".
# 1.3.7 DeviceNet

This chapter describes the characteristics of the DeviceNet master and slave and how to set them. 

<br>

##### Fieldbus Overview

Fieldbus is an industry standard that has been opened for connecting devices such as sensors, buttons, motor drivers, and operation interfaces to PLCs (Programmable Logic Controllers) with a single cable and operating them in factories.

Fieldbus provides intelligent services such as central monitoring of the entire network status and reconfiguration of the network.

For example, it is possible to set detailed information, operations, and modes for sensors and switches, not just simple On/Off.

Using a single cable reduces time and costs for wiring, simplifies the configuration, and provides advantage in maintenance.

Also, unlike protocols with non-deterministic response characteristics of general communications, fieldbuses guarantee data response speed to satisfy industrial applications where critical time characteristics are important.

![[Figure 1.3.7-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/image_1.png>)

<br>

One fieldbus network connects one master device and multiple slave devices.
The master device searches and manages the entire network and exchanges data with slave devices.

Generally, a PLC is a master device, while sensors, buttons, controllers, etc. can be configured as slave devices.# 1.3.7.1 DeviceNet Master Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Maximum Connectable Slave Count</td>
		<td>63</td>
	</tr>
    <tr>
		<td>Maximum Input Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Input Size (1 slave)</td>
		<td>255 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size (1 slave)</td>
		<td>255 bytes</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td>Bit Strobe <br>Change of State <br>Cyclic <br>Poll</td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>125 ~ 500 Kbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>Auto Baudrate Detection</td>
		<td>Not supported</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>CAN Frames</td>
	</tr>
</tbody>
</table>
<br># 1.3.7.2 DeviceNet Master Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[**1.3.2 SYCON.NET Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
\.      When using SYCON.net, if there are insufficient explanations in the manual, please refer to the ""[**1.3.2 SYCON.NET Help**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" function.
{% endhint %}

<br>

{% hint style="info" %}
\.      For DeviceNet connector connection, please refer to the following.

\.      ("[**1.2.2 Connector**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

##### 1. Select the DeviceNet master in the PCI slot settings and reboot the robot controller.

![[Figure 1.3.7.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_1.png>)

<br>

##### 2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.

<br>

{% hint style="info" %}
\.        For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.7.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the DeviceNet master PCI device by using Sycon.net.

![[Figure 1.3.7.2-3 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_3.png>)
![[Figure 1.3.7.2-4 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan the PCI device and apply the DeviceNet master.

![[Figure 1.3.7.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_5.png>) 

<br>

##### 5. Set the communication speed.

{% hint style="warning" %}
\.      If the communication speed differs between the master and the slave, the Network Scan function does not work normally.
{% endhint %}

![[Figure 1.3.7.2-6 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_6.png>) 

<br>

##### 6. Download the settings.

![[Figure 1.3.7.2-7 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_7.png>) 

<br>

##### 7. Prepare the slave module to be connected to the DeviceNet master.
   * In this example, we use the NA-9211 DeviceNet slave from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.7.2-8 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_8.png>) 

<br>

##### 8. Set the slave device.

{% hint style="info" %}
\.      Set the MAC ID, communication speed, and termination resistor of the DeviceNet slave device.
{% endhint %}

![[Figure 1.3.7.2-9 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_9.png>) 

![[Figure 1.3.7.2-10 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_10.png>)

{% hint style="info" %}
\.      [Example Settings]

\.      Termination resistor: Used by being installed in the cable (termination DIP switch OFF)

\.      MAC ID (station number): Set to 4 (Only DIP switch 3 is ON.)

\.      Communication speed (baudrate): Set to Auto (DIP switches 7 and 8 are ON.)
{% endhint %}

<br>

##### 9. Register the slave device EDS file.

{% hint style="info" %}
\.      An EDS file is required to use a device not registered in Sycon.net.

\.      The EDS file for NA-9211 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.7.2-11 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_11.png>)

{% hint style="info" %}
\.      Register all downloaded EDS files in Sycon.net.

\.      When registering an EDS file, please check the industrial communication protocol (DeviceNet).
{% endhint %}

![[Figure 1.3.7.2-12 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_12.png>)

<br>

![[Figure 1.3.7.5-13 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_13.png>)



<br>

##### 10. Network Scan

{% hint style="warning" %}
\.      **When performing the Network Scan function, be sure to check the following.**

\.      **(1) Whether a cable is connected.**  
\.      **(2) Whether a termination resistor is connected or a termination DIP switch is used.**  
\.      **(3) Whether the master - slave communication speed is set.**  

\.      **For smooth communication connection, be sure to check ("[**1.3.7.5 DeviceNet ERROR Handling**](../7-DeviceNet/5-Error-DeviceNet.md)").**
{% endhint %}

{% hint style="info" %}
\.      The DeviceNet master supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the DeviceNet master device and click Network Scan.
{% endhint %}

![[Figure 1.3.7.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      If there is no EDS file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

{% hint style="info" %}
\.      If an EDS file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.7.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_15.png>)

![[Figure 1.3.7.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_16.png>)

<br>

##### 11. Configure the slave device

{% hint style="info" %}
\.      Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.7.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 1.3.7.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_18.png>)


<br>

{% hint style="info" %}
\.      Set the connection type of the slave device.

\.      Select the message transmission method for DeviceNet communication connection.

\.      ** If the UCMM checkbox is not checked, UCMM group 2 is set as the default value.**   

\.      UCMM GROUP 1 : IO Message   
\.      UCMM GROUP 2: Master - Slave connection message during network initialization (default setting)   
\.      UCMM GROUP 3: Explicit Message   

\.      For certain devices, UCMM group 3 may be used, so please check the product specifications before proceeding.
{% endhint %}

![[Figure 1.3.7.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_19.png>)

<br>

{% hint style="info" %}
\.      For Crevis NA-9211, proceed without checking the UCMM check box. (Use the group 2 default value.)
{% endhint %}

![[Figure 1.3.7.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_20.png>)

<br>


{% hint style="info" %}
\.      Check the DeviceNet slave settings.

\.      Output: ST-2318 (1 byte)  
\.      Input: ST-1218 (1 byte)  
{% endhint %}

<br>

{% hint style="info" %}
\.      Required to set according to the communication method (Poll, Change of State, Cyclic, Bit-Strobe).
{% endhint %}

<br>

![[Figure 1.3.7.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_21.png>)

<br>

{% hint style="info" %}
\.      [Production Inhibit Time]

\.      Set the IO data generation cycle of the slave device (ms)  
\.  
\.      Example) 10 ms: IO data is generated every 10 ms.  
\.      Example) 0 ms: The slave generates IO data as quickly as possible.  

\.      The shorter the cycle, the greater the load on the slave device may be. (Specifications need to be checked for each slave.) 
{% endhint %}

<br>

{% hint style="info" %}
\.      [Expected Packet Rate]

\.      Set the time for IO data update between the master and the slave.  
{% endhint %}

<br>

![[Figure 1.3.7.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_22.png>)



<br>

##### 12. Configure the master device

{% hint style="info" %}
\.      Double-click the Master device.
{% endhint %}

![[Figure 1.3.7.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      Set the DeviceNet communication speed (to be the same as the slave communication speed).
{% endhint %}

![[Figure 1.3.7.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.7.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      Set whether to use the Quick Connect function.
{% endhint %}

![[Figure 1.3.7.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_26.png>)


{% hint style="info" %}
\.      After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.7.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_27.png>)

<br>

##### 13. Check the communication status.

{% hint style="info" %}
\.        Check the communication status in Sycon.net and TP.

\.        For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
\.      Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.7.2-28 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_28.png>)

![[Figure 1.3.7.2-29 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.        Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.7.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_30.png>)

<br>

##### 14. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}# 1.3.7.3 DeviceNet Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>Maximum Input Size</td>
		<td>255 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>255 bytes</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td>Bit Strobe <br>Change of State <br>Cyclic <br>Poll</td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>125 ~ 500 Kbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Auto Baudrate Detection</td>
		<td>Not supported</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>CAN Frames</td>
	</tr>
</tbody>
</table>
<br>

# 1.3.7.4 DeviceNet Slave Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
\.      **[DeviceNet Slave EDS File Download]**

\.      Please refer to "[**5. Slave Device Description File**](../../../5-slave-config-file.md)."
{% endhint %}

<br>

{% hint style="info" %}
\.      For DeviceNet connector connection, please refer to the following.

\.      ("[**1.2.2 Connector**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

##### 1. Using the TP, select a DeviceNet slave in the industrial communication firmware settings and reboot the robot controller.

![[Figure 1.3.7.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the current communication protocol readiness status in industrial communication monitoring menu.

![[Figure 1.3.7.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

##### 3. Touch the menu to enter the slave settings screen.
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > DeviceNet Slave]**

![[Figure 1.3.7.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_3.png>) 

![[Figure 1.3.7.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of each item

{% hint style="info" %}
\.      [Station Address = Mac ID]

\.      The DeviceNet identifies a slave through the station address (MAC ID) (1–63).
{% endhint %}

{% hint style="info" %}
\.      [Communication Speed (Baudrate)]

\.      You can select among 125, 250, and 500 Kbit/s.
{% endhint %}

{% hint style="info" %}
\.      [Input Byte Count (Input Byte)]

\.      Input Byte Count: Sets the size of the data input from the master -> slave.
{% endhint %}

{% hint style="info" %}
\.      [Output Byte Count (Output Byte)]

\.      Output Byte Count: Sets the size of the data output from the slave -> master.
{% endhint %}


<br>

##### 5. After completing the settings, check the communication status according to the procedure below.

For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.7.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_5.png>) 

<br>

##### 6. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}# 1.3.7.5 DeviceNet Error Handling

<br>

Please refer to "[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

<br>

##### 1. DeviceNet termination resistor

{% hint style="info" %}
\.      A resistor should be added at the termination when connecting the DeviceNet cable.

\.      If the Network Scan function does not work, please check the termination resistor.

\.      DeviceNet termination resistor: 120 ohms
{% endhint %}

{% hint style="info" %}
\.      As shown in the figure below, if the CIFX-50 DN PCI is at the DeviceNet termination, please add a termination resistor.
{% endhint %}

![[Figure 1.3.7.5-1 DeviceNet Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_1.png>) 

{% hint style="info" %}
\.      As shown in the figure below, if the DeviceNet Remote IO is at the termination, please add a termination resistor or operate the DIP switch.
{% endhint %}

![[Figure 1.3.7.5-2 DeviceNet Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_2.png>) 

<br>

##### 2. Communication Speed

{% hint style="info" %}
\.      If the communication speed differs between the DeviceNet master and slave, the Network Scan function may not work.

\.      If the Network Scan function does not work, please check the communication speed.
{% endhint %}

![[Figure 1.3.7.5-3 DeviceNet Baudrate]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_3.png>) 

<br>

##### 3. DeviceNet ERROR

{% hint style="info" %}
\.      If a 24V power is not supplied to the DeviceNet cable, the following error will appear.

\.      Please check the 24V power supply.
{% endhint %}

![[Figure 1.3.7.5-4 DeviceNet Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_4.png>) # 1.3.7.6 DeviceNet Object


<br>

##### 1. Object


The inside of the DeviceNet device is composed of a collection of objects. Each object represents a specific component inside the device.

<br>

![[Figure 1.3.7.6-1 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_1.png>) 


<br>

Individual objects are distinguished using a class code.

<br>

![[Figure 1.3.7.6-2 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_2.png>)

<br>

The inside of an object is composed of an instance number and attribute ID.

<br>

The DeviceNet master can access an object of a specific slave through a explicit message.

<br>

{% hint style="info" %}
\.      EX) Object of Crevis GN-9212 (The corresponding information can be found in the Crevis manual.)

\.      Reading the vendor ID value of the identity object (class code 0x01)

\.      Instance : 1

\.      Attribute ID : 1

\.      Permission: Get (Read only possible)
{% endhint %}


![[Figure 1.3.7.6-3 DeviceNet Object Crevis GN-9212]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_3.png>)


<br>

Each Object, Instance, and Attribute inside has different access permissions.

<br>

{% hint style="info" %}
\.      Access permissions

\.      Get: Read permission

\.      Set: Write permission 

\.      Attribute Single: Can access only one attribute item at a time.

\.      Attribute All: Can access all attributes in Instance at once.
{% endhint %}

<br># 1.3.8 CC-Link

This chapter describes the characteristics of CC-Link slaves and how to set them. 


<br>

##### Fieldbus Overview

Fieldbus is an industry standard that has been opened for connecting devices such as sensors, buttons, motor drivers, and operation interfaces to PLCs (Programmable Logic Controllers) with a single cable and operating them in factories.

Fieldbus provides intelligent services such as central monitoring of the status of the entire network and reconfiguration of the network.

For example, it is possible to set detailed information, operations, and modes for sensors and switches, not just simple On/Off.

Using a single cable reduces time and costs for wiring, simplifies the configuration, and provides advantage in maintenance.

Also, unlike protocols with non-deterministic response characteristics of general communications, fieldbuses guarantee data response speed to satisfy industrial applications where critical time characteristics are important.

![[Figure 1.3.8-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/image_1.png>)

<br>

One fieldbus network connects one master device and multiple slave devices.
The master device searches and manages the entire network and exchanges data with slave devices.

Generally, a PLC is a master device, while sensors, buttons, controllers, etc. can be configured as slave devices.# 1.3.8.1 CC-Link Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=3, class='powderblued'>Category</th>
		<th class='powderblued'>Specifications (Version 1.11)</th>
		<th class='powderblued'>Specifications (Version 2.0)</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td colspan=3>Maximum Input Size</td>
		<td>48 bytes</td>
		<td>368 bytes</td>
	</tr>
    <tr>
		<td colspan=3>Maximum Output Size</td>
		<td>48 bytes</td>
		<td>368 bytes</td>
	</tr>
    <tr>
		<td rowspan=6>IO Size</td>
		<td rowspan=2>IO Station</td>
        <td>RY</td>
		<td>4 bytes</td>
		<td>Not supported</td>
	</tr>
    <tr>
        <td>RX</td>
		<td>4 bytes</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td rowspan=4>Remote Device</td>
        <td>RY</td>
		<td>16 bytes</td>
		<td>112 Bytes</td>
	</tr>
    <tr>
        <td>RX</td>
		<td>16 bytes</td>
		<td>112 Bytes</td>
	</tr>
    <tr>
        <td>RWw</td>
		<td>32 bytes</td>
		<td>256 Bytes</td>
	</tr>
    <tr>
        <td>RWr</td>
		<td>32 bytes</td>
		<td>256 Bytes</td>
	</tr>
    <tr>
        <td colspan=2, rowspan=2>Occupied Station</td>
        <td>IO Station</td>
		<td>1</td>
		<td> - </td>
	</tr>
    <tr>
        <td>Remote Device</td>
		<td>1 ~ 4</td>
		<td>1 ~ 4</td>
	</tr>
    <tr>
        <td colspan=3>Extension Cycle</td>
		<td>Not supported</td>
		<td>1, 2, 4, 8</td>
	</tr>
   <tr>
		<td colspan=3>Communication Speed</td>
		<td colspan=2>156 kbit/s ~ 10 Mbit/s</td>
	</tr>
</tbody>
</table>
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

\.        Extension Cycle: Quadruple
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

<br># 1.3.8.2 CC-Link Slave Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
\.      For CC-Link connector connection, please refer to the following.

\.      ("[**1.2.2 Connector**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

##### 1. Using the TP, select CC-Link slave in the industrial communication firmware settings and reboot the robot controller.

![[Figure 1.3.8.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the current communication protocol readiness status in industrial communication monitoring menu.

![[Figure 1.3.8.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

##### 3. Touch the menu to enter the slave settings screen.
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > CC-Link Slave]**

![[Figure 1.3.8.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>) 

![[Figure 1.3.8.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of each item

{% hint style="info" %}
\.      [Station Address]

\.      The CC-Link identifies the slave through the Station Address (1–64).
{% endhint %}

{% hint style="info" %}
\.      [Communication Speed (Baudrate)]

\.      You can select from 156, 625, 2500, 5000, and 10000 Kbit/s.
{% endhint %}

{% hint style="info" %}
\.      [CC-Link Version]

\.      Version 1: IO Station available, Extension Cycle not available

\.      Version 2: IO Station not available, Extension Cycle available
{% endhint %}

{% hint style="info" %}
\.      [Occupied Station Count]

\.      IO Station: Occupies 1

\.      Remote Device: 1–4 selectable

\.      The size of the assigned IO byte area varies depending on the number of stations occupied.
{% endhint %}

{% hint style="info" %}
\.      [Extension Cycle]

\.      Available in Version 2

\.      Remote Device: You can select from Single (1x), Double (2x), Quadruple (4x), and Octuple (8x).

\.      The size of the assigned IO byte area varies depending on the Extension Cycle.
{% endhint %}

<br>

{% hint style="info" %}
\.      **For the IO Byte area, please refer to the link below.**

\.      **(["**1.3.8.1 CC-Link Slave Specifications**](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md))**
{% endhint %}

<br>

##### 5. After completing the settings, check the communication status according to the procedure below.

For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

<br>

##### 6. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}# 1.3.8.3 CC-Link Slave Error Handling

<br>

Please refer to "[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

<br>

##### 1. CC-Link termination resistor

{% hint style="info" %}
\.      A resistor should be added at the termination when connecting the CC-Link cable.

\.      If communication is not connected, please check the termination resistor.

\.      CC-Link termination resistor: 110 ohms
{% endhint %}

{% hint style="info" %}
\.      As shown in the figure below, if the CIFX-50 CC PCI is at the CC-Link termination, please add a termination resistor.
{% endhint %}

![[Figure 1.3.8.5-1 CC-Link Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/5-Error/image_1.png>) 



##### 2. CC-Link ERROR

{% hint style="info" %}
\.      A 24V power supply to the CC-Link cable is required for communication connection.

\.      If communication is not connected, please check the 24V power supply.
{% endhint %}
# 1.3.9 CC-Link IE Field

This chapter describes the characteristics of CC-Link IE field slaves and how to set them. 


<br>

##### Fieldbus Overview

Fieldbus is an industry standard that has been opened for connecting devices such as sensors, buttons, motor drivers, and operation interfaces to PLCs (Programmable Logic Controllers) with a single cable and operating them in factories.

Fieldbus provides intelligent services such as central monitoring of the status of the entire network or reconfiguration of the network.

For example, it is possible to set detailed information, operations, and modes for sensors and switches, not just simple On/Off.

Using a single cable reduces time and costs for wiring, simplifies the configuration, and provides advantage in maintenance.

Also, unlike protocols with non-deterministic response characteristics of general communications, fieldbuses guarantee data response speed to satisfy industrial applications where critical time characteristics are important.

![[Figure 1.3.9-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/image_1.png>)

<br>

One fieldbus network connects one master device and multiple slave devices.
The master device searches and manages the entire network and exchanges data with slave devices.

Generally, a PLC is a master device, while sensors, buttons, controllers, etc. can be configured as slave devices.
# 1.3.9.1 CC-Link IE Field Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=2, class='powderblued'>Category</th>
		<th colspan=2, class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td colspan=2>Network Number</td>
		<td colspan=2>1-239</td>
	</tr>
    <tr>
		<td colspan=2>Station Number</td>
		<td colspan=2>1-120</td>
	</tr>
    <tr>
		<td colspan=2>Communication Speed</td>
		<td colspan=2>1Gbps</td>
	</tr>
    <tr>
		<td colspan=2>Device Type</td>
		<td>Intelligent Device Station</td>
        <td>Remote Device Station</td>
	</tr>
    <tr>
		<td rowspan=4>IO Size</td>
        <td>RY data</td>
		<td>4-256 bytes (32-2048 bits)</td>
        <td>4-16 bytes (32-128 bits)</td>
	</tr>
    <tr>
        <td>RX data</td>
		<td>0 - 256 bytes (0 - 2048 bits)</td>
        <td>0 - 16 bytes (0 - 128 bits)</td>
	</tr>
    <tr>
        <td>RWw data</td>
		<td>0 - 1024 words</td>
        <td>0 - 64 words</td>
	</tr>
    <tr>
        <td>RWr data</td>
		<td>0-1024 words</td>
        <td>0-64 words</td>
	</tr>
</tbody>
</table>
<br>

##### Network Characteristics

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>1000 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>Constantly On</td>
	</tr>
    <tr>
		<td>Auto-Crossover</td>
		<td>Constantly On</td>
	</tr>
</tbody>
</table>
<br>

##### Connection

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Cable</td>
		<td>Minimum of Cat6, STP</td>
	</tr>
	<tr>
		<td>length</td>
		<td>Max. 100m</td>
	</tr>
	<tr>
		<td>Wiring</td>
		<td>Fully occupied cable (all 8 cable cores)</td>
	</tr>
</tbody>
</table>
<br># 1.3.9.2 CC-Link IE Field Slave Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.


<br>

##### 1. Using the TP, select a CC-Link IE Field slave in the industrial communication firmware settings and reboot the robot controller.

![[Figure 1.3.9.2-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the current communication protocol readiness status in industrial communication monitoring menu.

![[Figure 1.3.9.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

##### 3. Touch the menu to enter the slave settings screen.
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > CC-Link IE Field Slave]**

![[Figure 1.3.9.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>) 

![[Figure 1.3.9.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of each item

{% hint style="info" %}
\.      [Network Number]

\.      CC-Link IE field network number (1–239)
{% endhint %}

{% hint style="info" %}
\.      [Station Address]

\.      Device ID within the connected network (1–120)
{% endhint %}

{% hint style="info" %}
\.      [IO Type]

\.      IO type is determined by the master device settings.   
\.      - Mixed: Input and output use different indexes (different addresses).   
\.      - Input: Input only   
\.      - Output: Output only   
\.      - FrontBackMixture: Input and output use the same index (same address).   
{% endhint %}

{% hint style="info" %}
\.      [Device Type]

\.      The maximum IO size that can be set varies depending on the Device Type.

\.      Intelligent Device Station   
\.      - RY, RX (max): 256 bytes   
\.      - RWw, RWr (max): 1024 words

\.      Remote Device Station   
\.      - RY, RX (max): 16 bytes   
\.      - RWw, RWr (max): 64 words
{% endhint %}

{% hint style="info" %}
\.      [IO Size]

\.      Master -> Slave
\.      - RWw (word data)
\.      - RY (bit data)

\.      Slave -> Master   
\.      - RWr (word data)   
\.      - RX (bit data)  
{% endhint %}

<br>

##### 5. After completing the settings, check the communication status according to the procedure below.

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

<br>

##### 6. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}

<br>

![[Figure 1.3.9.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>) # 1.3.9.3 CC-Link IE Field Slave Error Handling

<br>

Please refer to "[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".
# 1.3.10 EtherNet/IP - Standard Remote IO Connection

<br>

This chapter explains how to connect several standard Remote IO modules selected by our company using the EtherNet/IP scanner (master).

<br>

{% hint style="info" %}
\.      The EtherNet/IP scanner (master) uses the CIFX-50 real time Ethernet PCI.


\.      Remote IO module uses the M9289 EtherNet/IP network adapter from Crevis.
{% endhint %}

# 1.3.10.1 EtherNet/IP - Standard Remote IO Connection Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

##### 1. Select EtherNet/IP Master in the industrial communication firmware settings and reboot the robot controller.

![[Figure 1.3.10.1-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>) 

<br>

##### 2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.

![[Figure 1.3.10.1-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

##### 3. Connect the PCI and Remote IO cables, etc. for communication and check the status.

![[Figure 1.3.10.1-3 Hardware Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[Figure 1.3.10.1-4 Hardware Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

<br>

{% hint style="info" %}
\.      Please connect the PCI and Remote IO using a LAN cable.

\.      Set all DIP switches of the Remote IO to OFF.

\.      Connect both the Remote IO power and Field Power (24 V DC).
{% endhint %}

<br>

{% hint style="info" %}
\.      The factory default IP of the Crevis M9289 Remote IO is 192.168.100.99.

\.      The Remote IO IP should be set to 192.168.100.99 to enable communication connection.

\.      "[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

##### 4. Touch the menu to enter the slave settings screen.
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > EtherNet/IP Remote IO Setting]**

![[Figure 1.3.10.1-5 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>)

![[Figure 1.3.10.1-6 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>)

<br>

{% hint style="info" %}
\.      The IP is set as a fixed value.

\.      Check the input and output byte counts.

\.      The selected input and output byte counts should be less than or equal to the IO byte counts of the card installed in the Remote IO slot.
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
\.      M5112 : Conveyer I/F
{% endhint %}

<br>

##### 5. Reboot the controller after completing the settings.

![[Figure 1.3.10.1-7 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>)

![[Figure 1.3.10.1-8 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
\.      Please reboot the controller after completing the settings.
{% endhint %}

<br>

##### 6. After confirming that the setting values are reflected, check the communication status.

![[Figure 1.3.10.1-9 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>)

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.10.1-10 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>)

{% hint style="info" %}
\.      If communication is not connected, you should check the Remote IO IP.

\.      Please follow the steps below. (If not 192.168.100.99)

\.      "[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

![[Figure 1.3.10.1-11 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>) 

![[Figure 1.3.10.1-12 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>)

<br>

##### 7. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}# 1.3.10.2 Remote IO IP Address Settings

This is how to set the IP address of the M9289 EtherNet/IP network adapter from Crevis.

<br>

{% hint style="info" %}
\.      The factory default IP of the Crevis M9289 Remote IO is 192.168.100.99.

\.      If you do not know the Remote IO IP or need to change it, please follow the steps below.
{% endhint %}

<br>

##### 1. Connect the PC and Remote IO directly using a LAN cable.

![[Figure 1.3.10.2-1 LAN Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

##### 2. Change only DIP switch 9 of the Remote IO Adapter to ON.

![[Figure 1.3.10.2-2 DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

##### 3. Execute the Bootpsvr.exe program.
   * This program is provided by Crevis. (Download and install IO Guide Pro from the website.)

![[Figure 1.3.10.2-3 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[Figure 1.3.10.2-4 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
\.      With Start BootP being pressed, disconnect and reapply power to the M9289 module to reboot it.
{% endhint %}

![[Figure 1.3.10.2-5 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>


##### 4. When the adapter device is rebooted, the device information will appear in the BootpSvr.exe program.

![[Figure 1.3.10.2-6 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

##### 5. Select the device and set the IP.

![[Figure 1.3.10.2-7 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[Figure 1.3.10.2-8 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

##### 6. After completing the IP setting, turn all DIP switches of the adapter to OFF and reboot the device.

{% hint style="info" %}
\.      Be sure to check the DIP switch status and whether the adapter is rebooted.
{% endhint %}

![[Figure 1.3.10.2-9 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

##### 7. Use the ping test, etc. on the PC to verify the IP.

![[Figure 1.3.10.2-10 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

##### 8. If the IP address has been changed successfully, proceed with settings.

{% hint style="info" %}
\.      Please proceed with the settings according to the "[**1.3.10.1 EtherNet/IP - Standard Remote IO Connection Settings**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)" procedure.
{% endhint %}
# 1.4 CIFX PCI Communication Monitoring

<br>

After setting the communication according to the procedures of “[**1.2 CIFX PCI - Installing and Setting Industrial Communication Cards**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)” and “[**1.3 CIFX PCI - Setting Industrial Communication**](../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md),” you can check the operations in the following screens.

<br>

#### 1. Industrial Communication Monitoring

<br>

You can enter the screens by touching **\[Service > 19: Industrial Communication Monitoring]**, and check the details such as the set firmware information, communication status, and communication configuration in relevant screens.

<br>

{% hint style="info" %}
\.      Using the **\[Restart]** button, you can restart the industrial communication of the PCI communication card.

\.      Please check the status of the slot, firmware, and device.

\.      For the master, check whether the number of the configured and active slaves matches the number of configured slaves.
{% endhint %}

<br>

![[Figure 1.4-1 Industrial Communication Monitoring]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_1.png>)

<br>

{% hint style="info" %}
\.      [Status Information]   
\.       Communication: Communication link established and I/O data exchanging   
\.       Run: Communication card (PCI) is operating   
\.       Ready: Communication is in standby state   
\.       Error: Communication error state   

\.       Communication Error: Error code occurred during communication   
\.       Error Count: Accumulated number of communication errors   
\.       Active Slaves: Number of slaves currently connected and exchanging I/O data   
\.       Configured Slaves: Number of slaves configured for communication   
\.       Diag Slave: Number of slaves under communication diagnostics   
\.       Watchdog Time (ms): Timeout value for monitoring communication program activity   
{% endhint %}

<br>

#### 2. Industrial Communication Node Monitoring

<br> 

#### Supported version: TBD 

<br>

Click the Node Statue button at the bottom of the monitoring screen to monitor the status of devices connected to the master protocol

<br>

![[그림 1.4-2 Industrial Communication Monitoring]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_2.png>)

{% hint style="info" %}
\.      [Node Status Information]   
\.       Green: Node currently connected and exchanging I/O data   
\.       Red: Node configured but not connected   
{% endhint %}

<br>

{% hint style="info" %}
\.      In the case of DeviceNet Master, you can monitor by scanning the node information list
{% endhint %}

<br>

![[그림 1.4-3 Industrial Communication Monitoring]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_3.png>)# 1.4.1 ERROR Code

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
		<td>Normal</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xC000000C</td>
		<td>Watchdog timeout between controller and PCI</td>
		<td>Please check the status of the controller and device. They can be reset by restarting communication.</td>
	</tr>
    <tr>
		<td>0xC0000123</td>
		<td>No license</td>
		<td>Please check if you have a license for master. </td>
	</tr>
    <tr>
		<td>0xC0000140</td>
		<td>Communication error</td>
		<td>Please check the status or connection of the device.</td>
	</tr>
    <tr>
		<td>0xC0000141</td>
		<td>Connection lost</td>
		<td>Please check the status or connection of the device.</td>
	</tr>
    <tr>
		<td>0xC0000142</td>
		<td>Connection waiting timeout</td>
		<td>Please check the status or connection of the device.</td>
	</tr>
    <tr>
		<td>0xC0000144</td>
		<td>Duplicate IP address</td>
		<td>Check the IP addresses of connected devices and change the duplicate addresses.</td>
	</tr>
    <tr>
		<td>0xC0000145</td>
		<td>Cable not connected</td>
		<td>Please check the connection status of the communication cable.</td>
	</tr>
    <tr>
		<td>0xC0000180</td>
		<td>Communication bus off flag set <br> [Possible causes] <br> - CAN High/Low communication line short circuit detected <br> - Unstable power supply voltage <br> - Continuous network errors due to noise, etc.</td>
		<td>Check the contact status or wiring of the communication cable, and reset the device.</td>
	</tr>
    <tr>
		<td>0xC0470298</td>
		<td>DeviceNet 24V not supplied</td>
		<td>Please check the DeviceNet 24V power supply.</td>
	</tr>
	<tr>
		<td>0xC0620023</td>
		<td>DeviceNet slave bus off detected <br> [Possible causes] <br>  - CAN High/Low communication line short circuit detected <br>  - Unstable power supply voltage <br>  - Continuous network errors due to noise, etc.</td>
		<td>Check the contact status or wiring of the communication cable, and reset the device. </td>
	</tr>
    <tr>
		<td>0xC062002C</td>
		<td>DeviceNet slave 24V not supplied</td>
		<td>Please check the DeviceNet 24V power supply.</td>
	</tr>
</tbody>
</table>

# 2. EtherNet/IP Adapter

Description of the built-in EtherNet/IP adapter.<br>

### Terminology
|Abbreviation|Description|
|---------------|------------------------------|
|Adapter|Device that collects output data from the EtherNet/IP scanner and transmits the input data|
|Scanner|Device that sends output data to terminal devices (EtherNet/IP adapters) and collects input data from them|
|LAN| Local Area Network|
|RPI|Requested Packet Interval (Communication Cycle)|
|PLC|Programmable logic controller|
|T2O|Target to Originator (Adapter -> Scanner)|
|O2T|Originator to Target (Scanner -> Adapter)|
## 2.1 EtherNet/IP Adapter

### 2.1.1 Introduction
The Robot controller provides various types of industrial communication functions. Among them, the EtherNet/IP adapter is a function that does not require additional hardware. To use this function, a separate software license should be purchased. For license purchase, please contact the HD Hyundai Robotics Parts Business Team. <br>

### 2.1.2 Product Specifications
|Item|Description|
|------|---|
|Netowork Type|EtherNet/IP|
|Speed|10/100 Mbps, 1Gbps|
|Input Size Range(bytes)|0 - 240|
|Output Size Range(bytes)|0 - 240|
|Transport Class|Class 1 I/O implicit|## 2.2 EtherNet/IP Adapter Network Settings

### 2.2.1 Main Module
The LAN ports that can connect with the EtherNet/IP adapter are LAN1/LAN2/LAN3.<br>

![MainModule.png](../_assets/2-EtherNet-IP-Adapter/Network/hi6com.png)<br>
*[Figure 2.2.1 Main Module]*<br>

### 2.2.2 Network Settings
Select a LAN port to connect EtherNet/IP communication and then check the settings of the LAN port through the TP screen as shown below and change the settings as needed.<br>

![networkConfig.png](../_assets/2-EtherNet-IP-Adapter/Network/networkConfig.png)<br>
*[Figure 2.2.2 Network Settings]*<br>

{% hint style="info" %}
\.      The subnet portion of each IP address of LAN1/LAN2/LAN3 should be set differently.

\.      After changing the settings, reboot the robot controller.
{% endhint %}

### 2.2.3 Connection Status Check
The status of the physical connection with the EtherNet/IP scanner can be checked according to the status of the Link/Act LED of the LAN port.<br>

![lanPort.png](../_assets/2-EtherNet-IP-Adapter/Network/lanPort.png)<br>
*[Figure 2.2.3 LAN Port]*<br>

Connect the EtherNet/IP adapter and scanner with a LAN cable and then check the LED status. If the LED on the left does not light up or blink, it means there is a problem with the cable or adapter or scanner device. Please check the connection status of the cable or device.<br>

### 2.2.4 Network Configuration
It is recommended to configure the EtherNet/IP Network and Factory Network as separate networks. As shown in the figure below, if you configure the EtherNet/IP Network and Factory Network as one network, they will share one transmission medium, increasing the network load. Therefore, it is recommended to use a separately configured network for the EtherNet/IP Network if possible.<br>

![NG_Network.png](../_assets/2-EtherNet-IP-Adapter/Network/NG_Network.png)<br>
*[Figure 2.2.4 Non-separated Network]*<br>

![Good_Network.png](../_assets/2-EtherNet-IP-Adapter/Network/Good_Network.png)<br>
*[Figure 2.2.5 Separated Network]*<br>
## 2.3 EtherNet/IP Adapter

### 2.3.1 EtherNet/IP Adapter Specifications
|Item|Description|
|------|---|
|Device Type|General Purpose Discrete I/O (7)|
|Input Assembly Instance|100|
|Output Assembly Instance|112|
|Input Size Range(bytes)|0 - 240|
|Output Size Range(bytes)|0 - 240|
|RPI Range (ms)|5 – 3000|<br>

### 2.3.2 EtherNet/IP Adapter Settings and Monitoring via Teaching Pendant
On the initial screen, navigate to "SYSTEM" > "Control Parameter" > "Industrial Communication" > "Ethernet/IP Adapter"<br>
![Config.PNG](../_assets/2-EtherNet-IP-Adapter/Spec/Config.PNG)<br>
*[Figure 2.3.1 Settings]*<br>

**[Network]**
-	Function Use: Select whether to use the Ethernet/IP adapter.
-	Ethernet Port Selection: Select the LAN port to be connected to the Ethernet/IP scanner. (The information of the selected LAN port is displayed on the line immediately below.)<br>

**[I/O Size]**
-	Input Byte Count: 0–240 can be set.
-	Output Byte Count: 0–240 can be set.<br>

**[Monitoring]**
- Run: Indicates the I/O data exchange status of Ethernet/IP (On: Normal communication. Off: No communication).
- Ready: Indicates the initialization status of the Ethernet/IP adapter (On: Initialization normal. Off: Initialization abnormal).
- Error: Displays the alarm or warning status of the Ethernet/IP adapter (On: Alarm/warning status. Off: Normal).
- Version: Displays the Ethernet/IP adapter S/W version information.
- Error Code: Displays the alarm or warning code when an alarm or warning occurs.
## 2.4 EtherNet/IP Adapter Alarm Codes

|Code|Message|
|------|---|
|W23101|EtherNet/IP initialization failed|
|W23102|EtherNet/IP communication timeout occurred|
|W23103|EIP adapter CPF O2T initialization failed|
|W23104|EIP adapter CPF T2O initialization failed|
|W23105|EIP adapter IO MSG O2T initialization failed|
|W23106|EIP adapter IO MSG T2O initialization failed|
|W23107|EIP adapter PIT initialization failed|
|W23108|EIP adapter socket communication initialization failed|
|W23109|EIP adapter socket communication (UDP 0) initialization failed|
|W23110|EIP adapter socket communication (UDP 1) initialization failed|
|W23111|EIP adapter socket communication (UDP 2) initialization failed|
|W23112|EIP adapter socket communication (UDP 3) initialization failed|
|W23113|EIP adapter socket communication (TCP 0) initialization failed|
|W23114|EIP adapter socket communication (TCP 1) initialization failed|
|W23115|EIP adapter socket communication (TCP 2) initialization failed|
|W23116|EIP adapter socket communication (TCP 3) initialization failed|
|W23117|EIP adapter internal communication1 (IO Write) problem|
|W23118|EIP adapter internal communication1 (IO Read) problem|
|W23119|EIP adapter internal communication1 (Status Write) problem|
|W23120|EIP adapter internal communication1 (Config Read) problem|
|W23150|EIP adapter internal communication2 (IO Read) problem|
|W23151|EIP adapter internal communication2 (IO Write) problem|
|W23152|EIP adapter internal communication2 (Status Read) problem|
|W23153|EIP adapter internal communication2 (Config Write) problem|



## 2.5 EtherNet/IP Adapter License
### 2.5.1 License Activation
On the initial screen, navigate to "System" > "2: Control Parameters" > "10: License Key Registration for Optional Functions"<br>
![license.png](../_assets/2-EtherNet-IP-Adapter/License/license.png)<br>
*[Figure 2.5.1-1 License Activation]*<br>

1. Select "Valid" for the EtherNet/IP adapter from the license list.
2. Deliver the system serial number to the license administrator
3. Obtain the license key from the administrator, enter it, and press the "Confirm" button
4. License Key [XXXXXX] ==>OK Confirm
5. Confirm that the warning message about no license has disappeared when entering the Ethernet/IP adapter menu.<br>
~ Reference<br>
![license_ng.png](../_assets/2-EtherNet-IP-Adapter/License/license_ng.png)<br>
*[Figure 2.5.1-2 Message displayed when there is no license activated]*<br>


## 2.6 Connecting with EtherNet/IP Scanner

This chapter explains how to connect the EtherNet/IP scanner with the EtherNet/IP adapter. <br>### 2.6.1 Connection with LS ELECTRIC PLC

This section explains how to connect the LS ELECTRIC PLC with EtherNet/IP.  
The PLC and communication module used below are as follows.  
(PLC: XGI-CPUS, Communication Module: XGL-EFMTB)

#### 2.6.1.1 XG5000 Running
![xg5000.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/xg5000.png) <br>
*[Figure 2.6.1.1 XG5000 Running]*<br>
For downloading the XG5000 program and detailed usage methods, please refer to the LS ELECTRIC website.

#### 2.6.1.2 EDS File Registration
Click Menu > Tools > EDS(D) > EDS File Registration, and then select "Hi6_EIP_240402.eds."<br>
Confirm EDS file registration as shown in the figure below.<br>
![eds.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/eds.png)<br>
*[Figure 2.6.1.2 EDS File Registration]*<br>


#### 2.6.1.3 Device Connection
[1] Create a project.<br>
![newProject_1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_1.png)<br>
*[Figure 2.6.1.3 Creating a New Project]*<br>

[2] Add a communication module.<br>
![newProject_2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_2.png)<br>
*[Figure 2.6.1.4 Adding a Communication Module 1]*<br>

![newProject_3.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_3.png)<br>
*[Figure 2.6.1.5 Adding a Communication Module 2]*<br>

![newProject_4.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_4.png)<br>
*[Figure 2.6.1.6 Adding a Communication Module 3]*<br>

[3] Set a communication module <br>
Double-click XGL-EFMT shown in the left tab in the figure below.<br>
![newProject_6.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_6.png)<br>
*[Figure 2.6.1.7 Communication Module Settings]*<br>
- Set the IP address, subnet mask, gateway, etc.  
- To use the two LAN ports of the PLC as a relay function, select the "Relay" checkbox.  
- Change the RAPIEnet setting to Disable.

#### 2.6.1.4 Online Connection Settings
[1] Connect the PLC with a USB cable.<br>
![newProject_7.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_7.png)<br>
*[Figure 2.6.1.8 Online Connection Settings 1]*<br>

[2] Press the button shown on the left in the figure below to download the entire settings.<br>
![newProject_8.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_8.png)<br>
*[Figure 2.6.1.9 Online Connection Settings 2]*<br>

#### 2.6.1.5 Auto Scan
[1] Auto Scan is possible when connected to the PLC.<br>
If the current state is not online, click Menu > Online > Connect to change to online status.<br>

[2] Right-click XGL-EFMT > Add Item > Smart Expansion<br>
![auto1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto1.png)<br>
*[Figure 2.6.1.10 Auto Scan 1]*<br>

[3] Click Next. <br>
![auto2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto2.png)<br>
*[Figure 2.6.1.11 Auto Scan 2]*<br>

[4] Click Auto Scan. <br>
![auto3.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto3.png)<br>
*[Figure 2.6.1.12 Auto Scan 3]*<br>

![auto4.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto4.png)<br>
*[Figure 2.6.1.13 Auto Scan4]*<br>

[5] Check the automatically scanned devices.  
![auto5.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto5.png)<br>
*[Figure 2.6.1.14 Auto Scan5]*<br>

![auto6.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto6.png)<br>
*[Figure 2.6.1.15 Auto Scan6]*<br>

The Hi6 EtherNet/IP adapter device appears in the list as shown in the figure below. <br>
![auto7.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto7.png)<br>
*[Figure 2.6.1.16 Auto Scan7]*<br>

#### 2.6.1.6 Program Variable Registration
[1] Scan Program > NewProgram > Local Variables (double-click)<br>
![variable1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/variable1.png)<br>
*[Figure 2.6.1.17 Variable Registration 1]*<br>

[2] Set the input/output data to be used in communication.<br>
![variable2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/variable2.png)<br>
*[Figure 2.6.1.18 Variable Registration 2]*<br>

#### 2.6.1.7 EtherNet/IP Adapter Settings
[1] Double-click EB01 (Hi6 EtherNet/IP adapter) in the list on the left.<br>

[2] Press the EIP detailed settings button.<br>
![AdapterSetting1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting1.png)<br>
*[Figure 2.6.1.19 EtherNet/IP Adapter Settings 1]*<br>

[3] Refer to the figure below to select the setting values for the EtherNet/IP adapter. <br>
- Connection type
- T2O RPI Range, O2T RPI Range
- T2O Input, O2T Output size
- Transmission cycle
- Timeout
- Local tag, Remote tag <br>
![AdapterSetting2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting2.png) <br>
*[Figure 2.6.1.20 EtherNet/IP Adapter Settings 2]*<br>

[4] Click Online > Communication Module Settings and Diagnostics > Service Enable.<br>
![AdapterSetting3.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting3.png)<br>
*[Figure 2.6.1.21 EtherNet/IP Adapter Settings 3]*<br>

[5] Check the FEnet I/O Service checkbox.<br>
![AdapterSetting4.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting4.png)<br>
*[Figure 2.6.1.22 EtherNet/IP Adapter Settings 4]*<br>

<br>

##### 2.6.1.8 Assignment of IO Blocks after Completion of Communication Settings

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../4-io-block-allocation.md)").**
{% endhint %}# 3. EtherCAT Master IO

<br>

This chapter explains how to connect several standard Remote IO modules selected by our company using an EtherCAT Master.

<br>

##### EtherCAT Overview

EtherCAT is an Ethernet-based fieldbus system developed by Beckhoff Automation.

The EtherCAT protocol provides functions for very fast IO data updates and precise synchronization. 

<br>

##### EtherCAT Master IO
   * Products that correspond to existing fieldbus masters and can ask EtherCAT slave devices to perform I/O data connection.

<br>

{% hint style="info" %}
\.      An EtherCAT Master uses the general LAN port for the controller.


\.      A Remote IO module uses the M9386 EtherCAT network adapter from Crevis.
{% endhint %}


# 3.1 EtherCAT Master IO Settings

<br>

##### 1. Touch the menu to enter the settings screen. 
**\[System > 2: Control Parameters > 11: Industrial Communication > 4: EtherCAT Master Settings]**

<br>

![[Figure 3.1-1 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_1.png>) 

<br>

{% hint style="info" %}
\.      Check the selected controller LAN port number on the EtherCAT master settings screen. 
{% endhint %}

##### 2. Connect the controller LAN port and Remote IO cables, etc. for communication and check the status.

<br>

![[Figure 3.1-2 Hardware Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_2.png>) 
![[Figure 3.1-3 Hardware Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_3.png>) 

<br>

{% hint style="info" %}
\.      Please connect the controller and Remote IO using a LAN Cable.

\.      Set all DIP switches of the Remote IO to OFF.

\.      Connect both the Remote IO power and Field Power (24 V DC).
{% endhint %}

<br>

##### 3. Select "ON" for the EtherCAT master usage in the settings menu.

<br>

![[Figure 3.1-4 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_4.png>)

<br>

{% hint style="info" %}
\.      Set the communication cycle according to your usage environment.

\.      Communication cycles of 1 ms, 2 ms, and 5 ms are supported.
{% endhint %}

<br>

##### 4. Select the same configuration as the connected Remote IO module from the slave list in the settings menu.

<br>

![[Figure 3.1-5 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_5.png>)

<br>

{% hint style="info" %}
\.      Check the input and output byte counts.
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
\.      M5112 : Conveyer I/F 
{% endhint %}

<br>

![[Figure 3.1-6 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_6.png>) 

<br>

##### 5. Reboot the controller after completing the settings.

![[Figure 3.1-7 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_7.png>) 

<br>

![[Figure 3.1-8 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_8.png>) 

<br>

{% hint style="info" %}
\.      Please reboot the controller after completing the settings.
{% endhint %}

<br>

##### 6. After confirming that the setting values are reflected, check the communication status.

![[Figure 3.1-9 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_9.png>) 

<br>

{% hint style="info" %}
\.      Please check the communication connection status and check for any error.
{% endhint %}

<br>

![[Figure 3.1-10 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_10.png>)

<br>

{% hint style="info" %}
\.      Please check if communication is properly established using LEDs on the Remote IO Module.
{% endhint %}

<br>

{% hint style="info" %}
\.      **If an error occurs during communication, refer to ("[**3.2 EtherCAT Master IO Error Handling**](../3-ethercat-master-io/2-Error-EtherCAT-Master.md)").**
{% endhint %}

<br>

##### 7. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../4-io-block-allocation.md)").**
{% endhint %}

# 3.2 EtherCAT Master IO Error Handling

This is a method for resolving major errors that may occur during EtherCAT master IO settings.

<br>

![[Figure 3.2-1 EtherCAT Master Status]](<../_assets/3-ethercat-master-io/2-Error/image_1.png>) 

{% hint style="info" %}
\.      Please check the connection status of the LAN cable.

\.      Check if the adapter device power is on.

\.      Please check if the settings match the IO combination of the Remote IO module.
{% endhint %}

<br>
# 5. Industrial Communication IO Reading and Writing

This is the method for assigning IO blocks for the communication with the controller after completing industrial communication settings.

To use the industrial communication IO, the IO blocks should be assigned to the fb0 - fb9 area.

<br>

{% hint style="info" %}
\.      For the IO reading/writing methods for fb blocks, please refer to the manual below.

\.   **\[Controller Operation Manual: General Input]**   
\.   **\[Controller Operation Manual: General Output]**   
{% endhint %}

<br>

##### 1. Select the IO block assignment menu.
   Touch the **\[System > 2: Control Parameters > 2: Input/Output Signal Settings > 6: FB Block Assignment]** menu.

<br>

##### 2. Specify industrial communication type for the desired fb area.
   After specifying it, touch the **\[OK]** button.

![[Figure 5-1]](<_assets/4-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[Caution]**: When using together with an embedded PLC, please check IO attributes and DI/DO - X/Y.
{% endhint %}

{% hint style="warning" %}
**\[Caution]**: For an EtherNet/IP adapter, the maximum block size is 120 bytes and up to 2 blocks can be selected. Any selection exceeding 2 will be ignored. 
{% endhint %}
# 6. Slave Device Description Files

To configure the slave communication from the industrial communication master, a description file for the slave device for each protocol is used.

<br>

The slave device description files can be downloaded from our website.
Download "**${cont_model} Fieldbus Config**" from [www.hd-hyundairobotics.com](https://hd-hyundairobotics.com/) -> Industrial Robot Website -> Customer Support -> Application Software.

<br>

{% hint style="info" %}
\.      EtherNet/IP: EDS file

\.      PROFINET IO: GSDML (.XML) file

\.      EtherCAT: ESI (.XML) file

\.      PROFIBUS-DP: GSD file

\.      DeviceNet: EDS file

\.      CC-Link IE Field: CSPP file

\.      CC-Link IE Basic: CSPP file
{% endhint %}

<br>

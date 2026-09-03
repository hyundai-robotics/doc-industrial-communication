
[__SOURCE](README.md)
# Hi7 Controller Function Manual - Industrial Communication

[__SOURCE](0-about-this-manual/README.md)
# About the Manual

[__SOURCE](0-about-this-manual/precautions.md)
# Precautions

{% include file="en/precautions.md" %}

[__SOURCE](0-about-this-manual/safety-notice.md)
# Safety Cautions

{% include file="en/safety-notice.md" %}

[__SOURCE](1-cifx-pci-communication/README.md)
# 1. CIFX PCI Communication

This is a manual for the industrial communication that uses a CIFX PCI. 

[__SOURCE](1-cifx-pci-communication/1-cifx-pci-install-program/README.md)
## 1.1 CIFX PCI Program Installation

This is the method for installing programs related to industrial communication.

[__SOURCE](1-cifx-pci-communication/1-cifx-pci-install-program/1-sycon-net.md)
### 1.1.1 SYCON.net Installation

"Sycon.net" is a program provided by Hilscher for configuring the PCI communication card.

<br>

**1. SYCON.net Latest Version Download Path**

{% hint style="info" %}
   - Click **[https://hilscher.atlassian.net/](https://hilscher.atlassian.net/wiki/spaces/HILKB/overview?mode=global) -> Software -> SYCON.net**.
{% endhint %}

<br>

![[Figure 1.1.1-1 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_1.png>)

<br>

![[Figure 1.1.1-2 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_2.png>)

<br>

{% hint style="info" %}
   - Select the latest version (current release) and download it.
{% endhint %}

<br>

![[Figure 1.1.1-3 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_3.png>)

<br>

![[Figure 1.1.1-4 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_4.png>)

<br>

{% hint style="info" %}
   - Execute the downloaded SYCON.NET Setup.exe file to install the program.
{% endhint %}

<br>

![[Figure 1.1.1-5 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_5.png>)

<br>

![[Figure 1.1.1-6 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_6.png>)

<br>

{% hint style="info" %}
   - Execute the installed SYCON.NET program to check that the installation has been completed successfully.
{% endhint %}

<br>

![[Figure 1.1.1-7 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_7.png>)

<br>


**2. Download the Program from the Hyundai Robotics Website.**

{% hint style="info" %}
   - Download "**Sycon.net**" from [www.hd-hyundairobotics.com](https://hd-hyundairobotics.com/) -> Industrial Robot Website -> Customer Support -> Application Software.
{% endhint %}

<br>

{% hint style="info" %}
   - Extract -> Execute the SYCON.NET Setup.exe file to install the program.
{% endhint %}

<br>

{% hint style="info" %}
   - The SYCON.net program provided on our website may differ from the latest version.
{% endhint %}

<br>
[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/README.md)
## 1.2 CIFX PCI Communication Card Installation and Settings

To use industrial communication, a PCI communication card (from Hilscher) is required. Set the communication card and wire the connectors according to the required communication.

[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)
### 1.2.1 PCI Industrial Communication Card


<br>

**1. Install the purchased PCI communication card inside the controller's Main Module.**

<br>

**2. Rotate the rotary switch of the PCI communication card to set the Slot number.**

<br>

{% hint style="warning" %}
**\[Caution]**: The physical location of the PCI slot is independent of the rotary switch settings on the communication card.
{% endhint %}

<br>

**3. Set the slot number separately for each PCI communication card within the number ranging 1 \~ 3.**
  (When multiple PCI communication cards are used, individual numbers should be set differently.)

![[Figure 1.2.1-1 PCI Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_2.png>)

<br>

![[Figure 1.2.1-2 PCI Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_3.png>)

{% hint style="warning" %}
**\[Caution]**: Please set the rotary switch number differently for each PCI card.
{% endhint %}


[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)
### 1.2.2 Connector

<br>

**Use connectors and cables suitable for the industrial communication method.**

![[Figure 1.2.2-1 Industrial Communication Connector]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector/image_2.png>)

{% hint style="info" %}
   - DeviceNet termination resistor: 120 ohms

   - CC-Link termination resistor: 110 ohms
{% endhint %}

<br>

{% hint style="warning" %}
**\[Caution]**: Please use separate power sources for the communication cable and the IO.
{% endhint %}

<br>
[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led.md)
### 1.2.3 LED Description

<br>

**PCI LED Description**

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

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/README.md)
## 1.3 CIFX PCI Communication Settings

To use industrial communication, install a PCI communication card, and proceed with settings using the teach pendant and Sycon.net program.

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)
### 1.3.1 CIFX PCI Slot Settings.

Configure the communication method for the CIFX PCI slot. To apply the settings, please disconnect the controller power and then supply it again.

<br>

Refer to "[1.2.1 PCI Industrial Communication Card](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" and proceed with the method below.

<br>

**1. Touch the menu to enter the slot settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 1: PCI Slot Settings > Channel 1]** 


<br>

**2. Refer to the screen below to select the slot, communication method (master/slave), and protocol.**
   * The slot number is the rotary switch number of the PCI communication card.
   * If you do not want to change the communication settings, touch the **\[OK]** button to exit.

{% hint style="warning" %}
**\[Caution]**: Touching the **\[Initialize]** or **\[Apply]** button will initialize the slot information on the current tab. The Config file will also be initialized, so please be aware.
{% endhint %}

![[Figure 1.3.1-1 PCI Slot Settings]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[Figure 1.3.1-2 PCI Slot Settings (master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[Figure 1.3.1-3 PCI Slot Settings (Slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

**3. Complete the slot settings.**
Touch the **\[Apply]** menu.

![[Figure 1.3.1-4 PCI Slot Settings]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[Caution]**

<1>. When applying the settings by touching the **\[Apply]** button, all CONFIG files applied to the corresponding slot will be deleted and changed. It is recommended to keep a separate backup of existing settings when changing communication.

<2>. If you touch the **\[OK]** button without touching the **\[Apply]** button, the selected communication will not be applied.
{% endhint %}

<br>

**4. Repeat steps 2. \~ 3. for each slot.**

<br>

**5. Reboot the controller to apply the set communication.**
Touch the **\[Service > 19: Industrial Communication Monitoring]** menu to check if the set communication has been applied.

![[Figure 1.3.1-5 Industrial Communication Settings Screen]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[Caution]**: Settings are applied when the controller is rebooted after slot settings.
{% endhint %}

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)
### 1.3.2 SYCON.NET Settings

For the PCI communication card, proceed with industrial communication settings using the "**Sycon.net**" program. The setting method is as follows. (Please install by referring to "[1.1 Sycon.net Installation](../../1-cifx-pci-install-program/1-sycon-net.md)".)

<br>

**1. Connect the PC with Sycon.net installed and the general LAN port of the robot controller (not the PCI LAN port).**
Touch the **\[System > 2: Control Parameters > 9: Network]** menu to check the IP of the general LAN port. Please check the connection status through a ping test, etc.

<br>

![[Figure 1.3.2-1 Network IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_1.png>)

<br>

{% hint style="info" %}
   - IP Address can be changed according to user settings.
{% endhint %}

<br>

**2. Execute Sycon.net.**

![[Figure 1.3.2-2 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_2.png>)

<br>

**3. In the Device Catalog menu on the right side of the screen, click the item matching the set communication protocol and place it on the bus line in the center by dragging and dropping it.**

![[Figure 1.3.2-3 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_3.png>)
![[Figure 1.3.2-4 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_4.png>)

<br>

**4. Double-click the imported item to set it.**

{% hint style="info" %}
   - "Double-click" the imported CIFX PCI (figure).

   - Settings -> Driver

   - Select netX Driver.
{% endhint %}

![[Figure 1.3.2-5 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_5.png>)

{% hint style="info" %}
   - Setting -> Driver -> netX Driver -> TCP Connection

   - IP Address: Please enter the general LAN port IP address of the connected controller.
{% endhint %}

![[Figure 1.3.2-6 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_6.png>)

{% hint style="info" %}
   - Device Assignment -> Click Scan

   - Select communication (check the channel protocol) then "Apply" and "OK."
{% endhint %}

{% hint style="warning" %}
**\[Caution]**: Please be sure to check the Channel Protocol and Slot number.
{% endhint %}

{% hint style="warning" %}
**\[Caution]**: If scan is not working, check the status of the cable connection with the controller and also the PCI Slot settings.
{% endhint %}

![[Figure 1.3.2-7 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_7.png>)


{% hint style="info" %}
   - Right-click the CIFX PCI figure -> Download
{% endhint %}

![[Figure 1.3.2-8 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_8.png>)
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)
#### 1.3.2.1 SYCON.NET Help



<br>

**When using SYCON.net, if there are insufficient explanations in the manual, please refer to the "help" function below.**

<br>

![[Figure 1.3.2.1-1 SYCON.net help]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/1-Help-SYCON/image_1.png>) 

<br>

![[Figure 1.3.2.1-2 SYCON.net help]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/1-Help-SYCON/image_2.png>) 

<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/README.md)
### 1.3.3 EtherNet/IP

This chapter describes the characteristics of the EtherNet/IP master (scanner) and slave (adapter) and how to set them. 

<br>

**EtherNet/IP Overview**

EtherNet/IP is an Ethernet-based open industrial communication protocol developed by CI (ControlNet International) and ODVA (Open DeviceNet Vendors Association).

In the factory, various devices such as sensors, remote IOs, motor drivers, HMIs, PLCs, and robot controllers can be connected to one EtherNet/IP network regardless of manufacturer.

![[Figure 1.3.3-1 EtherNet/IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/image_1.png>)


<br>

EtherNet/IP is classified as follows according to the communication function.

**Scanner Class**
   * Products that correspond to existing fieldbus masters and can ask the EtherNet/IP adapters or scanners to perform I/O data connection.

<br>

**Adapter Class**
  * Products that correspond to existing fieldbus slaves and are the targets of Real-Time I/O data connections requested by EtherNet/IP scanners.

  * An adapter cannot send and receive Real-Time I/O data on their own without the scanner.

<br>

**Messaging Class**
   * Products that can send and receive explicit messages for the products of all classes, but do not support Real-Time I/O data transmission and reception.

   * For example, the products can be computer interface cards for program upload/download and network setting tools, etc.
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/1-Specification-EtherNet-IP-Scanner.md)
#### 1.3.3.1 EtherNet/IP Scanner Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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

**Connection**

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

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Settings-EtherNet-IP-Scanner.md)
#### 1.3.3.2 EtherNet/IP Scanner Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[1.3.2 SYCON.NET Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - When using SYCON.net, if there are insufficient explanations in the manual, please refer to the "[1.3.2 SYCON.NET Help](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" function.
{% endhint %}

<br>

**1. Select EtherNet/IP Master in the PCI slot settings and reboot the robot controller.**

![[Figure 1.3.3.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_1.png>)

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.3.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

**3. Select the EtherNet/IP scanner PCI device by using Sycon.net.**

![[Figure 1.3.3.2-3 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_3.png>)
![[Figure 1.3.3.2-4 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

**4. Scan the PCI device and apply the EtherNet/IP scanner.**

![[Figure 1.3.3.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

**5. Download the settings.**

![[Figure 1.3.3.2-6 EtherNet/IP Scanner Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

**6. Prepare the adapter (slave) module to be connected to the EtherNet/IP scanner.**
   * In this example, we use the M9289 EtherNet/IP adapter from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.3.2-7 Crevis M9289]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

**7. Set the IP address of the adapter (slave) for EtherNet/IP communication connection.**

{% hint style="info" %}
   - Setting an IP address using the dip switch.
{% endhint %}

![[Figure 1.3.3.2-8 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
   - How to set an IP address using BootpSvr.exe
{% endhint %}

<br>

**8. (Bootp example) Set the slave device IP address using Bootp.**
   * Change only DIP switch 9 to ON.

![[Figure 1.3.3.2-9 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_9.png>)

   * Connect the PC to the M9289 adapter LAN port.

![[Figure 1.3.3.2-10 Crevis M9289 LAN Port]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

**9. Execute BootpSvr.exe on the PC.**
   * This program is provided by Crevis. (Download and install IO Guide Pro from the website.)

![[Figure 1.3.3.2-11 Crevis IO Guide Pro]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_11.png>)

![[Figure 1.3.3.2-12 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
   - With Start BootP being pressed, disconnect and reapply power to the M9289 module to reboot it.
{% endhint %}

![[Figure 1.3.3.2-13 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

**10. When the adapter device is rebooted, the device information will appear in the BootpSvr.exe program.**

![[Figure 1.3.3.2-14 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

**11. Select the device and set the IP.**

![[Figure 1.3.3.2-15 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_15.png>)![[Figure 1.3.3.2-16 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

**12. After setting the IP, turn all DIP switches of the adapter to OFF and reboot the device.**

{% hint style="info" %}
   - Be sure to check the DIP switch status and whether the adapter is rebooted.
{% endhint %}

![[Figure 1.3.3.2-17 Crevis DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

**13. Register the slave device EDS file.**

{% hint style="info" %}
   - An EDS file is required to use a device not registered in Sycon.net.

   - The EDS file for M9289 adapter can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.3.2-18 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
   - Register the downloaded EDS file in Sycon.net.

   - When registering an EDS file, please check the industrial communication protocol (EtherNet/IP).
{% endhint %}

![[Figure 1.3.3.2-19 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_19.png>)![[Figure 1.3.3.2-20 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_20.png>)
![[Figure 1.3.3.2-21 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_21.png>)

![[Figure 1.3.3.2-22 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

**14. Network Scan**

{% hint style="info" %}
   - The EtherNet/IP scanner does not support the Network Scan function.
{% endhint %}

<br>

**15. Configure the slave (adapter) device**

{% hint style="info" %}
   - Drag the registered device and place it on the EtherNet/IP master bus line.
{% endhint %}

![[Figure 1.3.3.2-23 Sycon.net Bus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - Double-click the device (adapter) to proceed with settings.

   - Set the input/output byte count appropriate for the IO device installed in that device.

   - In this example, settings were made as follows.
{% endhint %}

<br>

![[Figure 1.3.3.2-24 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - O -> T : Originator(Master) -> Target (Slave)

   - Output : EtherNet/IP Scanner  -> M9289

   [Output Module]   
      (1) M225F (2Bytes)   
      **=> 2Bytes**   
{% endhint %}

<br>

![[Figure 1.3.3.2-25 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - T -> O : Target (Slave) -> Originator(Master)

   - Input : M9289 -> EtherNet/IP Scanner

   [Input Module]
      (1) M7001  (1Byte)
      (2) M12DF  (2Bytes)
      **=> 3Bytes**


      (1) M7002 (0Byte)
      (2) M12DF (2Bytes)
      **=> 2Bytes**  
{% endhint %}

<br>

**16. Configure the master (scanner) device.**


{% hint style="info" %}
   - Right-click the master device to disconnect it.
{% endhint %}

![[Figure 1.3.3.2-26 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - Double-click the master device.

   - Set the master device IP address. 
{% endhint %}

![[Figure 1.3.3.2-27 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - Set the slave device IP address.
{% endhint %}

![[Figure 1.3.3.2-28 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - Set the slave device scan time. 

   - Please adjust the corresponding values to set an appropriate communication speed.
{% endhint %}

![[Figure 1.3.3.2-29 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
   - Check the slave device settings in the address table.

   - Check the input/output IO byte count and start address.
{% endhint %}

![[Figure 1.3.3.2-30 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
   [Quick Connect]

   - EtherNet/IP supports the Quick Connect function.
{% endhint %}

{% hint style="info" %}
   - The following conditions should be met to use the Quick Connect function.

      (1) Products that support the Quick Connection function for the master and slaves are required  
      (2) Quick Connect cannot be used when using Auto Negotiation  
      (3) Quick Connect cannot be used when using Auto MDI-X  
      (4) 100 Mbit/s, Full Duplex required  
{% endhint %}

{% hint style="info" %}
   - After completing the settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.3.2-31 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

**17. Check the communication status**

{% hint style="info" %}
   - Check the communication status in Sycon.net and TP.

   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
   - Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.3.2-32 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_32.png>)

![[Figure 1.3.3.2-33 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
   - Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.3.2-34 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_34.png>)

<br>

**18. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/3-Specification-EtherNet-IP-Adapter.md)
#### 1.3.3.3 EtherNet/IP Adapter Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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

**Connection**

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

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Settings-EtherNet-IP-Adapter.md)
#### 1.3.3.4 EtherNet/IP Adapter Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   **[EtherNet/IP Adapter EDS File Download]**

   - Please refer to "[6. Slave Device Description File](../../../6-slave-config-file.md)".
{% endhint %}

<br>

**1. Using the TP, select an EtherNet/IP slave in the industrial communication PCI Slot settings and reboot the robot controller.**

![[Figure 1.3.3.4-1 PCI Slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.3.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > EtherNet/IP Slave]**

![[Figure 1.3.3.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.3.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
   [IP Setting]

   - Fixed IP: User sets the IP address, subnet mask, and gateway information.

   - Dynamic Allocation (DHCP): An IP address is assigned from the DHCP server.
{% endhint %}

{% hint style="info" %}
   [Input Upon Communication Error (Action in Bus Error)]

   - Clear: Initializes all inputs to 0 when a communication error occurs.

   - Hold: Maintains the last valid input value when a communication error occurs.
{% endhint %}

{% hint style="info" %}
   [Communication Error Allowable Time (Error Allowed Time)]

   - If a communication error persists for the specified allowed time, a fieldbus error signal and alarm are output.
{% endhint %}

{% hint style="info" %}
   [Input Byte Count (Input Byte)]

   - Input Byte Count: Sets the size of the data input from the master -> slave.

   - O -> T: Originator(Master) -> Target (Slave)
{% endhint %}

{% hint style="info" %}
   [Output Byte Count (Output Byte)]

   - Output Byte Count: Sets the size of the data output from the slave -> master.

   - T -> O: Target (Slave) -> Originator (Master)
{% endhint %}

{% hint style="info" %}
   [Run / Idle Header]

   - The CIFX-50 RE EtherNet/IP Adapter applied to the controller uses 32-bit Run/Idle header when exchanging IO with the scanner (default).

   - Please set whether to use the input and output 32-bit Run/Idle Header appropriately according to the scanner specifications.
{% endhint %}

<br>

{% hint style="info" %}
   [Quick Connect]

   - EtherNet/IP supports the Quick Connect function.

   - If the Quick Connect function is required, please set the EtherNet/IP Adapter using Sycon.net.

      (1) Products that support the Quick Connection function for the master and slaves are required  
      (2) Quick Connect cannot be used when using Auto Negotiation  
      (3) Quick Connect cannot be used when using Auto MDI-X  
      (4) 100 Mbit/s, Full Duplex required  
{% endhint %}

<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.3.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_5.png>)

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error-EtherNet-IP.md)
#### 1.3.3.5 EtherNet/IP Error Handling

This is a method for resolving major errors that may occur during EtherNet/IP settings.

Errors can be checked using the diagnosis function of Sycon.Net.

<br>

Please refer to "[1.4.1 ERROR Code](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

<br>

**1. Communication cable disconnection error**

{% hint style="info" %}
   - Please check the connection status of the LAN cable.

   - Check if the adapter device power is on.
{% endhint %}

![[Figure 1.3.3.5-1 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_1.png>) 


<br>

**2. IP Address setting error**

{% hint style="info" %}
   - Please check the IP addresses of the master and slave devices.

   - An error occurs if the set IP address of the adapter device differs from the value entered in Sycon.net.

{% endhint %}

![[Figure 1.3.3.5-2 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_2.png>) 

![[Figure 1.3.3.5-3 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_3.png>) 



[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/README.md)
### 1.3.4 PROFINET IO

This chapter describes the characteristics of the PROFINET IO master (controller) and slave (device) and how to set them. 

<br>

**PROFINET IO Overview**

PROFINET IO is an Ethernet-based open industrial communication protocol that has progressively evolved from PROFIBUS-DP and industrial Ethernet.

![[Figure 1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>) 

<br>

It follows the Provider-Consumer model for data exchange and can be classified into the following three classes of products.

**IO Controller Class**
   * Products that correspond to existing PROFIBUS-DP class 1 masters and are types of products in which automation programs such PLCs are running.

   * An IO controller supplies output data to the IO devices set to it and consumes the input data from them.

<br>

**IO Device Class**
  * Products that correspond to existing PROFIBUS-DP slaves and are connected to IO controllers such as PLCs through PROFINET IO.

  * An IO device supplies output data to the IO controller, provides input data, and consumes output data.

<br>

**IO Supervisor Class**
   * Products that correspond to existing PROFIBUS-DP class 2 masters and include those programming devices, PCs, HMIs that are designed for network configuration and diagnosis.

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/1-Specification-PROFINET-IO-Controller.md)
#### 1.3.4.1 PROFINET IO Controller Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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

**Connection**

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
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Settings-PROFINET-IO-Controller.md)
#### 1.3.4.2 PROFINET IO Controller Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[1.3.2 SYCON.NET Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - When using SYCON.net, if there are insufficient explanations in the manual, please refer to the ""[1.3.2 SYCON.NET Help](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" function.
{% endhint %}

<br>

**1. Select the PROFINET IO master in the PCI slot settings and reboot the robot controller.**

![[Figure 1.3.4.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.4.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

**3. Select the PROFINET IO controller PCI device by using Sycon.net.**

![[Figure 1.3.4.2-3 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_3.png>)
![[Figure 1.3.4.2-4 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

**4. Scan the PCI device and apply the PROFINET IO controller.**

![[Figure 1.3.4.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

**5. Download the settings.**

![[Figure 1.3.4.2-6 PROFINET IO Controller Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

**6. Prepare the device (slave) module to be connected to the PROFINET IO controller.**
   * In this example, we use the M9287 PROFINET IO device from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.4.2-7 Crevis M9287]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
   - How to set the PROFINET IO device name using the DIP switch

   - M9287-XX: Number set using the DIP switch

   - In this example, the name was set to M9287-01 using DIP switch 1.
{% endhint %}

<br>

**7. (DIP switch use example) Set the slave device name using the DIP Switch.**
   * Change only DIP Switch 1 to ON.


![[Figure 1.3.4.2-8 Crevis M9287 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
   - Please reboot the device after setting the DIP switch.
{% endhint %}

<br>

**8. Register the slave device GSDML file.**

{% hint style="info" %}
   - A GSDML file is required to use a device not registered in Sycon.net.

   - The GSDML file for the M9287 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.4.2-9 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
   - Register the downloaded GSDML file in Sycon.net.

   - When registering a GSDML file, please check the industrial communication Protocol (PROFINET IO).
{% endhint %}

![[Figure 1.3.4.2-10 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_10.png>)![[Figure 1.3.4.2-11 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_11.png>)
![[Figure 1.3.4.2-12 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_12.png>)

![[Figure 1.3.4.2-13 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_13.png>)


<br>

**9. Network Scan**

{% hint style="info" %}
   - The PROFINET IO controller supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
   - Right-click the PROFINET IO master device and click Network Scan.
{% endhint %}

![[Figure 1.3.4.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
   - If there is no GSDML file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

![[Figure 1.3.4.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - If a GSDML file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.4.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_16.png>)

![[Figure 1.3.4.2-17 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_17.png>)

![[Figure 1.3.4.2-18 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

**10. Configure the slave (device).**

{% hint style="info" %}
   - Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.4.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - Double-click the slave device.
{% endhint %}

![[Figure 1.3.4.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - Add a slot connected to M9287 to set the PROFINET IO slave (device).

   - Slot 1 : M7001  
   - Slot 2 : M12DF  
   - Slot 3 : M225F  
{% endhint %}

![[Figure 1.3.4.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_21.png>)

![[Figure 1.3.4.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

**11. Configure the master (controller) device**

{% hint style="info" %}
   - Double-click the Master device.
{% endhint %}

![[Figure 1.3.4.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - Set the IP addresses of the master and slave devices.

   - The slave IP address of the PROFINET IO Device is to be set from the master.

   - Please ensure that the IP addresses of the master and slave do not overlap within the same band.
{% endhint %}

![[Figure 1.3.4.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_24.png>)

![[Figure 1.3.4.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - Check from the master device if the slot information of the slave device is correct.
{% endhint %}

![[Figure 1.3.4.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.4.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - Set the IO communication speed for the PROFINET IO.
{% endhint %}

![[Figure 1.3.4.2-28 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.4.2-29 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

**12. Check the communication status.**

{% hint style="info" %}
   - Check the communication status in Sycon.net and TP.

   - For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
   - Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.4.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_30.png>)

![[Figure 1.3.4.2-31 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
   - Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.4.2-32 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_32.png>)

<br>

**13. Assign IO blocks after completing the settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/3-Specification-PROFINET-IO-Device.md)
#### 1.3.4.3 PROFINET IO Device Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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

**Connection**

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

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Settings-PROFINET-IO-Device.md)
#### 1.3.4.4 PROFINET IO Device Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   **[PROFINET IO Device GSDML File Download]**

   - Please refer to "[6. Slave Device Description File](../../../6-slave-config-file.md)".
{% endhint %}

<br>

**1. Using the TP, select a PROFINET IO slave in the industrial communication PCI Slot settings and reboot the robot controller.**

![[Figure 1.3.4.4-1 PCI Slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_1.png>)

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.4.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > PROFINET IO Slave]**

![[Figure 1.3.4.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[Figure 1.3.4.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
   [Station Name]

   - The PROFINET IO identifies a slave through the station name.

   - Naming Rule
      - Device names connected by PROFINET IO cannot be duplicated.  
      - A name can be set up to 240 characters.  
      - Special characters "." and "-" can be used.  
      - Lowercase English letters and numbers can be used.  
      - Names should start and end with lowercase English letters or numbers.  
{% endhint %}

{% hint style="info" %}
   [Input Byte Count (Input Byte)]

   - Input Byte Count: Sets the size of the data input from the master -> slave.
{% endhint %}

{% hint style="info" %}
   [Output Byte Count (Output Byte)]

   - Output Byte Count: Sets the size of the data output from the slave -> master.
{% endhint %}

<br>

{% hint style="info" %}
   [When Setting a Slot from the Master]

   - Master Input (32byte)  <--  Slave Output (32bytes)

   - Master Output (256bytes = 64bytes * 4)  -->  Slave Input (256bytes)

   - 4, 8, 16, 32, and 64 Bytes -> Specify the slot matching each byte count  
   - 128 and 256 Bytes -> Specify multiple 64-byte slots (2, 4)

   - The input slot is located before the output slot.
{% endhint %}

<br>

![[Figure 1.3.4.4-5 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_5.png>) 


<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.4.4-6 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_6.png>)

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/5-Error-PROFINET-IO.md)
#### 1.3.4.5 PROFINET IO Error Handling

<br>

Please refer to "[1.4.1 ERROR Code](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".




[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/README.md)
### 1.3.5 EtherCAT

This chapter describes the characteristics of EtherCAT master and slave and how to set them.

<br>

**EtherCAT Overview**

EtherCAT is an Ethernet-based fieldbus system developed by Beckhoff Automation.

The EtherCAT protocol provides functions for very fast IO data updates and precise synchronization. 

<br>

**EtherCAT Master**
   * Products that correspond to existing fieldbus masters and can ask EtherCAT slave devices to perform I/O data connection.

<br>

**EtherCAT Slave**
   * Products that correspond to existing fieldbus slaves and are connected to the EtherCAT master device.

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/1-Specification-EtherCAT-Master.md)
#### 1.3.5.1 EtherCAT Master Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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

**Connection**

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
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Settings-EtherCAT-Master.md)
#### 1.3.5.2 EtherCAT Master Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[1.3.2 SYCON.NET Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - When using SYCON.net, if there are insufficient explanations in the manual, please refer to the "[1.3.2 SYCON.NET Help](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" function.
{% endhint %}

<br>

**1. Select the EtherCAT master in the PCI slot settings and reboot the robot controller.**

![[Figure 1.3.5.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_1.png>) 

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.5.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_2.png>) 

<br>

**3. Select the EtherCAT master PCI device by using Sycon.net.**

![[Figure 1.3.5.2-3 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_3.png>)
![[Figure 1.3.5.2-4 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_4.png>) 

<br>

**4. Scan the PCI device and apply the EtherCAT master.**

![[Figure 1.3.5.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_5.png>) 

<br>

**5. Download the settings.**

![[Figure 1.3.5.2-6 EtherCAT Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_6.png>) 

<br>

**6. Prepare the slave module to be connected to the EtherCAT master.**
   * In this example, we use the M9386 EtherCAT slave from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.5.2-7 Crevis M9386]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_7.png>) 

<br>

**7. Slave device station address**

{% hint style="info" %}
   - The station address of the EtherCAT slave device is set by the master.
{% endhint %}

<br>

**8. Register the slave device XML file.**

{% hint style="info" %}
   - An XML file is required to use a device not registered in Sycon.net.

   - The XML file for the M9386 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.5.2-8 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_8.png>)

{% hint style="info" %}
   - Register the downloaded XML file in Sycon.net.

   - When registering an XML File, please check the industrial communication Protocol (EtherCAT).
{% endhint %}

![[Figure 1.3.5.2-9 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_9.png>)

<br>

![[Figure 1.3.5.5-10 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.5.2-11 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_11.png>)

<br>

![[Figure 1.3.5.2-12 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_12.png>)


<br>

**9. Network Scan**

{% hint style="warning" %}
   **For EtherCAT, the available cable connections and ports are specified.**

   **For smooth communication connection, be sure to check ("[1.3.5.5 EtherCAT Cable Wiring](../5-EtherCAT/5-EtherCAT-Topology.md)").**
{% endhint %}

{% hint style="info" %}
   - The EtherCAT master supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
   - Right-click the EtherCAT master device and click Network Scan.
{% endhint %}

![[Figure 1.3.5.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_13.png>)

{% hint style="warning" %}
   - If there is no XML file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

{% hint style="info" %}
   - If an XML file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.5.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_14.png>)

<br>

**10. Configure the slave device.**

{% hint style="info" %}
   - Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.5.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - Double-click the slave device.
{% endhint %}

![[Figure 1.3.5.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_16.png>)

{% hint style="info" %}
   - Add a slot connected to M9386 to set the EtherCAT slave.

   - Slot 1 : M7001  
   - Slot 2 : M12DF  
   - Slot 3 : M225F  
{% endhint %}

![[Figure 1.3.5.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_17.png>)

![[Figure 1.3.5.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_18.png>)


<br>

**11. Configure the master device.**

{% hint style="info" %}
   - Double-click the Master device.
{% endhint %}

![[Figure 1.3.5.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - Synchronization: Select Freerun/DC (Distributed Clocks).

   - Whether to use Redundancy (cannot be used together with Distributed Clocks)

   - Bus Cycle Time: At least 250 us is supported. (1 ms or more is recommended.)
{% endhint %}

<br>

{% hint style="info" %}
   - You can set the station address for each slave.
{% endhint %}

![[Figure 1.3.5.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.5.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_21.png>)


{% hint style="info" %}
   - After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.5.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_22.png>)

<br>

**12. Check the communication status.**

{% hint style="info" %}
   - Check the communication status in Sycon.net and TP.

   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
   - Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.5.2-23 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_23.png>)

![[Figure 1.3.5.2-24 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.5.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_25.png>)

<br>

**13. Assign IO blocks after completing the settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/3-Specification-EtherCAT-Slave.md)
#### 1.3.5.3 EtherCAT Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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

**Connection**

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

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Settings-EtherCAT-Slave.md)
#### 1.3.5.4 EtherCAT Slave Settings

<br>

{% hint style="info" %}
   **[EtherCAT Slave ESI EDS File Download]**

   - Please refer to "[6. Slave Device Description File](../../../6-slave-config-file.md)".
{% endhint %}

<br>

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

**1. Using the TP, select an EtherCAT slave in the industrial communication PCI Slot settings and reboot the robot controller.**

![[Figure 1.3.5.4-1 PCI Slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Slave_setting/image_1.png>) 

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.5.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > EtherCAT Slave]**

![[Figure 1.3.5.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Slave_setting/image_3.png>) 

![[Figure 1.3.5.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
   [IO Type and Size]   
   - TxPDO: Slave -> Master   
   - RxPDO: Master -> Slave   
   - Max Size: 256 bytes   
{% endhint %}

<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.5.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Slave_setting/image_5.png>)

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-EtherCAT-Topology.md)
#### 1.3.5.5 EtherCAT Cable Wiring (Topology)

<br>

Unlike existing industrial communications, EtherCAT has restrictions in cable wiring and usable Ethernet Ports.

**1. Ethernet Port**

{% hint style="info" %}
   - When connecting the EtherCAT master and slave, port 0 should be used.
{% endhint %}

![[Figure 1.3.5.5-1 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
   - When one slave is connected to the master
{% endhint %}

![[Figure 1.3.5.5-2 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
   - When two or more slaves are connected to the master

   - Connect from the slave port 1 to the next slave port 0.
{% endhint %}

![[Figure 1.3.5.5-3 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_3.png>)

<br>

**2. Redundancy**

{% hint style="info" %}
   - When using the Redundancy function in the master 

   - Connect port 1 of the last slave and port 1 of the master to form a ring structure.
{% endhint %}

![[Figure 1.3.5.5-4 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_4.png>) 


<br>

**3. Cable wiring error**


Please refer to "[1.4.1 ERROR Code](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

<br>

{% hint style="info" %}
   - If the Network scan function is not working.

   - Please check the port and cable connected to the master.
{% endhint %}

![[Figure 1.3.5.5-5 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
   - Topology Error (Error in Configuration)

   - Please check the cable wiring between the master and slave.
{% endhint %}

![[Figure 1.3.5.5-6 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
   - Topology error 2 (normal during configuration but there is an error during diagnosis)

   - Please check the cable wiring between the master and slave.

   - Please check the cable wiring between slaves.
{% endhint %}

![[Figure 1.3.5.5-7 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_7.png>)

![[Figure 1.3.5.5-8 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
   - Mandatory Slave Missing Error

   - Please check the cable wiring between slaves.
{% endhint %}

![[Figure 1.3.5.5-9 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_9.png>)
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/README.md)
### 1.3.6 PROFIBUS-DP

This chapter describes the characteristics of the PROFIBUS-DP master and slave and how to set them. 

<br>

**Fieldbus Overview**

Fieldbus is an industry standard that has been opened for connecting devices such as sensors, buttons, motor drivers, and operation interfaces to PLCs (Programmable Logic Controllers) with a single cable and operating them in factories.

Fieldbus provides intelligent services such as central monitoring of the status of the entire network and reconfiguration of the network.

For example, it is possible to set detailed information, operations, and modes for sensors and switches, not just simple On/Off.

Using a single cable reduces time and costs for wiring, simplifies the configuration, and provides advantage in maintenance.

Also, unlike protocols with non-deterministic response characteristics of general communications, fieldbuses guarantee data response speed to satisfy industrial applications where critical time characteristics are important.

![[Figure 1.3.6-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/image_1.png>) 

<br>

One fieldbus network connects one master device and multiple slave devices.
The master device searches and manages the entire network and exchanges data with slave devices.

Generally, a PLC is a master device, while sensors, buttons, controllers, etc. can be configured as slave devices.
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/1-Specification-PROFIBUS-DP-Master.md)
#### 1.3.6.1 PROFIBUS-DP Master Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Settings-PROFIBUS-DP-Master.md)
#### 1.3.6.2 PROFIBUS-DP Master Settings


Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[1.3.2 SYCON.NET Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - When using SYCON.net, if there are insufficient explanations in the manual, please refer to the ""[1.3.2 SYCON.NET Help](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" function.
{% endhint %}

<br>

**1. Select the PROFIBUS-DP master in the PCI slot settings and reboot the robot controller.**

![[Figure 1.3.6.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.6.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_2.png>)

<br>

**3. Select the PROFIBUS-DP master PCI device by using Sycon.net.**

![[Figure 1.3.6.2-3 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[Figure 1.3.6.2-4 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

**4. Scan the PCI device and apply the PROFIBUS-DP master.**

![[Figure 1.3.6.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>


**5. Download the settings.**

![[Figure 1.3.6.2-6 PROFIBUS-DP Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

**6. Prepare the slave module to be connected to the PROFIBUS-DP Master.**
   * In this example, we use the GN-9222 PROFIBUS-DP slave from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.6.2-7 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_7.png>) 


<br>

**7. Set the slave device**

{% hint style="info" %}
   - Set the node number and termination of the PROFIBUS-DP slave device.
{% endhint %}

![[Figure 1.3.6.2-8 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_8.png>) 


{% hint style="info" %}
   - Termination: To be set using the DIP switch (Example: Termination processing ON)

   - Node ID (station number): To be set using the DIP switch (Example: Node 3)
{% endhint %}

<br>

**8. Register the slave device GSD file.**

{% hint style="info" %}
   - A GSD file is required to use a device not registered in Sycon.net.

   - The GSD file for the GN-9222 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.6.2-9 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_9.png>)

{% hint style="info" %}
   - Register the downloaded GSD file in Sycon.net.

   - When registering a GSD file, please check the industrial communication protocol (PROFIBUS-DP).
{% endhint %}

![[Figure 1.3.6.2-10 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.6.5-11 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_11.png>)

![[Figure 1.3.6.5-12 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_12.png>)



<br>

**9. Network Scan**

{% hint style="warning" %}
   **When performing the Network Scan function, be sure to check the following.**

   **(1) Whether a cable is connected.**  
   **(2) Whether a termination DIP switch is used.**  
{% endhint %}

{% hint style="info" %}
   - PROFIBUS-DP master supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
   - Right-click the PROFIBUS-DP master device and click Network Scan.
{% endhint %}

![[Figure 1.3.6.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
   - If there is no GSD file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

{% hint style="info" %}
   - If a GSD file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.6.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

**10. Configure the slave device**

{% hint style="info" %}
   - Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.6.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - Double-click the slave device.
{% endhint %}

![[Figure 1.3.6.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_16.png>)

{% hint style="info" %}
   - Check the PROFIBUS-DP slave settings.

   - Slot 1 : GN-9222  
   - Slot 2 : GT-12DF (Input 2 Byte)  
   - Slot 3 : GT-227F (Output 2 Byte)  
   - Slot 4 : GT-3154 (Input 8 Byte)  
   - Slot 5 : GT-4254 (Output 8 Byte)  
{% endhint %}

![[Figure 1.3.6.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_17.png>)

<br>

![[Figure 1.3.6.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_18.png>)


<br>

**11. Configure the master device.**

{% hint style="info" %}
   - Double-click the Master device.
{% endhint %}

![[Figure 1.3.6.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_19.png>)


{% hint style="info" %}
   - Set the PROFIBUS-DP communication speed.

   - 9.6 - 12000 Kbit/s 
{% endhint %}

![[Figure 1.3.6.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - Check from the master device if the slot information of the slave device is correct.
{% endhint %}

![[Figure 1.3.6.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
   - Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.6.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
   - Check if each device in the station table is in active status.
{% endhint %}

![[Figure 1.3.6.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_23.png>)


{% hint style="info" %}
   - After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.6.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

**12. Check the communication status.**

{% hint style="info" %}
   - Check the communication status in Sycon.net and TP.

   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
   - Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.6.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[Figure 1.3.6.2-26 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - Using Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.6.2-27 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_27.png>)

<br>

**13. Assign IO blocks after completing the settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/3-Specification-PROFIBUS-DP-Slave.md)
#### 1.3.6.3 PROFIBUS-DP Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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


[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Settings-PROFIBUS-DP-Slave.md)
#### 1.3.6.4 PROFIBUS-DP Slave Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   **[PROFIBUS-DP Slave GSD File Download]**

   - Please refer to "[6. Slave Device Description File](../../../6-slave-config-file.md)".
{% endhint %}

<br>

**1. Using the TP, select a PROFIBUS-DP slave in the industrial communication PCI Slot settings and reboot the robot controller.**

![[Figure 1.3.6.4-1 PCI Slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.6.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > PROFIBUS-DP Slave]**

![[Figure 1.3.6.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.6.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
   [Station Address]

   - The PROFIBUS-DP identifies a slave through the station address.
{% endhint %}

{% hint style="info" %}
   [Input Byte Count (Input Byte)]

   - Input Byte Count: Sets the size of the data input from the master -> slave.
{% endhint %}

{% hint style="info" %}
   [Output Byte Count (Output Byte)]

   - Output Byte Count: Sets the size of the data output from the slave -> master.
{% endhint %}

{% hint style="info" %}
   [When Setting a Module from the Master]

   - Modules should be specified from the master to match the set byte count.

   - Order: Master Input (64-1) -> Master Output (64-1)

   - EX) Master Input 109 bytes  <---  Slave Output 109 bytes   
         - Input 109 Bytes : 64Byte + 32Byte + 8Byte + 4Byte + 1 Byte

   - EX) Master Output 120 bytes  --->  Slave Input 120 bytes   
         - Output 120 Bytes : 64Byte + 32Byte + 16Byte + 8Byte


   - EX) Master Input 12 bytes  <---  Slave Output 12 bytes   
         - Input 12 Bytes : 8Byte + 4Byte

   - EX) Master Output 200 bytes  --->  Slave Input 200 bytes   
         - Output 200 Bytes : 64Byte + 64Byte + 64Byte + 8Byte

   - The input module is located before the output module.
{% endhint %}

![[Figure 1.3.6.4-5 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>)


<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.6.4-6 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>)

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/5-Error-PROFIBUS-DP.md)
#### 1.3.6.5 PROFIBUS-DP Error Handling

<br>

Please refer to "[1.4.1 ERROR Code](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/README.md)
### 1.3.7 DeviceNet

This chapter describes the characteristics of the DeviceNet master and slave and how to set them. 

<br>

**Fieldbus Overview**

Fieldbus is an industry standard that has been opened for connecting devices such as sensors, buttons, motor drivers, and operation interfaces to PLCs (Programmable Logic Controllers) with a single cable and operating them in factories.

Fieldbus provides intelligent services such as central monitoring of the entire network status and reconfiguration of the network.

For example, it is possible to set detailed information, operations, and modes for sensors and switches, not just simple On/Off.

Using a single cable reduces time and costs for wiring, simplifies the configuration, and provides advantage in maintenance.

Also, unlike protocols with non-deterministic response characteristics of general communications, fieldbuses guarantee data response speed to satisfy industrial applications where critical time characteristics are important.

![[Figure 1.3.7-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/image_1.png>)

<br>

One fieldbus network connects one master device and multiple slave devices.
The master device searches and manages the entire network and exchanges data with slave devices.

Generally, a PLC is a master device, while sensors, buttons, controllers, etc. can be configured as slave devices.
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/1-Specification-DeviceNet-Master.md)
#### 1.3.7.1 DeviceNet Master Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Settings-DeviceNet-Master.md)
#### 1.3.7.2 DeviceNet Master Settings (SYCON)

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[1.3.2 SYCON.NET Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - When using SYCON.net, if there are insufficient explanations in the manual, please refer to the ""[1.3.2 SYCON.NET Help](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" function.
{% endhint %}

<br>

{% hint style="info" %}
   - For DeviceNet connector connection, please refer to the following.

      ("[1.2.2 Connector](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. Select the DeviceNet master in the PCI slot settings and reboot the robot controller.**

![[Figure 1.3.7.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_1.png>)

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.7.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_2.png>) 

<br>

**3. Select the DeviceNet master PCI device by using Sycon.net.**

![[Figure 1.3.7.2-3 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_3.png>)
![[Figure 1.3.7.2-4 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_4.png>) 

<br>

**4. Scan the PCI device and apply the DeviceNet master.**

![[Figure 1.3.7.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_5.png>) 

<br>

**5. Set the communication speed.**

{% hint style="warning" %}
   - If the communication speed differs between the master and the slave, the Network Scan function does not work normally.
{% endhint %}

![[Figure 1.3.7.2-6 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_6.png>) 

<br>

**6. Download the settings.**

![[Figure 1.3.7.2-7 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_7.png>) 

<br>

**7. Prepare the slave module to be connected to the DeviceNet master.**
   * In this example, we use the NA-9211 DeviceNet slave from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.7.2-8 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_8.png>) 

<br>

**8. Set the slave device.**

{% hint style="info" %}
   - Set the MAC ID, communication speed, and termination resistor of the DeviceNet slave device.
{% endhint %}

![[Figure 1.3.7.2-9 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_9.png>) 

![[Figure 1.3.7.2-10 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_10.png>)

{% hint style="info" %}
   [Example Settings]

   - Termination resistor: Used by being installed in the cable (termination DIP switch OFF)

   - MAC ID (station number): Set to 4 (Only DIP switch 3 is ON.)

   - Communication speed (baudrate): Set to Auto (DIP switches 7 and 8 are ON.)
{% endhint %}

<br>

**9. Register the slave device EDS file.**

{% hint style="info" %}
   - An EDS file is required to use a device not registered in Sycon.net.

   - The EDS file for NA-9211 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.7.2-11 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_11.png>)

{% hint style="info" %}
   - Register all downloaded EDS files in Sycon.net.

   - When registering an EDS file, please check the industrial communication protocol (DeviceNet).
{% endhint %}

![[Figure 1.3.7.2-12 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_12.png>)

<br>

![[Figure 1.3.7.5-13 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_13.png>)



<br>

**10. Network Scan**

{% hint style="warning" %}
   **When performing the Network Scan function, be sure to check the following.**

   **(1) Whether a cable is connected.**  
   **(2) Whether a termination resistor is connected or a termination DIP switch is used.**  
   **(3) Whether the master - slave communication speed is set.**  

   **For smooth communication connection, be sure to check ("[1.3.7.5 DeviceNet ERROR Handling](../7-DeviceNet/6-Error-DeviceNet.md)").**
{% endhint %}

{% hint style="info" %}
   - The DeviceNet master supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
   - Right-click the DeviceNet master device and click Network Scan.
{% endhint %}

![[Figure 1.3.7.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
   - If there is no EDS file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

{% hint style="info" %}
   - If an EDS file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.7.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_15.png>)

![[Figure 1.3.7.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_16.png>)

<br>

**11. Configure the slave device**

{% hint style="info" %}
   - Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.7.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
   - Double-click the slave device.
{% endhint %}

![[Figure 1.3.7.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_18.png>)


<br>

{% hint style="info" %}
   - Set the connection type of the slave device.

   - Select the message transmission method for DeviceNet communication connection.

   **If the UCMM checkbox is not checked, UCMM group 2 is set as the default value.**   

   - UCMM GROUP 1 : IO Message   
   - UCMM GROUP 2: Master - Slave connection message during network initialization (default setting)   
   - UCMM GROUP 3: Explicit Message   

   - For certain devices, UCMM group 3 may be used, so please check the product specifications before proceeding.
{% endhint %}

![[Figure 1.3.7.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_19.png>)

<br>

{% hint style="info" %}
   - For Crevis NA-9211, proceed without checking the UCMM check box. (Use the group 2 default value.)
{% endhint %}

![[Figure 1.3.7.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_20.png>)

<br>


{% hint style="info" %}
   - Check the DeviceNet slave settings.

   - Output: ST-2318 (1 byte)  
   - Input: ST-1218 (1 byte)  
{% endhint %}

<br>

{% hint style="info" %}
   - Required to set according to the communication method (Poll, Change of State, Cyclic, Bit-Strobe).
{% endhint %}

<br>

![[Figure 1.3.7.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_21.png>)

<br>

{% hint style="info" %}
   [Production Inhibit Time]

   - Set the IO data generation cycle of the slave device (ms)  

   - Example) 10 ms: IO data is generated every 10 ms.  
   - Example) 0 ms: The slave generates IO data as quickly as possible.  

   - The shorter the cycle, the greater the load on the slave device may be. (Specifications need to be checked for each slave.) 
{% endhint %}

<br>

{% hint style="info" %}
   [Expected Packet Rate]

   - Set the time for IO data update between the master and the slave.  
{% endhint %}

<br>

![[Figure 1.3.7.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_22.png>)



<br>

**12. Configure the master device**

{% hint style="info" %}
   - Double-click the Master device.
{% endhint %}

![[Figure 1.3.7.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_23.png>)


{% hint style="info" %}
   - Set the DeviceNet communication speed (to be the same as the slave communication speed).
{% endhint %}

![[Figure 1.3.7.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.7.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - Set whether to use the Quick Connect function.
{% endhint %}

![[Figure 1.3.7.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_26.png>)


{% hint style="info" %}
   - After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.7.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_27.png>)

<br>

**13. Check the communication status.**

{% hint style="info" %}
   - Check the communication status in Sycon.net and TP.

   - For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
   - Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.7.2-28 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_28.png>)

![[Figure 1.3.7.2-29 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_29.png>)

{% hint style="info" %}
   - Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.7.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_30.png>)

<br>

**14. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Settings-DeviceNet-Master-tp.md)
#### 1.3.7.3 DeviceNet Master Settings (TP)

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - For DeviceNet connector connection, please refer to the following.

      ("[1.2.2 Connector](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. Select the DeviceNet master in the PCI slot settings and reboot the robot controller.**

![[Figure 1.3.7.3-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_1.png>)

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.7.3-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Select the DeviceNet master PCI device by using Sycon.net.**

**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > DeviceNet Master]**

![[Figure 1.3.7.3-3 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_3.png>)

![[Figure 1.3.7.3-4 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="warning" %}
**\[TP Network Scan Limitations]**   
   - Only Poll Connection is supported   
   - Quick Start is not supported  

{% endhint %}

<br>

{% hint style="info" %}
   [Use (Enable / Disable)]   
   - Off: DeviceNet Master disabled   
   - On: DeviceNet Master enabled   

   [Baud Rate]   
   - 125 kbit/s   
   - 250 kbit/s   
   - 500 kbit/s   

   [Master MAC ID]   
   - The MAC ID of the DeviceNet Master is fixed to 0   

   [IO Update Cycle]   
   - Production Inhibit Time: Minimum time interval between IO updates   
   - Expected Packet Rate: Expected time interval for packets to be received normally (related to timeout)   

{% endhint %}

<br>

**5. Click the "Network Scan" button after configuring the settings according to the communication environment.**

<br>

**10. Network Scan**

{% hint style="warning" %}
   **When performing the Network Scan function, be sure to check the following.**

   **(1) Whether a cable is connected.**  
   **(2) Whether a termination resistor is connected or a termination DIP switch is used.**  
   **(3) Whether the master - slave communication speed is set.**  

   **For smooth communication connection, be sure to check ("[1.3.7.5 DeviceNet ERROR Handling](../7-DeviceNet/5-Error-DeviceNet.md)").**
{% endhint %}

<br>

![[Figure 1.3.7.3-5 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_5.png>)

<br>

**6. After checking the device settings, click the "OK" button to apply the communication settings.**

<br>

![[Figure 1.3.7.3-6 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_6.png>)

<br>

**7. Description of node settings**

{% hint style="info" %}
   [Node information]   
   - Node: MAC ID of the device   
   - Product Name: Product name of the device   
   - Vendor ID: Unique ID of the device manufacturer   
   - Status: Status value of the device   
   
   [IO settings]   
   - Output Size: Master --> Slave (in bytes)   
   - Input Size: Slave --> Master (in bytes)   
   
   [IO update cycle]   
   - PIT (Production Inhibit Time): Minimum time interval between IO updates   
   - EPR (Expected Packet Rate): Expected time interval for packets to be received normally (related to timeout)   

{% endhint %}

<br>

{% hint style="info" %}
   [PIT (Production Inhibit Time)]   
   - After the network scan, the PIT is automatically calculated based on the total IO size of the connected devices.   

   - Example 1)   
      - 125 Kbit/s   
      - Total Input + Output: 100 byte   
      - Time required for 1 cycle: 100 x 8 (bit) / 125K = 6.4ms   
      - Applying a 33% communication load: 6.4 ms x 3 = 19.2ms --> PIT set to 20ms   

   - Example 2)   
      - 250 Kbit/s   
      - Total Input + Output: 500 byte   
      - Time required for 1 cycle: 500 x 8 (bit) / 250K = 16ms   
      - Applying a 33% communication load: 16 ms x 3 = 48ms --> PIT set to 48ms   

   - The PIT value can be changed individually for each device.   
   - A shorter interval may increase the communication load on the device. (check the specifications of each device.)   

{% endhint %}

<br>

![[Figure 1.3.7.3-7 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_7.png>)

<br>

**8. Check the communication status.**

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.7.3-8 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_8.png>)

<br>

![[Figure 1.3.7.3-9 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_9.png>)

<br>

**9. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Specification-DeviceNet-Slave.md)
#### 1.3.7.4 DeviceNet Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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


[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Settings-DeviceNet-Slave.md)
#### 1.3.7.5 DeviceNet Slave Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   **[DeviceNet Slave EDS File Download]**

   - Please refer to "[6. Slave Device Description File](../../../6-slave-config-file.md)."
{% endhint %}

<br>

{% hint style="info" %}
   - For DeviceNet connector connection, please refer to the following.

      ("[1.2.2 Connector](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. Using the TP, select a DeviceNet slave in the industrial communication PCI Slot settings and reboot the robot controller.**

![[Figure 1.3.7.5-1 PCI Slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Slave_setting/image_1.png>) 

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.7.5-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > DeviceNet Slave]**

![[Figure 1.3.7.5-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Slave_setting/image_3.png>) 

![[Figure 1.3.7.5-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
   [Station Address = Mac ID]

   - The DeviceNet identifies a slave through the station address (MAC ID) (1-63).
{% endhint %}

{% hint style="info" %}
   [Communication Speed (Baudrate)]

   - You can select among 125, 250, and 500 Kbit/s.
{% endhint %}

{% hint style="info" %}
   [Input Byte Count (Input Byte)]

   - Input Byte Count: Sets the size of the data input from the master -> slave.
{% endhint %}

{% hint style="info" %}
   [Output Byte Count (Output Byte)]

   - Output Byte Count: Sets the size of the data output from the slave -> master.
{% endhint %}


<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.7.5-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Slave_setting/image_5.png>) 

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Error-DeviceNet.md)
#### 1.3.7.6 DeviceNet Error Handling

<br>

Please refer to "[1.4.1 ERROR Code](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

<br>

**1. DeviceNet termination resistor**

{% hint style="info" %}
   - A resistor should be added at the termination when connecting the DeviceNet cable.

   - If the Network Scan function does not work, please check the termination resistor.

   - DeviceNet termination resistor: 120 ohms
{% endhint %}

{% hint style="info" %}
   - As shown in the figure below, if the CIFX-50 DN PCI is at the DeviceNet termination, please add a termination resistor.
{% endhint %}

![[Figure 1.3.7.6-1 DeviceNet Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Error/image_1.png>) 

{% hint style="info" %}
   - As shown in the figure below, if the DeviceNet Remote IO is at the termination, please add a termination resistor or operate the DIP switch.
{% endhint %}

![[Figure 1.3.7.6-2 DeviceNet Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Error/image_2.png>) 

<br>

**2. Communication Speed**

{% hint style="info" %}
   - If the communication speed differs between the DeviceNet master and slave, the Network Scan function may not work.

   - If the Network Scan function does not work, please check the communication speed.
{% endhint %}

![[Figure 1.3.7.6-3 DeviceNet Baudrate]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Error/image_3.png>) 

<br>

**3. DeviceNet ERROR**

{% hint style="info" %}
   - If a 24V power is not supplied to the DeviceNet cable, the following error will appear.

   - Please check the 24V power supply.
{% endhint %}

![[Figure 1.3.7.6-4 DeviceNet Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Error/image_4.png>) 
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/7-DeviceNet-Object.md)
#### 1.3.7.7 DeviceNet Object


<br>

**1. Object**


The inside of the DeviceNet device is composed of a collection of objects. Each object represents a specific component inside the device.

<br>

![[Figure 1.3.7.7-1 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/7-Object/image_1.png>) 


<br>

Individual objects are distinguished using a class code.

<br>

![[Figure 1.3.7.7-2 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/7-Object/image_2.png>)

<br>

The inside of an object is composed of an instance number and attribute ID.

<br>

The DeviceNet master can access an object of a specific slave through a explicit message.

<br>

{% hint style="info" %}
   - EX) Object of Crevis GN-9212 (The corresponding information can be found in the Crevis manual.)

   - Reading the vendor ID value of the identity object (class code 0x01)

   - Instance : 1

   - Attribute ID : 1

   - Permission: Get (Read only possible)
{% endhint %}


![[Figure 1.3.7.7-3 DeviceNet Object Crevis GN-9212]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/7-Object/image_3.png>)


<br>

Each Object, Instance, and Attribute inside has different access permissions.

<br>

{% hint style="info" %}
   - Access permissions

   - Get: Read permission

   - Set: Write permission 

   - Attribute Single: Can access only one attribute item at a time.

   - Attribute All: Can access all attributes in Instance at once.
{% endhint %}

<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/README.md)
### 1.3.8 CC-Link

This chapter describes the characteristics of CC-Link slaves and how to set them. 


<br>

**Fieldbus Overview**

Fieldbus is an industry standard that has been opened for connecting devices such as sensors, buttons, motor drivers, and operation interfaces to PLCs (Programmable Logic Controllers) with a single cable and operating them in factories.

Fieldbus provides intelligent services such as central monitoring of the status of the entire network and reconfiguration of the network.

For example, it is possible to set detailed information, operations, and modes for sensors and switches, not just simple On/Off.

Using a single cable reduces time and costs for wiring, simplifies the configuration, and provides advantage in maintenance.

Also, unlike protocols with non-deterministic response characteristics of general communications, fieldbuses guarantee data response speed to satisfy industrial applications where critical time characteristics are important.

![[Figure 1.3.8-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/image_1.png>)

<br>

One fieldbus network connects one master device and multiple slave devices.
The master device searches and manages the entire network and exchanges data with slave devices.

Generally, a PLC is a master device, while sensors, buttons, controllers, etc. can be configured as slave devices.
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md)
#### 1.3.8.1 CC-Link Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**CC-Link IO Mapping**

<br>

{% hint style="info" %}
   - CC-Link Version 1
{% endhint %}

<br>

![[Figure 1.3.8.1-1 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
   - CC-Link Version 2

   - Extension Cycle : Single
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
   - CC-Link Version 2

   - Extension Cycle : Double
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
   - CC-Link Version 2

   - Extension Cycle: Quadruple
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
   - CC-Link Version 2

   - Extension Cycle : Octuple
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_5.png>)

<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/2-Settings-CC-Link-Slave.md)
#### 1.3.8.2 CC-Link Slave Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   - For CC-Link connector connection, please refer to the following.

      ("[1.2.2 Connector](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. Using the TP, select CC-Link slave in the industrial communication PCI Slot settings and reboot the robot controller.**

![[Figure 1.3.8.4-1 PCI Slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.8.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > CC-Link Slave]**

![[Figure 1.3.8.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>) 

![[Figure 1.3.8.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
   [Station Address]

   - The CC-Link identifies the slave through the Station Address (1-64).
{% endhint %}

{% hint style="info" %}
   [Communication Speed (Baudrate)]

   - You can select from 156, 625, 2500, 5000, and 10000 Kbit/s.
{% endhint %}

{% hint style="info" %}
   [CC-Link Version]

   - Version 1: IO Station available, Extension Cycle not available

   - Version 2: IO Station not available, Extension Cycle available
{% endhint %}

{% hint style="info" %}
   [Occupied Station Count]

   - IO Station: Occupies 1

   - Remote Device: 1-4 selectable

   - The size of the assigned IO byte area varies depending on the number of stations occupied.
{% endhint %}

{% hint style="info" %}
   [Extension Cycle]

   - Available in Version 2

   - Remote Device: You can select from Single (1x), Double (2x), Quadruple (4x), and Octuple (8x).

   - The size of the assigned IO byte area varies depending on the Extension Cycle.
{% endhint %}

<br>

{% hint style="info" %}
   **For the IO Byte area, please refer to the link below.**

   **(["**1.3.8.1 CC-Link Slave Specifications](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md))**
{% endhint %}

<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.8.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_5.png>) 

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Error-CC-Link.md)
#### 1.3.8.3 CC-Link Slave Error Handling

<br>

Please refer to "[1.4.1 ERROR Code](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

<br>

**1. CC-Link termination resistor**

{% hint style="info" %}
   - A resistor should be added at the termination when connecting the CC-Link cable.

   - If communication is not connected, please check the termination resistor.

   - CC-Link termination resistor: 110 ohms
{% endhint %}

{% hint style="info" %}
   - As shown in the figure below, if the CIFX-50 CC PCI is at the CC-Link termination, please add a termination resistor.
{% endhint %}

![[Figure 1.3.8.5-1 CC-Link Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/5-Error/image_1.png>) 



**2. CC-Link ERROR**

{% hint style="info" %}
   - A 24V power supply to the CC-Link cable is required for communication connection.

   - If communication is not connected, please check the 24V power supply.
{% endhint %}

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/README.md)
### 1.3.9 CC-Link IE Field

This chapter describes the characteristics of CC-Link IE field slaves and how to set them. 


<br>

**Fieldbus Overview**

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

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/1-Specification-CC-Link-IE-Field-Slave.md)
#### 1.3.9.1 CC-Link IE Field Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

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

**Network Characteristics**

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

**Connection**

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
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/2-Settings-CC-Link-IE-Field-Slave.md)
#### 1.3.9.2 CC-Link IE Field Slave Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.


<br>

**1. Using the TP, select a CC-Link IE Field slave in the industrial communication PCI Slot settings and reboot the robot controller.**

![[Figure 1.3.9.2-1 PCI Slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_1.png>) 

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.9.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > CC-Link IE Field Slave]**

![[Figure 1.3.9.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>) 

![[Figure 1.3.9.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
   [Network Number]

   - CC-Link IE field network number (1-239)
{% endhint %}

{% hint style="info" %}
   [Station Address]

   - Device ID within the connected network (1-120)
{% endhint %}

{% hint style="info" %}
   [IO Type]

   - IO type is determined by the master device settings.   
      - Mixed: Input and output use different indexes (different addresses).   
      - Input: Input only   
      - Output: Output only   
      - FrontBackMixture: Input and output use the same index (same address).   
{% endhint %}

{% hint style="info" %}
   [Device Type]

   - The maximum IO size that can be set varies depending on the Device Type.

   - Intelligent Device Station   
      - RY, RX (max): 256 bytes   
      - RWw, RWr (max): 1024 words

   - Remote Device Station   
      - RY, RX (max): 16 bytes   
      - RWw, RWr (max): 64 words
{% endhint %}

{% hint style="info" %}
   [IO Size]

   - Master -> Slave
      - RWw (word data)
      - RY (bit data)

   - Slave -> Master   
      - RWr (word data)   
      - RX (bit data)  
{% endhint %}

<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}

<br>

![[Figure 1.3.9.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>) 
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/3-Error-CC-Link-IE-Field.md)
#### 1.3.9.3 CC-Link IE Field Slave Error Handling

<br>

Please refer to "[1.4.1 ERROR Code](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/README.md)
### 1.3.10 EtherNet/IP - Standard Remote IO Connection

<br>

This chapter explains how to connect several standard Remote IO modules selected by our company using the EtherNet/IP scanner (master).

<br>

{% hint style="info" %}
   - The EtherNet/IP scanner (master) uses the CIFX-50 real time Ethernet PCI.


   - Remote IO module uses the M9289 EtherNet/IP network adapter from Crevis.
{% endhint %}


[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)
#### 1.3.10.1 EtherNet/IP - Standard Remote IO Connection Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

**1. Select EtherNet/IP Master in the industrial communication PCI Slot settings and reboot the robot controller.**

![[Figure 1.3.10.1-1 PCI Slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>) 

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

![[Figure 1.3.10.1-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

**3. Connect the PCI and Remote IO cables, etc. for communication and check the status.**

![[Figure 1.3.10.1-3 Hardware Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[Figure 1.3.10.1-4 Hardware Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

<br>

{% hint style="info" %}
   - Please connect the PCI and Remote IO using a LAN cable.

   - Set all DIP switches of the Remote IO to OFF.

   - Connect both the Remote IO power and Field Power (24 V DC).
{% endhint %}

<br>

{% hint style="info" %}
   - The factory default IP of the Crevis M9289 Remote IO is 192.168.100.99.

   - The Remote IO IP should be set to 192.168.100.99 to enable communication connection.

   - "[1.3.10.2 Remote IO IP Setting](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

**4. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > EtherNet/IP Remote IO Setting]**

![[Figure 1.3.10.1-5 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>)

![[Figure 1.3.10.1-6 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>)

<br>

{% hint style="info" %}
   - The IP is set as a fixed value.

   - Check the input and output byte counts.

   - The selected input and output byte counts should be less than or equal to the IO byte counts of the card installed in the Remote IO slot.
{% endhint %}

<br>

{% hint style="info" %}
   - Input Module  
   - M12DF: Digital 16 points  
   - M3534: Analog 4 points  
{% endhint %}

{% hint style="info" %}
   - Output Module  
   - M225F: Digital 16 points  
   - M226F: Digital 16 points  
   - M2768: Digital 8 points   
   - M4534: Analog 4 points  
{% endhint %}

{% hint style="info" %}
   - Special Module  
   - M5112 : Conveyer I/F
{% endhint %}

<br>

**5. Reboot the controller after completing the settings.**

![[Figure 1.3.10.1-7 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>)

![[Figure 1.3.10.1-8 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
   - Please reboot the controller after completing the settings.
{% endhint %}

<br>

**6. After confirming that the setting values are reflected, check the communication status.**

![[Figure 1.3.10.1-9 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>)

For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.10.1-10 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>)

{% hint style="info" %}
   - If communication is not connected, you should check the Remote IO IP.

   - Please follow the steps below. (If not 192.168.100.99)

   - "[1.3.10.2 Remote IO IP Setting](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

![[Figure 1.3.10.1-11 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>) 

![[Figure 1.3.10.1-12 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>)

<br>

**7. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)
#### 1.3.10.2 Remote IO IP Address Settings

This is how to set the IP address of the M9289 EtherNet/IP network adapter from Crevis.

<br>

{% hint style="info" %}
   - The factory default IP of the Crevis M9289 Remote IO is 192.168.100.99.

   - If you do not know the Remote IO IP or need to change it, please follow the steps below.
{% endhint %}

<br>

**1. Connect the PC and Remote IO directly using a LAN cable.**

![[Figure 1.3.10.2-1 LAN Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

**2. Change only DIP switch 9 of the Remote IO Adapter to ON.**

![[Figure 1.3.10.2-2 DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

**3. Execute the Bootpsvr.exe program.**
   * This program is provided by Crevis. (Download and install IO Guide Pro from the website.)

![[Figure 1.3.10.2-3 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[Figure 1.3.10.2-4 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
   - With Start BootP being pressed, disconnect and reapply power to the M9289 module to reboot it.
{% endhint %}

![[Figure 1.3.10.2-5 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>


**4. When the adapter device is rebooted, the device information will appear in the BootpSvr.exe program.**

![[Figure 1.3.10.2-6 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

**5. Select the device and set the IP.**

![[Figure 1.3.10.2-7 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[Figure 1.3.10.2-8 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

**6. After completing the IP setting, turn all DIP switches of the adapter to OFF and reboot the device.**

{% hint style="info" %}
   - Be sure to check the DIP switch status and whether the adapter is rebooted.
{% endhint %}

![[Figure 1.3.10.2-9 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

**7. Use the ping test, etc. on the PC to verify the IP.**

![[Figure 1.3.10.2-10 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

**8. If the IP address has been changed successfully, proceed with settings.**

{% hint style="info" %}
   - Please proceed with the settings according to the "[1.3.10.1 EtherNet/IP - Standard Remote IO Connection Settings](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)" procedure.
{% endhint %}

[__SOURCE](1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)
## 1.4 CIFX PCI Communication Monitoring

<br>

After setting the communication according to the procedures of "[1.2 CIFX PCI - Installing and Setting Industrial Communication Cards](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" and "[1.3 CIFX PCI - Setting Industrial Communication](../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)," you can check the operations in the following screens.

<br>

**1. Industrial Communication Monitoring**

<br>

You can enter the screens by touching **\[Service > 19: Industrial Communication Monitoring]**, and check the details such as the set PCI Slot information, communication status, and communication configuration in relevant screens.

<br>

{% hint style="info" %}
   - Using the **\[Restart]** button, you can restart the industrial communication of the PCI communication card.

   - Please check the status of the slot, PCI Slot, and device.

   - For the master, check whether the number of the configured and active slaves matches the number of configured slaves.
{% endhint %}

<br>

![[Figure 1.4-1 Industrial Communication Monitoring]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_1.png>)

<br>

{% hint style="info" %}
   [Status Information]   
      - Communication: Communication link established and I/O data exchanging   
      - Run: Communication card (PCI) is operating   
      - Ready: Communication is in standby state   
      - Error: Communication error state   

      - Communication Error: Error code occurred during communication   
      - Error Count: Accumulated number of communication errors   
      - Active Slaves: Number of slaves currently connected and exchanging I/O data   
      - Configured Slaves: Number of slaves configured for communication   
      - Diag Slave: Number of slaves under communication diagnostics   
      - Watchdog Time (ms): Timeout value for monitoring communication program activity   
{% endhint %}

<br>

**2. Industrial Communication Node Monitoring**

<br> 

Click the Node Statue button at the bottom of the monitoring screen to monitor the status of devices connected to the master protocol

<br>

![[그림 1.4-2 Industrial Communication Monitoring]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_2.png>)

{% hint style="info" %}
   [Node Status Information]   
      - Green: Node currently connected and exchanging I/O data   
      - Red: Node configured but not connected   
{% endhint %}

<br>

{% hint style="info" %}
   - In the case of DeviceNet Master, you can monitor by scanning the node information list
{% endhint %}

<br>

![[그림 1.4-3 Industrial Communication Monitoring]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_3.png>)
[__SOURCE](1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)
### 1.4.1 ERROR Code

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


[__SOURCE](2-ethernet-ip/README.md)
# 2. EtherNet/IP

This chapter describes the characteristics and configuration methods of the built-in EtherNet/IP Master (Scanner) and Slave (Adapter).
<br>

**EtherNet/IP Overview**

<br>

EtherNet/IP is an Ethernet-based open industrial communication protocol developed by CI (ControlNet International) and ODVA (Open DeviceNet Vendors Association)

In a factory environment, various devices such as sensors, remote I/Os, motor drivers, HMIs, PLCs and robot controllers can be connected to a single EtherNet/IP network, regardless of the manufacturer.

![[Figure 2-1 EtherNet/IP]](<../_assets//2-ethernet-ip/image_1.png>)
 

<br>

EtherNet/IP is classified as follows based on its communication functions:

**Scanner Class**

   * These products correspond to traditional Fieldbus Masters and can request I/O data connections from EtherNet/IP Adapters or Scanners.

<br>

**Adapter Class**

  * These products correspond to traditional Fieldbus Slaves and serve as the connection targets for real-time I/O data requested by an EtherNet/IP Scanner.
    
  * An Adapter cannot transmit or receive real-time I/O data on its own without a request from a Scanner.

<br>

**Messaging Class**

   * These products are capable of sending and receiving explicit messages to and from products of all classes, but they do not support real-time I/O data transmission.
   
   * Examples include computer interface cards for program upload/download and network configuration tools.

<br>

**Abbreviation**

<br>

|Abbreviation|Description|
|---------------|------------------------------|
|Adapter|A device that collects output data from and transmits input data to an EtherNet/IP Scanner|
|Scanner|A device that sends output data to and collects input data from end devices (EtherNet/IP Adapters)|
|LAN| Local Area Network|
|RPI|Requested Packet Interval|
|PLC|Programmable logic controller|
|T2O|Target to Originator (Adapter -> Scanner)|
|O2T|Originator to Target (Scanner -> Adapter)|

[__SOURCE](2-ethernet-ip/1-network.md)
## 2.1 Network Settings

**1. Main Module**

<br>

The LAN ports that can connect with the EtherNet/IP adapter are LAN1/LAN2/LAN3.

<br>

![figure 2.1-1 Main Module](../_assets/2-ethernet-ip/1-network/hi6com.png)

<br>

**2. Network Settings**

<br>

Select a LAN port to connect EtherNet/IP communication and then check the settings of the LAN port through the TP screen as shown below and change the settings as needed.

<br>

![figure 2.1-2 Network configuration](../_assets/2-ethernet-ip/1-network/networkConfig.png)

<br>

{% hint style="info" %}
   - The subnet portion of each IP address of LAN1/LAN2/LAN3 should be set differently.

   - After changing the settings, reboot the robot controller.
{% endhint %}

<br>

**3. Connection Status Check**

<br>

The status of the physical connection with the EtherNet/IP scanner can be checked according to the status of the Link/Act LED of the LAN port.

<br>

Connect the EtherNet/IP adapter and scanner with a LAN cable and then check the LED status. If the LED on the left does not light up or blink, it means there is a problem with the cable or adapter or scanner device. Please check the connection status of the cable or device.

<br>

![figure 2.1-3 LAN Port](../_assets/2-ethernet-ip/1-network/lanPort.png)

<br>

**4. Network Configuration**

<br>

It is recommended to configure the EtherNet/IP Network and Factory Network as separate networks. As shown in the figure below, if you configure the EtherNet/IP Network and Factory Network as one network, they will share one transmission medium, increasing the network load. Therefore, it is recommended to use a separately configured network for the EtherNet/IP Network if possible.

<br>

![figure 2.1-4 Network](../_assets/2-ethernet-ip/1-network/NG_Network.png)

<br>

![figure 2.1-5 Network](../_assets/2-ethernet-ip/1-network/Good_Network.png)

<br>

[__SOURCE](2-ethernet-ip/2-license.md)
## 2.2 License Settings

**1. License Activation**

<br>

On the initial screen, navigate to "System" > "2: Control Parameters" > "10: License Key Registration for Optional Functions"

<br>

![figure 2.2-1 license](../_assets/2-ethernet-ip/2-license/license.png)

<br>

1. Deliver the system serial number to the license administrator
2. Obtain the license key from the administrator, enter it, and press the "Confirm" button
3. License Key [XXXXXX] ==>OK Confirm
4. Select "Valid" for the "Embedded EtherNet/IP slave" or "Embedded EtherNet/IP master" from the license list.

<br>

{% hint style="info" %}
   [EtherNet/IP Licensing Policy]

   - Slave License : Supports EtherNet/IP Slave only

   - Master License : Supports both EtherNet/IP Master and Slave
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/3-adapter/README.md)
## 2.3 EtherNet/IP Adapter (Slave)

<br>

This section provides an overview and instructions for the built-in EtherNet/IP Adapter (Slave)

<br>


[__SOURCE](2-ethernet-ip/3-adapter/1-specification.md)
### 2.3.1 EtherNet/IP Adapter Specifications (Slave)


<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th colspan=2, class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
    <tr>
        <td>Connection</td>
        <td>O (Master) -> T (Slave)</td>
		<td>T (Slave) -> O (Master)</td>
	</tr>
    <tr>
        <td>Maximum IO Size</td>
        <td>240 bytes</td>
		<td>240 bytes</td>
	</tr>
    <tr>
        <td>Instance No.</td>
        <td>112 (0x70)</td>
		<td>100 (0x64)</td>
	</tr>
    <tr>
        <td>Real-Time Transfer Format</td>
        <td>32-bit run/idle header</td>
		<td>None</td>
	</tr>
	<tr>
        <td>Connection Type</td>
        <td>Point to Point</td>
		<td>Point to Point</td>
	</tr>
	<tr>
        <td>Priority</td>
        <td>Scheduled</td>
		<td>Scheduled</td>
	</tr>
    <tr>
		<td>IO Cycle Time (RPI)</td>
		<td colspan=2>Min. 5ms</td>
	</tr>
    <tr>
		<td>Device Type</td>
		<td colspan=2>General Purpose Discrete I/O</td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td colspan=2>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td colspan=2>Not supported</td>
	</tr>
    <tr>
		<td >IP Allocation Method</td>
		<td colspan=2>Static IP Address</td>
	</tr>
</tbody>
</table>
<br>

**Network Characteristics**

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

**Connection**

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
[__SOURCE](2-ethernet-ip/3-adapter/2-settings.md)
### 2.3.2 EtherNet/IP Adapter (Slave) Settings

<br>

**1. EtherNet/IP Adapter Settings and Monitoring via Teaching Pendant**

<br>

**\[System > 2: Control Parameter > 11: Industrial Communication > 3: EtherNet/IP Settings]**

<br>

![Config.PNG](../../_assets/2-ethernet-ip/3-adapter/Config.png)<br>

<br>

{% hint style="info" %}
   [Protocol Settings]

      - OFF : EtherNet/IP disable   
      - Adapter : EtherNet/IP Adapter mode   
      - Scanner : EtherNet/IP Scanner mode   
      - Adapter + Scanner : EtherNet/IP Adapter + Scanner mode   
{% endhint %}

<br>

{% hint style="info" %}
   [Port Settings]

      - General-purpose controller LAN1 to LAN3 are available (Ensure the status is "OK")
{% endhint %}

<br>

{% hint style="info" %}
   [IO Size]

      -	Input Byte Count: 0-240 can be set.   
      -	Output Byte Count: 0-240 can be set.
{% endhint %}   

<br>

{% hint style="info" %}
   [Communication Status Check]   

      - License: Current license status   
      - Run: Indicates the operational status of the EtherNet/IP function   
      - Communication: Indicates the EtherNet/IP connection status   
      - Error: Indicates the EtherNet/IP error status    
{% endhint %}

[__SOURCE](2-ethernet-ip/3-adapter/3-connect-scanner/README.md)
### 2.3.3 Connecting External Scanner Devices

<br>

This section explains how to connect the external EtherNet/IP Scanner to the EtherNet/IP Adapter.
[__SOURCE](2-ethernet-ip/3-adapter/3-connect-scanner/1-connect-ls-plc.md)
#### 2.3.3.1 LS ELECTRIC PLC

<br>

This section explains how to connect the LS ELECTRIC PLC with EtherNet/IP.  
The PLC and communication module used below are as follows.  
(PLC: XGI-CPUS, Communication Module: XGL-EFMTB)

<br>

**1. XG5000 Running**

<br>

![xg5000.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/xg5000.png)

<br>

For downloading the XG5000 program and detailed usage methods, please refer to the LS ELECTRIC website.

<br>

**2. EDS File Registration**

<br>

Click Menu > Tools > EDS(D) > EDS File Registration, and then select "Hi7_EIP_251023.eds"
Confirm EDS file registration as shown in the figure below.

<br>

![eds.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/eds.png)

<br>

**3. Device Connection**

<br>

[1] Create a project.<br>
![newProject_1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_1.png)<br>

[2] Add a communication module.<br>
![newProject_2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_2.png)<br>

![newProject_3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_3.png)<br>

![newProject_4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_4.png)<br>

<br>

[3] Set a communication module <br>
Double-click XGL-EFMT shown in the left tab in the figure below.<br>
![newProject_6.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_6.png)

<br>

- Set the IP address, subnet mask, gateway, etc.  
- To use the two LAN ports of the PLC as a relay function, select the "Relay" checkbox.  
- Change the RAPIEnet setting to Disable.

<br>

**4. Online Connection Settings**

<br>

[1] Connect the PLC with a USB cable.<br>
![newProject_7.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_7.png)<br>

[2] Press the button shown on the left in the figure below to download the entire settings.<br>
![newProject_8.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_8.png)<br>

<br>

**5. Auto Scan**

<br>

[1] Auto Scan is possible when connected to the PLC.<br>
If the current state is not online, click Menu > Online > Connect to change to online status.<br>

[2] Right-click XGL-EFMT > Add Item > Smart Expansion<br>
![auto1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto1.png)<br>

[3] Click Next. <br>
![auto2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto2.png)<br>

[4] Click Auto Scan. <br>
![auto3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto3.png)<br>

![auto4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto4.png)<br>

[5] Check the automatically scanned devices.  
![auto5.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto5.png)<br>

![auto6.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto6.png)<br>

The Hi7 EtherNet/IP adapter device appears in the list as shown in the figure below. <br>
![auto7.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto7.png)<br>

<br>

**6. Program Variable Registration**

<br>

[1] Scan Program > NewProgram > Local Variables (double-click)<br>
![variable1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/variable1.png)<br>

[2] Set the input/output data to be used in communication.<br>
![variable2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/variable2.png)<br>

<br>

**7. EtherNet/IP Adapter Settings**

<br>

[1] Double-click EB01 (Hi7 EtherNet/IP adapter) in the list on the left.<br>

[2] Press the EIP detailed settings button.<br>
![AdapterSetting1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting1.png)<br>

[3] Refer to the figure below to select the setting values for the EtherNet/IP adapter. <br>
- Connection type
- T2O RPI Range, O2T RPI Range
- T2O Input, O2T Output size
- Transmission cycle
- Timeout
- Local tag, Remote tag <br>
![AdapterSetting2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting2.png) <br>

[4] Click Online > Communication Module Settings and Diagnostics > Service Enable.<br>
![AdapterSetting3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting3.png)<br>

[5] Check the FEnet I/O Service checkbox.<br>
![AdapterSetting4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting4.png)<br>

<br>

**8. Assignment of IO Blocks after Completion of Communication Settings**

<br>

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](2-ethernet-ip/3-adapter/4-error_code.md)
### 2.3.4 Error Code

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




[__SOURCE](2-ethernet-ip/4-scanner/README.md)
## 2.4 EtherNet/IP Scanner (Master)

<br>

This section provides an overview and instructions for the built-in EtherNet/IP Scanner (Master)

<br>

[__SOURCE](2-ethernet-ip/4-scanner/1-specification.md)
### 2.4.1 EtherNet/IP Scanner (Master) Specifications

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=2, class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td colspan=2>Maximum Connectable Slave Count</td>
		<td>20</td>
	</tr>
    <tr>
		<td rowspan=2>IO Size</td>
        <td>Maximum I/O Size</td>
		<td>Max 1200 bytes</td>
	</tr>
    <tr>
        <td>Maximum I/O Size (1 slave)</td>
		<td>Max 240 bytes</td>
	</tr>
    <tr>
		<td colspan=2>IO Connection</td>
		<td>Cyclic</td>
	</tr>
    <tr>
		<td colspan=2>IO Update Time</td>
		<td>Min. 5ms</td>
	</tr>
    <tr>
		<td colspan=2>Communication Speed</td>
		<td>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td colspan=2>Quick Connect</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td colspan=2>Topology</td>
		<td>Tree, Line</td>
	</tr>
    <tr>
		<td colspan=2>IP Allocation Method</td>
		<td>Static IP Address</td>
	</tr>
</tbody>
</table>
<br>

**Network Characteristics**

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

**Connection**

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
[__SOURCE](2-ethernet-ip/4-scanner/2-settings.md)
### 2.4.2 EtherNet/IP Scanner (Master) Settings

<br>

After completing the procedures in "[2.1 Network Settings](../../2-ethernet-ip/1-network.md)" and "[2.2 License Settings](../../2-ethernet-ip/2-license.md)" please proceed with the following steps.

<br>

**1. Touch the menu to enter the settings screen.**

<br>

**\[System > 2: Control Parameter > 11: Industrial Communication > 3: EtherNet/IP Settings]**

<br>

![[figure 2.4.2-1 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_1.png>) 

<br>

![[figure 2.4.2-2 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_2.png>) 

<br>

{% hint style="info" %}
   [Protocol Settings]

      - OFF : EtherNet/IP disable   
      - Adapter : EtherNet/IP Adapter mode   
      - Scanner : EtherNet/IP Scanner mode   
      - Adapter + Scanner : EtherNet/IP Adapter + Scanner mode   
{% endhint %}

<br>

{% hint style="info" %}
   [Port Settings]

      - General-purpose controller LAN1 to LAN3 are available (Ensure the status is "OK")
{% endhint %}

<br>

**2. Select "Scanner" mode and click the "Add Device" button to proceed to the next screen.**

<br>

![[figure 2.4.2-3 Scanner Add Device]](<../../_assets/2-ethernet-ip/4-scanner/img_3.png>) 

<br>

**3. Enter the settings to match the target device and save.**

<br>

{% hint style="info" %}
   [Device Settings]

      - Device No. : Device connection order (sequence of I/O data allocation)   
      - IP Address : IP address of the device   
      - Device Name : Name of the device (for identification purposes only; does not affect communication)   
      - RPI (ms) : Requested Packet Interval (I/O data update cycle)   
      - Connection Type   
            - Exclusive Owner (I/O) : Establishes a bidirectional I/O connection between the Scanner and Adapter   
            - Input Only : Connects to the Adapter's input signals only   
            - Listen Only : Connects to the input signals only while the Adapter is already connected to another Scanner   

      - Input (T > O) : Slave > Master connection   
      - Output (O > T) : Master > Slave connection   

      - Run/Idle Header : Select whether to include the I/O data header   
      - Instance No. : Instance number of the Input/Output Assembly for I/O data exchange   
      - IO Size : Size of I/O data (in bytes)   
{% endhint %}

<br>

{% hint style="info" %}
   - For connection examples, please refer to the manuals below.    
   - "[2.4.3.1 Connecting External Adapter Devices - Crevis Remote IO](3-connect-adapter/1-crevis.md)"

   - "[2.4.3.2 Connecting External Adapter Devices - Wago Remote IO](3-connect-adapter/2-wago.md)"

   - "[2.4.3.3 Connecting External Adapter Devices - Hilscher CIFX PCI EtherNet/IP Adapter](3-connect-adapter/3-pci.md)"

   - "[2.4.3.4 Connecting External Adapter Devices - Baumer OM-70](3-connect-adapter/4-baumer.md)"  
{% endhint %}

<br>

![[figure 2.4.2-4 Scanner Add Device]](<../../_assets/2-ethernet-ip/4-scanner/img_4.png>) 

<br>

**4. Click the "OK" button to transmit the communication settings.**

<br>

![[figure 2.4.2-5 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_5.png>) 

<br>

**5. Check the status to verify if the communication is successfully established.**

<br>

![[figure 2.4.2-6 Communication Status]](<../../_assets/2-ethernet-ip/4-scanner/img_6.png>) 

<br>

{% hint style="info" %}
   [Communication Status Check]   

      - License: Current license status   
      - Run: Indicates the operational status of the EtherNet/IP function   
      - Communication: Indicates the EtherNet/IP connection status   
      - Error: Indicates the EtherNet/IP error status    
{% endhint %}

<br>

{% hint style="info" %}
   [Device Number Color]   

      - Green: Communication connection OK   
      - Red: Communication connection NG (Failed)   
{% endhint %}

<br>

![[figure 2.4.2-7 Communication Status]](<../../_assets/2-ethernet-ip/4-scanner/img_7.png>) 

<br>

**6. After completing the communication settings, allocate the I/O Blocks.**

{% hint style="info" %}
   **After the communication settings are complete, you can use the input/output signals by allocating I/O Blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../5-io-block-allocation.md)")**
{% endhint %}
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/README.md)
### 2.4.3 Connecting External Adapter Devices

<br>

<style type="text/css">
table  {border-collapse:collapse;}
.sm-font-table th, .sm-font-table td {font-size:9px;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Configuration Values for Connecting External Adapter Devices**

<br>

{% hint style="info" %}
   - Please set the IO size to match the Input/Output size configured on the external device.   
{% endhint %}

<br>

{% hint style="info" %}
   - For detailed specifications, please refer to the manual provided by the device manufacturer    
{% endhint %}

<br>

<table class="tg sm-font-table">
<thead>
	<tr>
    	<th rowspan=2, class='powderblued'>Maker</th>
		<th rowspan=2, class='powderblued'>Product</th>
		<th rowspan=2, class='powderblued'>Connection Type</th>
        <th colspan=2, class='powderblued'>T -> O</th>
        <th colspan=2, class='powderblued'>O -> T</th>
        <th colspan=5, class='powderblued'>Additional Configuration</th>
	</tr>
    <tr>
        <th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Run Idle Header</th>
        <th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Run Idle Header</th>
		<th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Total Size</th>
		<th class='powderblued'>Data Size</th>
        <th class='powderblued'>Data Type</th>
		<th class='powderblued'>Data</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Crevis</td>
		<td>M9289</td>
        <td>Exclusive Owner</td>
		<td>1</td>
		<td>No</td>
        <td>2</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Wago</td>
		<td>750-366</td>
        <td>Exclusive Owner</td>
		<td>104: Status + AI + DI<br>105: Status + DI<br>106: Status + AI<br>107: AI + DI<br>108: DI<br>109: AI</td>
		<td>No</td>
        <td>101: AO + DO<br>102: DO<br>103: AO</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Hilscher</td>
		<td>CIFX PCI EtherNet/IP Adapter</td>
        <td>Exclusive Owner</td>
		<td>101</td>
		<td>Yes</td>
        <td>100</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Baumer</td>
		<td>OM-70 EtherNet/IP</td>
        <td>Input Only</td>
		<td>100</td>
		<td>No</td>
        <td>238</td>
		<td>-</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Beckhoff</td>
		<td>EK-9500</td>
        <td>Exclusive Owner</td>
		<td>129</td>
		<td>No</td>
        <td>130</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
	<tr>
		<td rowspan=6>Rockwell Automation (AB)</td>
		<td rowspan=6>Point I/O 1734-AENTR</td>
        <td rowspan=6>Exclusive Owner</td>
		<td rowspan=6>101</td>
		<td rowspan=6>No</td>
        <td rowspan=6>100</td>
		<td rowspan=6>Yes</td>
		<td rowspan=6>102</td>
		<td rowspan=6>10</td>
		<td>4byte</td>
		<td>unsigned int</td>
		<td>1</td>
	</tr>
	<tr>
		<td>2byte</td>
		<td>unsigned int</td>
		<td>IO slot + 1</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(T -> O) Alignment<br>0: bytes<br>2: word<br>4: Dword<br>255: Fixed</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(T -> O) Fixed Size per Slot</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(O -> T) Alignment<br>0: bytes<br>2: word<br>4: Dword<br>255: Fixed</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(O -> T) Fixed Size per Slot</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis.md)
#### 2.4.3.1 Connecting External Adapter Devices - Crevis Remote IO

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[Download EDS File Tool (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - For the IP settings of the Remote I/O used in the example, please refer to the manual link below.

   - "[1.3.10.2 Remote IO IP Setting](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

![[figure 2.4.3.1-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_1.png>) 

<br>

![[figure 2.4.3.1-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_2.png>) 

<br>

![[figure 2.4.3.1-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_3.png>) 

<br>

**2. Open the EDS file using the EZ-EDS program and verify the device information.**

<br>

![[figure 2.4.3.1-4 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_4.png>) 

<br>

{% hint style="info" %}
   - Check the connection type in the Connection Manager   
      - Example: Exclusive Owner

   - Check for the presence of headers in the Real Time Transfer Format   
      - Input (T > O) : No header   
      - Output (O > T) : 32-bit run/idle header   

   - Click "Create / Decode Path" to verify the Instance ID   
{% endhint %}

<br>

![[figure 2.4.3.1-5 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_5.png>) 

<br>

{% hint style="info" %}
      - Input (T > O) : 1   
      - Output (O > T) : 2   
{% endhint %}

<br>

**3. Check the I/O size in the device manual.**

<br>

{% hint style="info" %}
   - Verify the I/O configuration of the device to be connected. 
{% endhint %}

<br>

![[figure 2.4.3.1-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_6.png>) 

<br>

{% hint style="info" %}
   - Refer to the manual for each slot configuration to determine the total I/O size.
{% endhint %}

<br>

![[figure 2.4.3.1-7 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_7.png>) 

<br>

![[그림 2.4.3.1-8 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_8.png>) 

<br>

**4. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.1-8 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_9.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the settings correctly.   
      - Input (T > O) : Slave > Master   
      - Output (O > T) : Master > Slave   

   [Adapter Configuration]   
   - Crevis M9289   
      - M7002 : None   
      - M2768 : 1byte (O > T)   
      - M2768 : 1byte (O > T)   
      - M12DF : 2bytes (T > O)   
      - M12DF : 2bytes (T > O)   
      - M2768 : 1byte (O > T)   
      - M2768 : 1byte (O > T)   

   [IO Assembly Information]   
   [T > O]   
      - Size: 4bytes   
      - Instance: 1   
      - Run/Idle Header: No   

   [O > T]    
      - Size: 4bytes   
      - Instance: 2   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/2-wago.md)
#### 2.4.3.2 Connecting External Adapter Devices - Wago Remote IO

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[Download EDS File Tool (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - Please refer to the Wago manual for the IP configuration of the device.
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

![[figure 2.4.3.2-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_1.png>) 

<br>

**2. Check the Instance ID provided in the device manual**

<br>

![[figure 2.4.3.2-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_2.png>) 

<br>

{% hint style="info" %}
   - Input (T > O)   
      - 104: Status  + Analog  + Digital   
      - 105: Status  + Digital   
      - 106: Status  + Analog   
      - 107: Analog  + Digital   
      - 108: Digital   
      - 109: Analog   

   - Output (O > T)   
      - 101: Analog + Digital   
      - 102: Digital   
      - 103: Analog   
{% endhint %}

<br>

**3. Open the EDS file using the EZ-EDS program and verify the device information.**

<br>

![figure 2.4.3.2-3 EDS Info](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_3.png>) 

<br>

{% hint style="info" %}
   - Check the connection type in the Connection Manager   
      - Example: Exclusive Owner

   - Check for the presence of headers in the Real Time Transfer Format   
      - Input (T > O) : No header   
      - Output (O > T) : 32-bit run/idle header   
{% endhint %}

<br>

**4. Check the I/O size in the device manual.**

<br>

{% hint style="info" %}
   - Verify the I/O configuration of the device to be connected. 
{% endhint %}

<br>

![[figure 2.4.3.2-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_4.png>) 

<br>

{% hint style="info" %}
   - Refer to the manual for each slot configuration to determine the total I/O size.
{% endhint %}

<br>

![[figure 2.4.3.2-5 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_5.png>) 

<br>

![[figure 2.4.3.2-6 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_6.png>) 

<br>

**5. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.2-7 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_7.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the settings correctly.   
      - Input (T > O) : Slave > Master   
      - Output (O > T) : Master > Slave   

   [Adapter Configuration]   
   - Wago 750-366   
      - Status 1byte (T > O) (When selecting Instance ID 104, 105, 106)   
      - 753-436 : 1byte (T > O)   
      - 753-536 : 1byte (O > T)   

   [IO Assembly Information]   
   [T > O]   
      - Size: 2bytes   
      - Instance: 105   
      - Run/Idle Header: No   

   [O > T]    
      - Size: 1bytes   
      - Instance: 101   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/3-pci.md)
#### 2.4.3.3 Connecting External Adapter Devices - Hilscher CIFX PCI EtherNet/IP Adapter

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[Download EDS File Tool (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - Please refer to the Hilscher manual for the IP configuration of the device.
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

![[figure 2.4.3.3-1 CIFX PCI]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_1.png>) 

<br>

**2. Open the EDS file using the EZ-EDS program and verify the device information.**

<br>

![[figure 2.4.3.3-2 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_2.png>) 

<br>

{% hint style="info" %}
   - Check the connection type in the Connection Manager   
      - Example: Exclusive Owner

   - Check for the presence of headers in the Real Time Transfer Format   
      - Input (T > O) : 32-bit run/idle header   
      - Output (O > T) : 32-bit run/idle header   
{% endhint %}

<br>

![[figure 2.4.3.3-3 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_3.png>) 

<br>

{% hint style="info" %}
   - Check the Instance ID in Param   
      - Input (T > O) : 101   
      - Output (O > T) : 100   
{% endhint %}

<br>

**3. Check the I/O size in the device manual.**

<br>

{% hint style="info" %}
   - Check the I/O Size of the current device to be connected (Refer to the corresponding PCI device settings)   
{% endhint %}

<br>

**4. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.3-4 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_4.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the settings correctly.   
      - Input (T > O) : Slave > Master   
      - Output (O > T) : Master > Slave   

   [IO Assembly Information]   
   [T > O]   
      - Size: 240 bytes (Value configured in the PCI device)   
      - Instance: 101   
      - Run/Idle Header: 32Bit   

   [O > T]    
      - Size: 240 bytes (Value configured in the PCI device)   
      - Instance: 100   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer.md)
#### 2.4.3.4 Connecting External Adapter Devices - Baumer OM-70

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[Download EDS File Tool (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - Please refer to the Baumer manual for the IP configuration of the device.
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

![[figure 2.4.3.4-1 Baumer OM-70]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_1.png>) 

<br>

**2. Verify the Instance ID and I/O Size in the device manual.**

<br>

![[figure 2.4.3.4-2 Baumer OM-70]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_2.png>) 

<br>

{% hint style="info" %}
   [Input Only Connection]   

   - Input (T > O)   
      - Instance ID: 100   
      - Size : 34 bytes   

   - Output (O > T)   
      - Instance ID: 238   
      - Size : 0 byte    
{% endhint %}

<br>

**3. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.4-3 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_3.png>)

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff.md)
#### 2.4.3.5 Connecting External Adapter Devices - Beckhoff Remote IO

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[Download EDS File Tool (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - Please refer to the Beckhoff manual for the IP configuration of the device.
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

![[figure 2.4.3.5-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_1.png>) 

<br>

**2. Access the device's webpage to configure the IP address.**

<br>

{% hint style="info" %}
   - In this example, the initial IP address is set to 192.168.1.2 (DIP switch No. 2 is ON)
{% endhint %}

<br>

![[figure 2.4.3.5-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_2.png>) 

<br>

![[figure 2.4.3.5-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_3.png>) 

<br>

{% hint style="info" %}
   - In this example, the IP address is changed to 192.168.10.95. 

   - After entering the IP address, click the Check button to save. 
{% endhint %}

<br>

![[figure 2.4.3.5-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_4.png>) 

<br>

{% hint style="info" %}
   - Set the DIP switches as shown below and reboot the device:   
      - 1 ~ 8  : ON   
      - 9 ~ 10 : OFF   
{% endhint %}

<br>

![[figure 2.4.3.5-5 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_5.png>) 

<br>

![[figure 2.4.3.5-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_6.png>) 

<br>

**3. Access the device's webpage to verify the EtherNet/IP configuration information.**

<br>

{% hint style="info" %}
   - Re-access the webpage using the newly configured IP address and verify the IP address and EtherNet/IP configuration details.
{% endhint %}

<br>

![[figure 2.4.3.5-7 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_7.png>) 

<br>

![[figure 2.4.3.5-8 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_8.png>) 

<br>

{% hint style="info" %}
   - Input (T > O)   
      - Instance ID: 129   
      - Byte Size: 6      

   - Output (O > T)   
      - Instance ID: 130   
      - Byte Size: 6   
{% endhint %}

<br>

**4. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.5-9 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_9.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the settings correctly.   
      - Input (T > O) : Slave > Master    
      - Output (O > T) : Master > Slave   

   [Adapter Configuration]   
   - Beckhoff EK-9500   
      - EK-1008 : 1byte (T > O)   
      - EK-2008 : 1byte (O > T)   

   [IO Assembly Information]   
   [T > O]   
      - Size: 6bytes   
      - Instance: 129   
      - Run/Idle Header: No   

   [O > T]    
      - Size: 6bytes   
      - Instance: 130   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell.md)
#### 2.4.3.6 Connecting External Adapter Devices - Rockwell Automation (AB) Remote IO

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[Download EDS File Tool (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - Please refer to the Rockwell Automation manual for the IP configuration of the device.
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

<br>

![[figure 2.4.3.6-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_1.png>) 

<br>

![[figure 2.4.3.6-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_2.png>) 

<br>

**2. Open the EDS file using the EZ-EDS program and verify the device information.**

<br>

![[figure 2.4.3.6-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_3.png>) 

<br>

![[figure 2.4.3.6-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_4.png>) 

<br>

{% hint style="info" %}
   - Check the connection type in the Connection Manager   
      - Example: Exclusive Owner

   - Check for the presence of headers in the Real Time Transfer Format   
      - Input (T > O) : No header   
      - Output (O > T) : 32-bit run/idle header   

   - Click "Create / Decode Path" to verify the Instance ID   
      - Input (T > O) : 101   
      - Output (O > T) : 100   
      - Configuration : 102   
{% endhint %}

<br>

**3. Check the I/O size in the device manual.**

<br>

{% hint style="info" %}
   - Verify the I/O configuration of the device to be connected. 
{% endhint %}

<br>

![[figure 2.4.3.6-5 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_5.png>) 

<br>

{% hint style="info" %}
   - Verify the I/O configuration of the device to be connected. 
{% endhint %}

<br>

![[figure 2.4.3.6-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_6.png>) 

<br>

![[figure 2.4.3.6-7 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_7.png>) 

<br>

**4. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.6-8 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_8.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the settings correctly.   
      - Input (T > O) : Slave > Master    
      - Output (O > T) : Master > Slave    

   [Adapter Configuration]   
   - Point I/O 1734-AENTR    
      - Status : 8byte (T > O)    
      - 1734-IB8 : 1byte (T > O)   
      - 1734-OB8E : 1byte (O > T) + 1byte (T > O, Status)   

   [IO Assembly Information]   
   [T > O]   
      - Size: 10bytes   
      - Instance: 101   
      - Run/Idle Header: No   

   [O > T]    
      - Size: 1byte   
      - Instance: 100   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>

![[figure 2.4.3.6-9 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_9.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the additional settings correctly.   
      - Input (T > O) : Slave > Master   
      - Output (O > T) : Master > Slave   

   [Additional Settings]   
      - Config Segment : ON   
      - Instance: 102   
      - Size: 10bytes    

   [Config Segment Information]    
      - (4bytes) 1 : Header    
      - (2bytes) 3 : Connected Slots + 1   
      - (1byte)  0 : T > O Alignment (in bytes)      
      - (1byte)  1 : T > O Data Size per slot      
      - (1byte)  0 : O > T Alignment (in bytes)      
      - (1byte)  1 : O > T Data Size per slot      
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/4-error.md)
### 2.4.4 Error Codes

<br>

{% hint style="info" %}
   - Provides a real-time diagnostic function by displaying the communication status of each device using CIP standard General Status codes.
{% endhint %}

<br>

![[figure 2.4.4-1 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_8.png>) 

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**General Status Codes**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Status Value (Hex)</th>
		<th class='powderblued'>Name</th>
		<th class='powderblued'>Description</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>-</td>
		<td>Communication not configured or changed</td>
		<td>Communication settings have not been applied or are in the process of changing</td>
	</tr>
	<tr>
		<td>0x00</td>
		<td>Success</td>
		<td>The service has successfully been performed by the specified
object.</td>
	</tr>
	<tr>
		<td>0x00 (In case of error)</td>
		<td>No reponse</td>
		<td>No communication response (e.g., cable disconnected, invalid IP address, etc.)</td>
	</tr>
	<tr>
		<td>0x01</td>
		<td>Connection failed</td>
		<td>A connection-elated service failed. This happened at any
location along the connection path.</td>
	</tr>
	<tr>
		<td>0x02</td>
		<td>Resource unavailable</td>
		<td>Some resources which were required for the object to perform
the requested service were not available.</td>
	</tr>
	<tr>
		<td>0x03</td>
		<td>Invalid parameter value</td>
		<td>See status code 0x20, which is usually applied in this situation.</td>
	</tr>
	<tr>
		<td>0x04</td>
		<td>Path segment error</td>
		<td>A path segment error has been encountered. Evaluation of the
supplied path information failed.</td>
	</tr>
	<tr>
		<td>0x05</td>
		<td>Path destination unknown</td>
		<td>The path references an unknown object class, instance or
structure element causing the abort of path processing.</td>
	</tr>
	<tr>
		<td>0x06</td>
		<td>Partial transfer</td>
		<td>Only a part of the expected data could be transferred.</td>
	</tr>
	<tr>
		<td>0x07</td>
		<td>Connection lost</td>
		<td>The connection for messaging has been lost.</td>
	</tr>
	<tr>
		<td>0x08</td>
		<td>Service not supported</td>
		<td>The requested service has not been implemented or has not
been defined for this object class or instance</td>
	</tr>
	<tr>
		<td>0x09</td>
		<td>Invalid attribute value</td>
		<td>Detection of invalid attribute data</td>
	</tr>
	<tr>
		<td>0x0A</td>
		<td>Attribute list error</td>
		<td>An attribute in the Get_Attribute_List or Set_Attribute_List
response has a status not equal to 0.</td>
	</tr>
	<tr>
		<td>0x0B</td>
		<td>Already in requested state</td>
		<td>The object is already in the mode or state which has been
requested by the service</td>
	</tr>
	<tr>
		<td>0x0C</td>
		<td>Object state conflict</td>
		<td>The object is not able to perform the requested service in the
current mode or state</td>
	</tr>
	<tr>
		<td>0x0D</td>
		<td>Object already exists</td>
		<td>It has been tried to create an instance of an object which
already exists.</td>
	</tr>
	<tr>
		<td>0x0E</td>
		<td>Attribute not settable</td>
		<td>It has been tried to change a non-modifiable attribute.</td>
	</tr>
	<tr>
		<td>0x0F</td>
		<td>Privilege violation</td>
		<td>A check of permissions or privileges failed</td>
	</tr>
	<tr>
		<td>0x10</td>
		<td>Device state conflict</td>
		<td>The current mode or state of the device prevents the execution
of the requested service.</td>
	</tr>
	<tr>
		<td>0x11</td>
		<td>Reply data too large</td>
		<td>The data to be transmitted in the response buffer requires more
space than the size of the allocated response buffer</td>
	</tr>
	<tr>
		<td>0x12</td>
		<td>Fragmentation of primitive value</td>
		<td>The service specified an operation that is going to fragment a
primitive data value, i.e. half a REAL data type.</td>
	</tr>
	<tr>
		<td>0x13</td>
		<td>Not enough data</td>
		<td>The service did not supply all required data to perform the
specified operation</td>
	</tr>
	<tr>
		<td>0x14</td>
		<td>Attribute not supported</td>
		<td>An unsupported attribute has been specified in the request</td>
	</tr>
	<tr>
		<td>0x15</td>
		<td>Too much data</td>
		<td>More data than was expected were supplied by the service.</td>
	</tr>
	<tr>
		<td>0x16</td>
		<td>Object does not exist</td>
		<td>The specified object does not exist in the device.</td>
	</tr>
	<tr>
		<td>0x17</td>
		<td>Service fragmentation sequence erroruccess</td>
		<td>Fragmentation sequence for this service is not currently active
for this data</td>
	</tr>
	<tr>
		<td>0x18</td>
		<td>No stored attribute data</td>
		<td>The attribute data of this object has not been saved prior to the
requested service.</td>
	</tr>
	<tr>
		<td>0x19</td>
		<td>Store operation failure</td>
		<td>The attribute data of this object could not be saved due to a
failure during the storage attempt</td>
	</tr>
	<tr>
		<td>0x1A</td>
		<td>Routing failure, request packet too large</td>
		<td>The service request packet was too large for transmission on a
network in the path to the destination. The routing device was
forced to abort the service</td>
	</tr>
	<tr>
		<td>0x1B</td>
		<td>Routing failure, response packet too large</td>
		<td>The service response packet was too large for transmission on
a network in the path from the destination. The routing device
was forced to abort the service</td>
	</tr>
	<tr>
		<td>0x1C</td>
		<td>Missing attribute list entry data</td>
		<td>The service did not supply an attribute in a list of attributes that
was needed by the service to perform the requested behavior</td>
	</tr>
	<tr>
		<td>0x1D</td>
		<td>Invalid attribute value list</td>
		<td>The service returns the list of attributes containing status
information for invalid attributes</td>
	</tr>
	<tr>
		<td>0x1E</td>
		<td>Embedded service error</td>
		<td>An embedded service caused an error</td>
	</tr>
	<tr>
		<td>0x1F</td>
		<td>Vendor specific error</td>
		<td>A vendor specific error has occurred. This error should only
occur when none of the other general error codes can correctly
be applied</td>
	</tr>
	<tr>
		<td>0x20</td>
		<td>Invalid parameter</td>
		<td>A parameter which was associated with the request was invalid.
The parameter does not meet the requirements of the CIP
specification and/or the requirements defined in the specification
of an application object.</td>
	</tr>
	<tr>
		<td>0x21</td>
		<td>Write-once value already written</td>
		<td>An attempt was made to write to a write-once medium for the
second time, or to modify a value that cannot be changed after
being established once</td>
	</tr>
	<tr>
		<td>0x22</td>
		<td>Invalid reply received</td>
		<td>An invalid reply is received. Possible causes can for instance be
among others a reply service code not matching the request
service code or a reply message shorter than the expectable
minimum size</td>
	</tr>
	<tr>
		<td>0x23</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0x24</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0x25</td>
		<td>Key failure in path</td>
		<td>The key segment (i.e. the first segment in the path) does not
match the destination module. More information about which
part of the key check failed can be derived from the object
specific status.</td>
	</tr>
	<tr>
		<td>0x26</td>
		<td>Path size invalid</td>
		<td>Path cannot be routed to an object due to lacking information or
too much routing data have been included</td>
	</tr>
	<tr>
		<td>0x27</td>
		<td>Unexpected attribute in list</td>
		<td>It has been attempted to set an attribute which may not be set in
the current situation</td>
	</tr>
	<tr>
		<td>0x28</td>
		<td>Invalid member ID</td>
		<td>The Member ID specified in the request is not available within
the specified class/ instance or attribute</td>
	</tr>
	<tr>
		<td>0x29</td>
		<td>Member cannot be set</td>
		<td>A request to modify a member which cannot be modified has
occurred</td>
	</tr>
	<tr>
		<td>0x2A</td>
		<td>Group 2 only server general failure</td>
		<td>This DeviceNet-specific error cannot occur in EtherNet/IP</td>
	</tr>
	<tr>
		<td>0x2B - 0xCF</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xD0 - 0xFF</td>
		<td>Vendor specific Codes</td>
		<td>An object class specific error has occurred</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](4-pnio/README.md)
# 4. PROFINET I/O (Hi7)

<br>

This chapter explains how to connect the robot controller's internal input/output signals using the PROFINET I/O device (BD671). <br>

<br>


{% hint style="info" %}
The function of PROFINET I/O (BD671) is supported by the Hi7 robot controller.<br>
For the PROFIsafe manual, please refer to the SafeSpace 2.0 manual ([SafeSpace 2.0 link](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/3-safety-function/3-safety-function/4-safety-io/5-profisafe))
{% endhint %}
[__SOURCE](4-pnio/1-pnio.md)
## 4.1 PROFINET Communication Settings

 **1. PROFINET**
- PROFINET is an Ethernet-based communication standard for industrial automation.
- It supports real-time data exchange between controllers (PLCs, robot controllers, etc.) and distributed I/O devices (drives, sensors, modules, etc.).

**2. PROFINET Specifications**
- Digital input: 50, 120, and 240 bytes (select one type of byte count)
- Digital output: 50, 120, and 240 bytes (select one type of byte count)
- Safety I/O: 8/8 bytes (activated or deactivated)
- Minimum communication cycle: 1 msec
- Supported communication speed: 10 or 100 Mbps
- Conformance Class: B
- Netload Class: II
- Optional Feature: Legacy, MRP

**3. PROFINET Configuration Procedure**

1) Connection of BD671, PROFINET controller and Hi7 Com
2) GSDML file registration (TIA portal)
3) PROFINET controller settings (TIA portal)
4) Hi7 settings (TP UI)
5) PROFINET communication verification
6) PROFINET I/O signal assignment (FB block settings)

**3.1 Connection of BD671, F-Host and Hi7 Com**

**3.1.1 LAN Cable Connection**
1) Connect the PROFINET controller and BD671 using a LAN cable.
2) Check if the Link LED is blinking.
3) Connect the Hi7 COM's LAN3 connector and BD671 using a LAN cable.
4) Check if the Link LED is blinking.

![](../_assets/4-pnio/profisafe_connect.png)

**3.1.2 Hi7 Com Connection Settings**
1) Navigate to the menu as follows: System -> Control Parameters -> Industrial Communication -> EtherCAT Master Settings
2) Configure as shown below.
- EtherCAT Master : ON
- Port : LAN3
3) Select "OptionBD - PROFINET_IO" from the slave list and press the Apply button.
4) Reboot the Hi7 robot controller.
5) After rebooting, check the status of the Run, Communication, Error LEDs.

![](../_assets/4-pnio/EC_master_setting1.png)
<br> <br>
![](../_assets/4-pnio/EC_master_setting2.png)


**3.2 GSDML File Registration (TIA portal)**
1) Run the TIA portal.
2) Navigate as shown on the right in the menu: [Options] → [Manage general station description file (GSD)].
3) Click the "..." button and set the directory where the GSDML file is located.
4) Select "GSDML-V2.43-Hyundai-Robotics-Hi7-20251127.xml" from the list displayed on the screen and press the [Install] button.
5) Check if it has been registered as a new device in the hardware catalog. <br>
![](../_assets/4-pnio/profisafe_gsdmal.png)

**3.3 PROFINET Controller Settings (TIA portal)**
1) Run the TIA portal and create a new project.
2) Double-click the Device & Network section to open it.<br>
![](../_assets/4-pnio/profisafe_device_network.png)

3) Select a controller that supports PROFINET communication (e.g., CPU 1511F-1 PN) and drag it to the network view.
4) Add the device (HRC, PROFINET I/O DAP) added in the previous step from the hardware catalog and drag it to the network view.
5) Connect the two devices by dragging and dropping the LAN ports in the two device figures.<br>
![](../_assets/4-pnio/profisafe_device_network2.png)

6) Double-click the HRC-IO device in the "Device & Network" screen.
7) Select the desired slot.
8) Drag the desired module (DI, DO, or PROFIsafe I/O) from the catalog on the right and move it to the "Device Overview window."<br>
![](../_assets/4-pnio/profisafe_device_network3.png)

9) Double-click the HRC-IO device in the "Device & Network" screen.
10) Click the HRC-IO device again to open the Settings screen.
11) Navigate to the General tab below.
12) Select Ethernet addresses from the menu on the left.
13) Uncheck "Generate PROFINET device name automatically."
14) Set "PROFINET device name" to "hd-hrc-0" and save.<br>
![](../_assets/4-pnio/profisafe_device_network4.png)

**3.4 Hi7 Settings (TP UI)**
1) Set the parameters to the values below, which are the same as those set in the PNIO controller.
- PROFINET IO Device Name : hd-hrc-0
- Slot 1 : Digital Input : 240
- Slot 2 : Digital Output : 240
- Slot 3 : Safety I/O : No
- (No need to change the IP address.)
2) Press the "Apply" button.<br>
![](../_assets/4-pnio/4_1_profinet_config.png)

**3.5 PROFINET Communication Verification**
**3.5.1 Ladder Program (TIA portal)**
1) In the Device Overview tab, create a ladder program as shown below and download it to the controller.<br>
![](../_assets/4-pnio/5_1_Safety_Ladder.png)
2) After downloading, check if a green checkbox is displayed on the Distribution I/O screen.<br>
![](../_assets/4-pnio/5_1_Safety_Ladder2.png)

**3.5.2 TP Screen**
In the menu, navigate to **\[System > 2: Control Parameter > 11: Industrial Communication > 5: PROFINET Settings]**<br>
![](../_assets/4-pnio/PROFINET_monitoring.png)
- Check the status information of each slot.
- Check if the counter continuously increases.


**3.6 PROFINET I/O Signal Assignment (FB block settings)**
1) Navigate to System → Control Parameters → Input/Output Signal Settings → FB Block Assignment
2) Change the block settings to PROFINET I/O as many as needed (up to two).
 (The maximum PROFINET I/O size is 240 bytes and the individual FB block size is 120 bytes. Therefore, **any settings exceeding two will be ignored.**)<br>
![](../_assets/4-pnio/6_fb_block.png)

3) Additionally, navigate to the Condition Settings menu and check if the PLC operation mode is OFF.<br>
![](../_assets/4-pnio/6_1_condition.png)
4) Check the input/output signals on the TIA portal screen and General I/O screen.<br>
![](../_assets/4-pnio/6_3_public_io.png)

[__SOURCE](4-pnio/2-pnio-status.md)
## 4.2 PROFINET Status Monitoring

By selecting the **\[System > 2: Control Parameter > 11: Industrial Communication > 5: PROFINET Settings]** menu, you can monitor the PROFINET status by slot.

<p align="center">
<img src="../_assets/4-pnio/PROFINET_monitoring.png"></img>
<em><p align="center">PROFINET Status Monitoring Screen</p></em>
</p>

- Size: Indicates the set I/O size (unit: byte).
- Status: BAD (not in use or communication error), GOOD (communication normal)
- Counter: I/O update count (communication normal if it continuously increases)

<p align="center">
<img src="../_assets/4-pnio/profinet_LED.png"></img>
<em><p align="center">BD671(PROFINET) </p></em>
</p>

* The version information is indicated by the LED blinking pattern during boot-up.
    - MCU: 1 (Major), 5 (Minor)
    - DSP: 4 (Major), 6 (Minor)
[__SOURCE](4-pnio/3-mrp.md)
## 4.3 MRP Settings

BD671 can be configured as an MRP Client to use the cable redundancy function.
In addition to the basic PROFINET settings, configure the following settings to enable the MRP function.

1) Topology setting
<p align="center">
<img src="../_assets/4-pnio/mrp-topology.png"></img>
<em><p align="center">Topology </p></em>
</p>

2) MRP Client setting

<p align="center">
<img src="../_assets/4-pnio/mrp_set_client.png"></img>
<em><p align="center">MRP Client </p></em>
</p>

3) Watchdog Time Setting (Set to 200 ms or longer)

 - The Watchdog Time must be set to 200 ms or longer to allow the MRP Manager to perform network topology reconfiguration (see figure).

<p align="center">
<img src="../_assets/4-pnio/mrp_watchdog.png"></img>
<em><p align="center">Watchdog Time </p></em>
</p>



[__SOURCE](5-io-block-allocation.md)
# 5. Industrial Communication IO Reading and Writing

This is the method for assigning IO blocks for the communication with the controller after completing industrial communication settings.

To use the industrial communication IO, the IO blocks should be assigned to the fb0 - fb9 area.

<br>

{% hint style="info" %}
   - For the IO reading/writing methods for fb blocks, please refer to the manual below.

      **\[Controller Operation Manual: General Input]**   
      **\[Controller Operation Manual: General Output]**   
{% endhint %}

<br>

**1. Select the IO block assignment menu.**
   Touch the **\[System > 2: Control Parameters > 2: Input/Output Signal Settings > 6: FB Block Assignment]** menu.

<br>

**2. Specify industrial communication type for the desired fb area.**
   After specifying it, touch the **\[OK]** button.

![[Figure 5-1]](<_assets/5-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[Caution]**: When using together with an embedded PLC, please check IO attributes and DI/DO - X/Y.
{% endhint %}

{% hint style="info" %}

   **[fb Block Allocation Method]**

   - The size of one fb block is 120 bytes (960 points).   

   - Example of fb block allocation   
      - PCI slot 1: CC-Link Slave   
      - Configuration: Version2, 3 Stations, 8 Extension cyclic   
      - I/O Size   
         - RX/Y: 80 byte   
         - RWr/w: 192 byte   
         - Total: 272 byte   

      - I/O mapping is assigned in ascending order of fb block number   
      - fb2: PCI slot 1 ( ~ 120 byte)   
      - fb4: PCI slot 1 ( ~ 240 byte)   
      - fb5: PCI slot 1 ( ~ 272 byte)   

{% endhint %}
[__SOURCE](6-slave-config-file.md)
# 6. Slave Device Description Files

To configure the slave communication from the industrial communication master, a description file for the slave device for each protocol is used.

<br>

The slave device description files can be downloaded from our website.
Download "**Hi7 Fieldbus Config**" from [www.hd-hyundairobotics.com](https://hd-hyundairobotics.com/) -> Industrial Robot Website -> Customer Support -> Application Software.

<br>

{% hint style="info" %}
   - EtherNet/IP: EDS file

   - PROFINET IO: GSDML (.XML) file

   - EtherCAT: ESI (.XML) file

   - PROFIBUS-DP: GSD file

   - DeviceNet: EDS file

   - CC-Link IE Field: CSPP file

   - CC-Link IE Basic: CSPP file
{% endhint %}

<br>

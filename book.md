# Hi6 Robot Controller Manual - Industrial Communication

{% hint style="warning" %}
The information presented in this manual is the property of Hyundai Robotics.

The manual may neither be copied, in part or in full, nor redistributed without prior written consent from Hyundai Robotics.

It may neither be provided to any third party nor used for any other purposes.



Hyundai Robotics reserves the right to modify this document without prior notification.



**Copyright ⓒ 2020 by Hyundai Robotics**
{% endhint %}
# 1. Installing the Program

This is about installing a program related to industrial communication.
# 1.1 Sycon.net

This is a program that creates a communication configuration that is to be used for a PCI communication card.

**1.**     Download “**Sycon.net**” from Hyundai Robotics’ home page ([www.hyundai-robotics.com](http://www.hyundai-robotics.com)) -> Customer Support -> Application Software.

**2.**     Decompress -> Run the “**Communication-Solutions.exe**” file in the internal folder. -> Select “**Install SYCON.net Configuration Software**” to install the program.

![Figure 1 Screen for installing Sycon.net](<../_assets/image_5.png>)
# 1.2 Multiprog

This is a PLC program to be used for DIO data exchange after connecting the PCI communication card. (Using it after setting “**PLC**” in “[**3.3 Setting the Industrial Communication DIO Block Allocation**](../3-setting-industrial-communication/3-3-dio-block-allocation/)” is required.)

**1.**     Download “**Hi6 Multiprog**” from Hyundai Robotics’ home page ([www.hyundai-robotics.com](http://www.hyundai-robotics.com)) -> Customer Support -> Application Software.

**2.**     Proceed to the installation according to the instructions below.

{% hint style="info" %}
1. Decompress the MP5.51 Express.zip file.
2. Run the MULTIPROG 5.51.msi file.
   * Perform installation with the setup.exe file if an error occurs during installation**.**
3. Decompress the MP eCLR Addon.zip file.
4. Run the I486\_LE\_GCC3\_eCLR.exe file
5. Decompress the MULTIPROG 5.51 Build 653.zip file.
6. Run the “multiprog\_set\_batch\_express.bat” file (run as administrator) in the MULTIPROG 5.51 Build 653 folder.

![](<../_assets/image_10.png>)

&#x20;

*   Additional work should be performed as below if there is a problem with building a project. It is possible that the files in the MULTIPROG 5.51 Build 653 folder are not copied properly.&#x20;

    \-> Copy all files of the MULTIPROG 5.51 Build 653 folder into the same folder as the MULTIPROG installation path. Find the “Default installation” location below and then paste the files of the MULTIPROG 5.51 Build 653 folder into the location.

    * Default installation: Paste the copied files into C:\Program Files (x86)\PHOENIX CONTACT Software\MULTIPROG 5.51 Express Build 653 folder (overwrite 3 files).

&#x20;

\*\*How to check\*\*

\-> Check the following files at the default installation (or installation) location.


{% endhint %}

![](../_assets/image.png)

(If you want to use the Pro version, you should install it using “**Hi6 MultiProg Development Environment Installation Guide.pdf.**” However, as the license for it is needed, you need to purchase it separately by requesting to the main office of Hyundai Robotics. Without a license, please note that the Pro version can be used only for 30 days.)
# 2. Mounting and Setting the Industrial Communication Card

A PCI communication card (Hilscher) is required to use industrial communication. The method of connecting the communication card in a way that matches the required communication is shown below.

1. Mount the purchased PCI communication card into the Hi6Com (Collaborative robots: Hi6Com Mini).
2. Turn the rotary switch of the PCI communication card to set it to a number ranging from 1 to 4.(Individual numbers should be set if multiple PCI communication cards are to be used.)

![Figure 2 Basic configuration of the LCD robot system](<_assets/image_14.png>)

{% hint style="warning" %}
**\[Caution]**: Setting the rotary switch number differently for each PCI card is required.
{% endhint %}
# 3. Setting the Industrial Communication

After the installation of the PCI communication card, the relevant setting should be performed using the teach pendant and Sycon.net program to use industrial communication.
# 3.1 Setting the Industrial Communication Firmware

The method to set and use the industrial communication firmware is as shown below. After the setting is completed, the controller power should be turned off and then back on to allow the firmware to be applied.

1. Set the **\[Set Up > 2: Control Parameter > 11: Industrial Communication > 1: Firmware Setting > 1 Channel]** menu to enter the firmware setting screen.
2. By referring to the screen shown below, select the slot you set in advance and then set the communication method (Master/Slave). Finally, select the desired protocol.
   * The slot number is the rotary switch number of the PCI communication card.
   * If you do not want to set the communication firmware, you should initialize the firmware information on the tab you are looking at now by touching the **\[Clear]** button. Please take note that the Config file will also be initialized.

![Figure 3 Screen for setting the industrial communication (master)](<../_assets/image_7.png>) ![Figure 3 Screen for setting the industrial communication (Slave)](<../_assets/image_3.png>)

3\. Touch the **\[Apply]** menu to complete the firmware setting.

{% hint style="warning" %}
**\[Caution]**

1. When you complete the firmware setting by touching the **\[Apply]** button, the Config file set for the relevant slot will also be deleted. If you want to modify the communication firmware in the middle of using it, you need to back up the existing Config setting.
2. If you touch the **\[OK]** button without touching the **\[Apply]** button first, the set firmware will not be applied.
{% endhint %}

4\. **** Set the firmware for each slot by repeating Steps #2 and #3.

5\. **** The firmware will be applied when you turn the controller power off and then back on.

{% hint style="warning" %}
**\[Caution]**: When you set the use of the firmware, the setting values will be applied to the system only when you turn the controller power off and then back on.
{% endhint %}
# 3.2 Setting the Addition of the Industrial Communication (Master and Slave)

After you set the industrial communication firmware, you are required to perform relevant settings using the “**Sycon.net**” program on the Hyundai Robotics home page to use the communication.
# 3.2.1 Using Sycon.net

When you need to use the industrial communication of the Hi6 controller, you are required to set the communication using the “**Sycon.net**” program. The setting method is as shown below. (Perform installation by referring to Section “[**1.1 Sycon.net**](../../1-install-program/1-1-sycon-net.md)”)

1. Connect the LAN3 port of the Hi6Com (Collaborative robot: Hi6MiniCom) to a PC.
2. &#x20;**** Regarding the communication setting method, you should refer to “Sycon.net v1.0500\DVD\_2018-12-1\_1\_0500\Documentation\4. You can also refer to the files in “Training Material\EN.”
   *   Names of the files to refer to

       1\) EtherNetIP Scanner - Configuration and Testing TM 02 EN.pdf

       2\) PROFIBUS DP Master - Configuration and Testing TM 02 EN.pdf

       3\) PROFINET IO Controller - Configuration and Testing TM 02 EN.pdf

{% hint style="info" %}
1\.      This example shows how to set the netX Driver for connecting the Hi6 driver.

2\.      You can set the IP address according to the setting of the controller.

3\.      How to set the EtherCAT Master (Connection of the CIFX card)
{% endhint %}

![](<../../_assets/image_6.png>)

{% hint style="info" %}
4\.      “Double-click” on the connected CIFX card (Figure).

5\.      Perform setting in Driver -> Netx Driver.
{% endhint %}

![](<../../_assets/image_13.png>)

{% hint style="info" %}
6\.      In netX Driver -> TCP Connection, perform setting as shown below. (The ID address&#x20;

&#x20;        may change depending on the controller, so you need to check it.)
{% endhint %}

![](<../../_assets/image_20.png>)

{% hint style="info" %}
7\.      Click on Device Assignment -> Scan. (If nothing appears: Change the device&#x20;

&#x20;        selection from suitale  only -> all and then click on Scan again).

8\.      Select the set communication (check the channel), and then “Apply,” and then “OK.”
{% endhint %}

![](<../../_assets/image_2.png>)

{% hint style="warning" %}
**\[Caution]**: If the location of the Access path is not cifX(num)\_Ch0, change it in Access path at the bottom and then apply
{% endhint %}

{% hint style="info" %}
9\.      Perform the necessary settings and right-click on the CIFX figure -> Download.
{% endhint %}
# 3.3 Setting the Industrial Communication DIO Block Allocation

This shows how to perform DIO block allocation for the communication with the controller after “[**3.1 Setting the Industrial Communication Firmware**](../3-1-firmware.md)” 및 “[**3.2 Setting the Addition of the Industrial Communication (Master and Slave)**](../3-2-addition-industrial-communication-master-slave/)” work is completed.

You can set the method to use the universal input and output signals of the controller. For the use, you can connect to None, PLC, or Fieldbus.

1. Touch the **\[2: Control Parameter > 2: Input/Output Signal Setting > 6: DIO Block Allocation]** menu.
2. Set the connection of the DIO block of the selected FB address and then touch the \[OK] button.
   * If Fieldbus is set, the board number will be the rotary switch number of the PCI communication card.
   * If PLC is to be used, refer to “[**3.3.1 Using Multiprog**](1-using-multiprog.md)”

![](<../../_assets/image_11.png>)

* **\[None]**: The DIO block of the selected FB address is not to be allocated. If nothing is to be selected for the initial setting value of the controller, None will be set.
* **\[PLC]**: The DIO block of the selected FB address will be allocated to the PLC for use. For the PLC operation, the MULTIPRO program will be used.
* **\[Fieldbus]**: The DIO block of the selected FB address will be allocated to the PCI communication card for use. If the DIO block is connected to the PCI communication card, the PCI board selection window will be enabled.

{% hint style="warning" %}
**\[Caution]**: The same communication card cannot be used both for PLC and Fieldbus at the same time. Data connection should be performed for one of the two.
{% endhint %}
# 3.3.1 Using Multiprog

After industrial communication is set, the following setting is necessary to perform DIO data exchange through ProconOS if the DIO block of the Hi6 controller is allocated to PLC. (Perform installation by referring to Section “[**1.2 Multiprog**](../../1-install-program/1-2-multiprog.md)”)

1. Regarding how to use after installation, refer to the manual included in Multiprog. –

{% hint style="info" %}
1\.      This shows a simple example of how to set Hi6 Multiprog.

2\.      You can set the IP address according to the setting of the controller.

3\.      Create a project (Execute Multiprog -> Click on “File” -> “New Project” -> Project&#x20;

&#x20;         Wizard and then OK).
{% endhint %}

![](<../../_assets/image_21.png>)

{% hint style="info" %}
4\.      Create a project according to the sequence.

(1)    Create a project.
{% endhint %}

![](<../../_assets/image_15.png>)

{% hint style="info" %}
(2) Set the POU and program language.
{% endhint %}

![](<../../_assets/image_18.png>)

{% hint style="info" %}
(3) Set the resource and type. (If there is no “Hi6” in Type, it means that installation has been performed in the wrong way. Checking whether the installation is performed correctly is required.)
{% endhint %}

![](<../../_assets/image_1.png>)

{% hint style="info" %}
(4) Create a task.
{% endhint %}

![](<../../_assets/image_8.png>)

{% hint style="info" %}
5\.      Set the project property.

(1)    Set the hardware property: Double-click on IO\_Configuration -> Set the Input/Output property
{% endhint %}

![](<../../_assets/image_16.png>)

{% hint style="info" %}
* Connection of HI6 DIO input <-> Multiprog output / HI6 DIO output <-> Multiprog input has been performed.
*   Connection of CIFX input <-> Multiprog input / HI6 DIO output <-> Multiprog output has been performed.

    &#x20;

(2)    How to set IO: Set the name. -> Set the task. -> Select the Board /IO module. -> Select and set the driver parameter (Offset 0: Hi6 Controller FB0.0. Unit: Byte).
{% endhint %}

![](<../../_assets/image_9.png>)

{% hint style="info" %}
(3) Set the IP address: Resource: Right-click on Hi6 (varies depending on the created name), and then match the IP in Settings -> Parameter to Hi6.
{% endhint %}

![](<../../_assets/image_4.png>)

{% hint style="info" %}
6\.      Write a PLC program. (Perform programming according to the needs of the user.)

7\.      Program downloading: Online -> Project Control -> Click on Download
{% endhint %}

![](<../../_assets/image_17.png>)
# 4. Monitoring the Industrial Communication

After communication is set according to the procedures of “[**2. Mounting and Setting the Industrial Communication Card**](2-mounting-setting-industrial-communication-card.md)” and “[**3. Setting the Industrial Communication**](3-setting-industrial-communication/),” it is possible to check, from the screen shown below, whether the operation is performed.

You need to enter **\[Menu > 19: Industrial Communication Monitoring]** by touching it. You can also check the information regarding the set firmware, communication state, communication configuration, etc. on the relevant screen.

![](<_assets/image_19.png>)

{% hint style="info" %}
Using the **\[Restart]** button, you can restart the industrial communication with the relevant PCI communication card.
{% endhint %}

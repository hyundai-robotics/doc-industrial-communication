# 1.3.2 SYCON.NET Settings

Hi6 제어기는 “**Sycon.net**” 프로그램을 이용하여 산업용 통신 설정을 진행합니다. 설정 방법은 다음과 같습니다. (“[For the Hi6 controller, proceed with industrial communication settings using the "**Sycon.net**" program. The setting method is as follows. (Please install by referring to "**1.1 Sycon.net Installation**.")](../../1-cifx-pci-install-program/1-sycon-net.md)”을 참고하여 설치해주시기 바랍니다.)

<br>

##### 1. Reference materials related to communication settings.
The materials of *\"Sycon.net v1.0500\DVD\_2018-12-1\_1\_0500\Documentation\4. Training Material\EN"** can be referenced.
   * Reference materials

1\) EtherNetIP Scanner - Configuration and Testing TM 02 EN.pdf

2\) PROFIBUS DP Master - Configuration and Testing TM 02 EN.pdf

3\) PROFINET IO Controller - Configuration and Testing TM 02 EN.pdf

<br>

##### 2. Connect the PC with Sycon.net installed and the general LAN port of the robot controller (not the PCI LAN port).
Touch the *\[System > 2: Control Parameters > 9: Network]** menu to check the IP of the general LAN port. Please check the connection status through a ping test, etc.

![[Figure 1.3.2-1 Network IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_1.png>)
![[Figure 1.3.2-2 Network IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_2.png>)

{% hint style="info" %}
\.      IP Address can be changed according to user settings.
{% endhint %}

<br>

##### 3. Execute Sycon.net.

![[Figure 1.3.2-3 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_3.png>)

<br>

##### 4. In the Device Catalog menu on the right side of the screen, click the item matching the set communication protocol and place it on the bus line in the center by dragging and dropping it.

![[Figure 1.3.2-4 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_4.png>)
![[Figure 1.3.2-5 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_5.png>)

<br>

##### 5. Double-click the imported item to set it.

{% hint style="info" %}
\.      "Double-click" the imported CIFX PCI (figure).

\.      Settings -> Driver

\.      Select netX Driver.
{% endhint %}

![[Figure 1.3.2-6 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_6.png>)

{% hint style="info" %}
\.     Setting -> Driver -> netX Driver -> TCP Connection

\.      IP Address: Please enter the general LAN port IP address of the connected controller.
{% endhint %}

![[Figure 1.3.2-7 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_7.png>)

{% hint style="info" %}
\.      Device Assignment -> Click Scan

\.      Select communication (check the channel protocol) then "Apply" and "OK."
{% endhint %}

{% hint style="warning" %}
*\[Caution]**: Please be sure to check the channel protocol and slot number.
{% endhint %}

{% hint style="warning" %}
*\[Caution]**: If scan is not working, check the status of the cable connection with the controller and also the firmware settings.
{% endhint %}

![[Figure 1.3.2-8 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_8.png>)


{% hint style="info" %}
\.      Right-click the CIFX PCI figure -> Download
{% endhint %}

![[Figure 1.3.2-9 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_9.png>)
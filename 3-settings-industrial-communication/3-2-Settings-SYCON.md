# 3.2 Setting SYCON.net

If the industrial communications of the Hi6 controller will be be used, communications should be set using the “**SYCON.net**” program. The installation methods are as follows (refer to “[**1.1 Installing SYCON.net**](../1-install-program/1-1-sycon-net.md)” for installation).

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

![[Figure 3.2-1 Network IP]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_1.png>) 

{% hint style="info" %}
\.      The IP address can be changed according to the User settings.
{% endhint %}

<br>

##### 3. Run SYCON.net.

![[Figure 3.2-2 SYCON.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_2.png>)

<br>

##### 4. In the device catalog on the right side of the screen, click the item that fits the set communication protocol, then drag and drop it on the bus line at the center. 

![[Figure 3.2-3 SYCON.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_3.png>)
![[Figure 3.2-4 SYCON.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_4.png>)

<br>

##### 5. Double-click the imported item to set it.

{% hint style="info" %}
\.      “Double click” the CIFX PCI card (figure.)

\.      Settings -> Driver 

\.      Select netX Driver
{% endhint %}

![[Figure 3.2-5 SYCON.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_5.png>)

{% hint style="info" %}
\.     Settings -> Driver -> netX Driver -> TCP Connection 

\.     IP Address: Input the universal LAN Port IP Address of the connected controller.
{% endhint %}

![[Figure 3.2-6 SYCON.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_6.png>)

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

![[Figure 3.2-7 SYCON.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_7.png>)


{% hint style="info" %}
\.      right-click the CIFX PCI figure -> Download
{% endhint %}

![[Figure 3.2-8 SYCON.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_8.png>)
# 3.10.1 EtherNet/IP - Setting the Connection of a Standard Remote IO

Perform settings according to the procedures of “[**3.1 Setting Industrial Communication Firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” first and proceed with the following methods.

<br>

##### 1. Select the EtherNet/IP Master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 3.10.1-1 Firmware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 3.10.1-2 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

##### 3. For communication, connect the cables for the PCI and remote IOs and check their status.

![[Figure 3.10.1-3 Hardware Connection]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[Figure 3.10.1-4 Hardware Connection]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

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

\.      “[**3.10.2 Remote IO IP Setting**](../../3-settings-industrial-communication/3-10-EtherNet-IP-Remote-IO/3-10-2-Settings-Remote-IO-IP.md)”
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave Configuration > EtherNet/IP Remote IO Setting]**

![[Figure 3.10.1-5 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>) 

![[Figure 3.10.1-6 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>) 

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

![[Figure 3.10.1-7 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>) 

![[Figure 3.10.1-8 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
\.      After the settings are completed, reboot the controller.
{% endhint %}

<br>

##### 6. Check whether the set values are reflected and then check the communication status.

![[Figure 3.10.1-9 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>) 

Please refer to (“[**4 Monitoring Industrial Communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

![[Figure 3.10.1-10 Industrial Commuication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>) 

{% hint style="info" %}
\.      If the communication is not connected, check the IP address of the remote IO.

\.      Check according to the following (if not 192.168.100.99).

\.      “[**3.10.2 Remote IO IP Setting**](../../3-settings-industrial-communication/3-10-EtherNet-IP-Remote-IO/3-10-2-Settings-Remote-IO-IP.md)”
{% endhint %}

![[Figure 3.10.1-11 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>) 

![[Figure 3.10.1-12 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>) 
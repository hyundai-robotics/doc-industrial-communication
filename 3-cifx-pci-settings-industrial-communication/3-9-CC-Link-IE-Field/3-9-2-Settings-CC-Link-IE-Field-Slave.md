# 3.8.2 Setting a CC-Link Slave

Perform settings according to the procedures of “[**3.1 Setting Industrial Communication Firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      Refer to the following for the connection of a CC-Link connector.

\.      (“[**2.2 Connectors**](../../2-mounting-settings-industrial-communication-card/2-2-Connector.md)”)
{% endhint %}

<br>

##### 1. By using the teach pendant, select the CC-Link slave in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 3.8.4-1 Firmware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 3.8.4-2 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If the Config file set using SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave Configuration > CC-Link Slave]**

![[Figure 3.8.4-3 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/4-Slave_setting/image_3.png>) 

![[Figure 3.8.4-4 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/4-Slave_setting/image_4.png>) 

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

\.      Depending on Number of Station, the size of the IO byte area will vary.
{% endhint %}

{% hint style="info" %}
\.      [Extension Cycle]

\.      Can be used in Version 2

\.      Remote Device: Can select among Single, Double, Quadruple, and Octuple

\.      Depending on the Extension Cycle, the size of the IO byte area to be assigned will vary. 
{% endhint %}

<br>

{% hint style="info" %}
\.      **For the IO byte area, please refer to the following link.**

\.      **(“[**3.8.1 Specifications of a CC-Link slave**](../../3-settings-industrial-communication/3-8-CC-Link/3-8-1-Specification-CC-Link-Slave.md)”)**
{% endhint %}

<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.

Please refer to (“[**4 Monitoring industrial communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

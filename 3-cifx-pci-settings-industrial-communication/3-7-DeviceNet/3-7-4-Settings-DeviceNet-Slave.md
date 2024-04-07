# 3.7.4 Setting a DeviceNet Slave

Perform settings according to the procedures of “[**3.1 Setting Industrial Communication Firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      **[DeviceNet Slave EDS File Download]**

\.      Please refer to “[**6. Slave Device Description Files**](../../6-slave-config-file.md).”
{% endhint %}

<br>

{% hint style="info" %}
\.      Refer to the following for the connection of the DeviceNet connector.

\.      (“[**2.2 Connectors**](../../2-mounting-settings-industrial-communication-card/2-2-Connector.md)”)
{% endhint %}

<br>

##### 1. By using the teach pendant, select the DeviceNet slave in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 3.7.4-1 Firmware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 3.7.4-2 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If the Config file set using SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave Configuration > DeviceNet Slave]**

![[Figure 3.7.4-3 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/4-Slave_setting/image_3.png>) 

![[Figure 3.7.4-4 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/4-Slave_setting/image_4.png>) 

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

Please refer to (“[**4 Monitoring Industrial Communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

![[Figure 3.7.4-5 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/4-Slave_setting/image_5.png>) 
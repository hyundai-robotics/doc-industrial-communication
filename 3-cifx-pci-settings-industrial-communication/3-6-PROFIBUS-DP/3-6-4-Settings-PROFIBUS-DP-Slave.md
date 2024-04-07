# 3.6.4 Setting a PROFIBUS-DP Slave

Perform settings according to the procedures of “[**3.1 Setting Industrial Communication Firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      **[PROFIBUS-DP Slave GSD File Download]**

\.      Please refer to “[**6. Slave Device Description File**](../../6-slave-config-file.md).”
{% endhint %}

<br>

##### 1. By using the teach pendant, select the PROFIBUS-DP slave in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 3.6.4-1 Firmware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 3.6.4-2 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**:  If the Config file set using SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave Configuration >  PROFIBUS-DP Slave]**

![[Figure 3.6.4-3 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[Figure 3.6.4-4 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

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

![[Figure 3.6.4-5 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/4-Slave_setting/image_5.png>) 


<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.


Please refer to (“[**4 Monitoring Industrial Communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

![[Figure 3.6.4-6 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/4-Slave_setting/image_6.png>) 
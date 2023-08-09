# 3.4.4 Setting a PROFINET IO Device

Perform settings according to the preocedures of “[**3.1 Setting Industrial Commuication Firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      **[PROFINET IO Device GSDML File Download]**

\.      Please refer to “[**6. Slave Device Description Files**](../../6-slave-config-file.md)"
{% endhint %}

<br>

##### 1. By using the teach pendant, select a PROFINET IO slave in the section for setting the industrial commuication firmware and reboot the robot controller.

![[Figure 3.4.4-1 Firmware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication. 

![[Figure 3.4.4-2 Industrial Communications Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If the Config file set via SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave Configuration > PROFINET IO Slave]**

![[Figure 3.4.4-3 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[Figure 3.4.4-4 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of Each Item

{% hint style="info" %}
\.      [Station Name]

\.      PROFINET IO identifies a slave via the station name.

\.      Naming Rule
\.       > The names of the devices connected through PROFINET IO should not be duplicated.  
\.       > The name can only have up to 240 characters.  
\.       > For special characters, "." and "-" can be used.  
\.       > For characters, English and numerical characters can be used.  
\.       > The name should start and end with an English character or number.

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

![[Figure 3.4.4-5 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_5.png>) 


<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.

Please refer to (“[**4 Monitoring Industrial Communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

![[Figure 3.4.4-6 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_6.png>) 
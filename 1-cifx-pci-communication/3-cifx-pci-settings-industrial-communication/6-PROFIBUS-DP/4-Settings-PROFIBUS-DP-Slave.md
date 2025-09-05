# 1.3.6.4 Setting a PROFIBUS-DP Slave

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      **[PROFIBUS-DP Slave GSD File Download]**

\.      Please refer to “[**5. Slave Device Description Files**](../../../5-slave-config-file.md).”
{% endhint %}

<br>

##### 1. By using the teach pendant, select the PROFIBUS-DP slave in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.6.4-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 1.3.6.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**:  If the Config file set using SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave PCI Slot Configuration >  PROFIBUS-DP Slave]**

![[Figure 1.3.6.4-3 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.6.4-4 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

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

<br>

{% hint style="info" %}
\.      [**setting the modules in the master**]

\.      Required to designate the modules in a way to match the individually set byte count

\.      Order: Master Input (64–1) -> Master Output (64–1)

\.      EX) Master Input 109 bytes  <---  Slave Output 109 bytes   
\.          109 Bytes : 64Byte + 32Byte + 8Byte + 4Byte + 1 Byte

\.      EX) Master Output 120 bytes  --->  Slave Input 120 bytes   
\.          120 Bytes : 64Byte + 32Byte + 16Byte + 8Byte


\.      EX) Master Input 12 bytes  <---  Slave Output 12 bytes   
\.          12 Bytes : 8Byte + 4Byte

\.      EX) Master Output 200 bytes  --->  Slave Input 200 bytes   
\.          200 Bytes : 64Byte + 64Byte + 64Byte + 8Byte

\.      Input modules are placed before the output modules.
{% endhint %}

<br>

![[Figure 1.3.6.4-5 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>) 


<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.


Please refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

![[Figure 1.3.6.4-6 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>) 

<br>

##### 6. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}
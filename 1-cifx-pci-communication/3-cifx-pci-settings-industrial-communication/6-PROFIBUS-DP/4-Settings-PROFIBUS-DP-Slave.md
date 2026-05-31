#### 1.3.6.4 PROFIBUS-DP Slave Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   **[PROFIBUS-DP Slave GSD File Download]**

   - Please refer to "[6. Slave Device Description File](../../../6-slave-config-file.md)".
{% endhint %}

<br>

**1. Using the TP, select a PROFIBUS-DP slave in the industrial communication firmware settings and reboot the robot controller.**

![[Figure 1.3.6.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

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
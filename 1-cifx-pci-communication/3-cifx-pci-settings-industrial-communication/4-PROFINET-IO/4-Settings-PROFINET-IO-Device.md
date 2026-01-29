#### 1.3.4.4 PROFINET IO Device Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   **[PROFINET IO Device GSDML File Download]**

   - Please refer to "[**5. Slave Device Description File**](../../../5-slave-config-file.md)".
{% endhint %}

<br>

**1. Using the TP, select a PROFINET IO slave in the industrial communication firmware settings and reboot the robot controller.**

![[Figure 1.3.4.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_1.png>)

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.4.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > PROFINET IO Slave]**

![[Figure 1.3.4.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[Figure 1.3.4.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
   [Station Name]

   - The PROFINET IO identifies a slave through the station name.

   - Naming Rule
      - Device names connected by PROFINET IO cannot be duplicated.  
      - A name can be set up to 240 characters.  
      - Special characters "." and "-" can be used.  
      - Lowercase English letters and numbers can be used.  
      - Names should start and end with lowercase English letters or numbers.  
{% endhint %}

{% hint style="info" %}
   [Input Byte Count (Input Byte)]

   - Input Byte Count: Sets the size of the data input from the master -> slave.
{% endhint %}

{% hint style="info" %}
   [Output Byte Count (Output Byte)]

   - Output Byte Count: Sets the size of the data output from the slave -> master.
{% endhint %}

<br>

{% hint style="info" %}
   [**When Setting a Slot from the Master**]

   - Master Input (32byte)  <--  Slave Output (32bytes)

   - Master Output (256bytes = 64bytes * 4)  -->  Slave Input (256bytes)

   - 4, 8, 16, 32, and 64 Bytes -> Specify the slot matching each byte count  
   - 128 and 256 Bytes -> Specify multiple 64-byte slots (2, 4)

   - The input slot is located before the output slot.
{% endhint %}

<br>

![[Figure 1.3.4.4-5 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_5.png>) 


<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.4.4-6 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_6.png>)

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}
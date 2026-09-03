#### 1.3.7.3 DeviceNet Master Settings (TP)

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - For DeviceNet connector connection, please refer to the following.

      ("[1.2.2 Connector](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. Select the DeviceNet master in the PCI slot settings and reboot the robot controller.**

![[Figure 1.3.7.3-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_1.png>)

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.7.3-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Select the DeviceNet master PCI device by using Sycon.net.**

**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > DeviceNet Master]**

![[Figure 1.3.7.3-3 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_3.png>)

![[Figure 1.3.7.3-4 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="warning" %}
**\[TP Network Scan Limitations]**   
   - Only Poll Connection is supported   
   - Quick Start is not supported  

{% endhint %}

<br>

{% hint style="info" %}
   [Use (Enable / Disable)]   
   - Off: DeviceNet Master disabled   
   - On: DeviceNet Master enabled   

   [Baud Rate]   
   - 125 kbit/s   
   - 250 kbit/s   
   - 500 kbit/s   

   [Master MAC ID]   
   - The MAC ID of the DeviceNet Master is fixed to 0   

   [IO Update Cycle]   
   - Production Inhibit Time: Minimum time interval between IO updates   
   - Expected Packet Rate: Expected time interval for packets to be received normally (related to timeout)   

{% endhint %}

<br>

**5. Click the "Network Scan" button after configuring the settings according to the communication environment.**

<br>

**10. Network Scan**

{% hint style="warning" %}
   **When performing the Network Scan function, be sure to check the following.**

   **(1) Whether a cable is connected.**  
   **(2) Whether a termination resistor is connected or a termination DIP switch is used.**  
   **(3) Whether the master - slave communication speed is set.**  

   **For smooth communication connection, be sure to check ("[1.3.7.5 DeviceNet ERROR Handling](../7-DeviceNet/5-Error-DeviceNet.md)").**
{% endhint %}

<br>

![[Figure 1.3.7.3-5 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_5.png>)

<br>

**6. After checking the device settings, click the "OK" button to apply the communication settings.**

<br>

![[Figure 1.3.7.3-6 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_6.png>)

<br>

**7. Description of node settings**

{% hint style="info" %}
   [Node information]   
   - Node: MAC ID of the device   
   - Product Name: Product name of the device   
   - Vendor ID: Unique ID of the device manufacturer   
   - Status: Status value of the device   
   
   [IO settings]   
   - Output Size: Master --> Slave (in bytes)   
   - Input Size: Slave --> Master (in bytes)   
   
   [IO update cycle]   
   - PIT (Production Inhibit Time): Minimum time interval between IO updates   
   - EPR (Expected Packet Rate): Expected time interval for packets to be received normally (related to timeout)   

{% endhint %}

<br>

{% hint style="info" %}
   [PIT (Production Inhibit Time)]   
   - After the network scan, the PIT is automatically calculated based on the total IO size of the connected devices.   

   - Example 1)   
      - 125 Kbit/s   
      - Total Input + Output: 100 byte   
      - Time required for 1 cycle: 100 x 8 (bit) / 125K = 6.4ms   
      - Applying a 33% communication load: 6.4 ms x 3 = 19.2ms --> PIT set to 20ms   

   - Example 2)   
      - 250 Kbit/s   
      - Total Input + Output: 500 byte   
      - Time required for 1 cycle: 500 x 8 (bit) / 250K = 16ms   
      - Applying a 33% communication load: 16 ms x 3 = 48ms --> PIT set to 48ms   

   - The PIT value can be changed individually for each device.   
   - A shorter interval may increase the communication load on the device. (check the specifications of each device.)   

{% endhint %}

<br>

![[Figure 1.3.7.3-7 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_7.png>)

<br>

**8. Check the communication status.**

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.7.3-8 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_8.png>)

<br>

![[Figure 1.3.7.3-9 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_9.png>)

<br>

**9. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
#### 1.3.9.2 CC-Link IE Field Slave Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.


<br>

**1. Using the TP, select a CC-Link IE Field slave in the industrial communication firmware settings and reboot the robot controller.**

![[Figure 1.3.9.2-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_1.png>) 

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.9.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > CC-Link IE Field Slave]**

![[Figure 1.3.9.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>) 

![[Figure 1.3.9.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
   [Network Number]

   - CC-Link IE field network number (1-239)
{% endhint %}

{% hint style="info" %}
   [Station Address]

   - Device ID within the connected network (1-120)
{% endhint %}

{% hint style="info" %}
   [IO Type]

   - IO type is determined by the master device settings.   
      - Mixed: Input and output use different indexes (different addresses).   
      - Input: Input only   
      - Output: Output only   
      - FrontBackMixture: Input and output use the same index (same address).   
{% endhint %}

{% hint style="info" %}
   [Device Type]

   - The maximum IO size that can be set varies depending on the Device Type.

   - Intelligent Device Station   
      - RY, RX (max): 256 bytes   
      - RWw, RWr (max): 1024 words

   - Remote Device Station   
      - RY, RX (max): 16 bytes   
      - RWw, RWr (max): 64 words
{% endhint %}

{% hint style="info" %}
   [IO Size]

   - Master -> Slave
      - RWw (word data)
      - RY (bit data)

   - Slave -> Master   
      - RWr (word data)   
      - RX (bit data)  
{% endhint %}

<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**5. Industrial Communication IO Reading and Writing**](../../../5-io-block-allocation.md)").**
{% endhint %}

<br>

![[Figure 1.3.9.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>) 
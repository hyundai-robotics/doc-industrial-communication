# 1.3.9.2 Setting a CC-Link IE Field Slave

Perform settings according to the procedures of “[**1.3.1 Setting CIFX PCI Slot**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” first and proceed with the following methods.

<br>

##### 1. By using the teach pendant, select the CC-Link IE Field slave in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 1.3.9.2-1 Firmware Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 1.3.9.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If the Config file set using SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave PCI Slot Configuration > CC-Link IE Field Slave]**

![[Figure 1.3.9.4-3 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>) 

![[Figure 1.3.9.4-4 Slave Setting]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of Each Item

{% hint style="info" %}
\.      [Network Number]

\.      Identifies the CC-Link IE Field network (1~239)
{% endhint %}

{% hint style="info" %}
\.      [Station Address]

\.      Current station address of the slave device as an unique identifier of a station within a network (1 ~ 120)
{% endhint %}

{% hint style="info" %}
\.      [IO Type]

\.      The parameter is not relevant for the Slave configuration. The IO type is evaluated by the master. For more information, refer to the manual of the master and/ or of the PLC.   
\.      - Mixed: In/Out with the different index. Refers to a case where the input and output are mixed and the input and output do not use the same address.      
\.      - Input: Input only   
\.      - Output: Output only   
\.      - FrontBackMixture: In/Out with the same index. Refers to a case where the input and output are mixed and the input and output use the same address.   
{% endhint %}

{% hint style="info" %}
\.      [Device Type]

\.      Intelligent Device Station   
\.      - RY, RX (max): 256 bytes   
\.      - RWw, RWr (max): 1024 words

\.      Remote Device Station   
\.      - RY, RX (max): 16 bytes   
\.      - RWw, RWr (max): 64 words
{% endhint %}

{% hint style="info" %}
\.      [IO Size]

\.      Master -> Slave   
\.      - RWw (word data)   
\.      - RY (bit data)   

\.      Slave -> Master   
\.      - RWr (word data)   
\.      - RX (bit data)  
{% endhint %}

<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.

Please refer to (“[**1.4 CIFX PCI - Monitoring Industrial Communication**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.

<br>

##### 6. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../../../4-io-block-allocation.md)”)**
{% endhint %}

<br>

![[Figure 1.3.9.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>) 
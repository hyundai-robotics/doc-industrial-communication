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
**\[Caution]**: 如果使用 Sycon.net 配置的文件下载到相应的 PCI 槽，TP 设置将被忽略。
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

   - 连接网络中的设备 ID (1-120)
{% endhint %}

{% hint style="info" %}
   [IO Type]

   - IO 类型由主设备设置决定。   
      - Mixed: 输入和输出使用不同的索引（不同的地址）。   
      - Input: 仅输入   
      - Output: 仅输出   
      - FrontBackMixture: 输入和输出使用相同的索引（相同的地址）。   
{% endhint %}

{% hint style="info" %}
   [Device Type]

   - 可设置的最大 IO 大小因设备类型而异。

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
      - RWw (字数据)
      - RY (位数据)

   - Slave -> Master   
      - RWr (字数据)   
      - RX (位数据)  
{% endhint %}

<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参阅 ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)")。**
{% endhint %}

<br>

![[Figure 1.3.9.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>)
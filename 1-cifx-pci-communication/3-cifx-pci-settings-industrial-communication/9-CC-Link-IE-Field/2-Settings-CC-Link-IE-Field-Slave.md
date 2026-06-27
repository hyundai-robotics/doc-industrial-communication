#### 1.3.9.2 CC-Link IE Field Slave Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

**1. 使用TP选择工业通信固件设置中的CC-Link IE Field从站，并重启机器人控制器。**

![[Figure 1.3.9.2-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查当前通信协议准备状态。**

![[Figure 1.3.9.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果通过Sycon.net设置的配置文件下载到相应的PCI插槽，则TP设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单以进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从站插槽设置 > CC-Link IE Field从站]**

![[Figure 1.3.9.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>) 

![[Figure 1.3.9.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>) 

<br>

**4. 各项描述**

{% hint style="info" %}
   [网络编号]

   - CC-Link IE现场网络编号 (1-239)
{% endhint %}

{% hint style="info" %}
   [站地址]

   - 连接网络内的设备ID (1-120)
{% endhint %}

{% hint style="info" %}
   [IO类型]

   - IO类型由主设备设置决定。   
      - 混合: 输入和输出使用不同的索引（不同的地址）。   
      - 输入: 仅输入   
      - 输出: 仅输出   
      - FrontBackMixture: 输入和输出使用相同的索引（相同的地址）。   
{% endhint %}

{% hint style="info" %}
   [设备类型]

   - 可以设置的最大IO大小因设备类型而异。

   - 智能设备站   
      - RY, RX (最大): 256字节   
      - RWw, RWr (最大): 1024字  

   - 远程设备站   
      - RY, RX (最大): 16字节   
      - RWw, RWr (最大): 64字
{% endhint %}

{% hint style="info" %}
   [IO大小]

   - 主 -> 从
      - RWw (字数据)
      - RY (位数据)

   - 从 -> 主   
      - RWr (字数据)   
      - RX (位数据)  
{% endhint %}

<br>

**5. 设置完成后，按照以下程序检查通信状态。**

For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

<br>

**6. 完成通信设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，可以通过分配IO块来使用输入/输出信号。请参考 ("[5. 工业通信IO读取和写入](../../../5-io-block-allocation.md)").**
{% endhint %}

<br>

![[Figure 1.3.9.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>)
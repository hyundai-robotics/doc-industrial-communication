#### 1.3.8.2 CC-Link从站设置

请遵循 "[1.3.1 CIFX PCI插槽设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 程序，然后继续以下方法。

<br>

{% hint style="info" %}
   - 有关CC-Link连接器连接，请参考以下内容。

      ("[1.2.2 连接器](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. 使用TP，在工业通信固件设置中选择CC-Link从站，并重新启动机器人控制器。**

![[Figure 1.3.8.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监视菜单中检查当前通信协议准备状态。**

![[Figure 1.3.8.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果使用Sycon.net设置的配置文件下载到对应的PCI插槽，TP设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单以进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从站插槽设置 > CC-Link从站]**

![[Figure 1.3.8.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>) 

![[Figure 1.3.8.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

**4. 每个项目的描述**

{% hint style="info" %}
   [站地址]

   - CC-Link通过站地址 (1-64) 识别从站。
{% endhint %}

{% hint style="info" %}
   [通信速度（波特率）]

   - 您可以选择156、625、2500、5000和10000 Kbit/s。
{% endhint %}

{% hint style="info" %}
   [CC-Link版本]

   - 版本1：可用IO站，不可用扩展周期

   - 版本2：不可用IO站，可用扩展周期
{% endhint %}

{% hint style="info" %}
   [占用站数]

   - IO站：占用1个

   - 远程设备：可选择1-4个

   - 分配的IO字节区域的大小取决于占用的站数。
{% endhint %}

{% hint style="info" %}
   [扩展周期]

   - 版本2中可用

   - 远程设备：您可以选择单一（1x）、双重（2x）、四重（4x）和八重（8x）。

   - 分配的IO字节区域的大小取决于扩展周期。
{% endhint %}

<br>

{% hint style="info" %}
   **有关IO字节区域的信息，请参考以下链接。**

   **(["**1.3.8.1 CC-Link从站规格](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md))**
{% endhint %}

<br>

**5. 完成设置后，请按照以下程序检查通信状态。**

有关在TP上检查工业通信状态的程序，请参考 ("[1.4 CIFX PCI通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。

![[Figure 1.3.8.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_5.png>) 

<br>

**6. 完成通信设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块来使用输入/输出信号。请参考 ("[5. 工业通信IO读写](../../../5-io-block-allocation.md)")。**
{% endhint %}
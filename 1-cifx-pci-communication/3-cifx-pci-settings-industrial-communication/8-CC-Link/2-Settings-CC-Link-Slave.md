#### 1.3.8.2 CC-Link 从站设置

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   - 对于 CC-Link 连接器连接，请参考以下内容。

      ("[1.2.2 Connector](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. 使用 TP，在工业通信固件设置中选择 CC-Link 从站并重新启动机器人控制器。**

![[Figure 1.3.8.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查当前通信协议准备状态。**

![[Figure 1.3.8.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果使用 Sycon.net 设置的配置文件下载到相应的 PCI 插槽，TP 设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单以进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI 从站插槽设置 > CC-Link 从站]**

![[Figure 1.3.8.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>) 

![[Figure 1.3.8.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

**4. 各项描述**

{% hint style="info" %}
   [站地址]

   - CC-Link 通过站地址 (1-64) 识别从站。
{% endhint %}

{% hint style="info" %}
   [通信速度 (波特率)]

   - 可以选择 156, 625, 2500, 5000 和 10000 Kbit/s。
{% endhint %}

{% hint style="info" %}
   [CC-Link 版本]

   - 版本 1: 可用 IO 站，扩展周期不可用。

   - 版本 2: 不可用 IO 站，扩展周期可用。
{% endhint %}

{% hint style="info" %}
   [占用的站数]

   - IO 站: 占用 1

   - 远程设备: 可选择 1-4

   - 分配的 IO 字节区域大小根据占用的站数而异。
{% endhint %}

{% hint style="info" %}
   [扩展周期]

   - 在版本 2 可用

   - 远程设备: 可以选择单个 (1x)、双重 (2x)、四重 (4x) 和八重 (8x)。

   - 分配的 IO 字节区域大小根据扩展周期而异。
{% endhint %}

<br>

{% hint style="info" %}
   **有关 IO 字节区域，请参考以下链接。**

   **(["**1.3.8.1 CC-Link 从站规格](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md))**
{% endhint %}

<br>

**5. 完成设置后，请按照以下程序检查通信状态。**

For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.8.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_5.png>) 

<br>

**6. 完成通信设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[5. 工业通信 IO 读写](../../../5-io-block-allocation.md)")。**
{% endhint %}
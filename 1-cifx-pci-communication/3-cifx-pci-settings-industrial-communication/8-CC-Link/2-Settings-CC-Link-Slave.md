#### 1.3.8.2 CC-Link从设备设置

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   - For CC-Link connector connection, please refer to the following.

      ("[**1.2.2 Connector**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. 使用TP选择工业通信固件设置中的CC-Link从设备，并重启机器人控制器。**

![[Figure 1.3.8.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查当前通信协议准备状态。**

![[Figure 1.3.8.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[警告]**: 如果使用Sycon.net设置的配置文件被下载到相应的PCI插槽，TP设置将被忽略。
{% endhint %}

<br>

**3. 点击菜单以进入从设备设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从设备插槽设置 > CC-Link从设备]**

![[Figure 1.3.8.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>) 

![[Figure 1.3.8.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

**4. 每个项目的描述**

{% hint style="info" %}
   [站点地址]

   - CC-Link通过站点地址（1-64）识别从设备。
{% endhint %}

{% hint style="info" %}
   [通信速度（波特率）]

   - 您可以从156、625、2500、5000和10000 Kbit/s中选择。
{% endhint %}

{% hint style="info" %}
   [CC-Link版本]

   - 版本1: 可用IO站，扩展周期不可用

   - 版本2: 不可用IO站，扩展周期可用
{% endhint %}

{% hint style="info" %}
   [占用站点计数]

   - IO站: 占用1

   - 远程设备: 可选择1-4

   - 分配的IO字节区的大小取决于占用的站点数量。
{% endhint %}

{% hint style="info" %}
   [扩展周期]

   - 版本2可用

   - 远程设备: 您可以选择单组（1x）、双组（2x）、四组（4x）和八组（8x）。

   - 分配的IO字节区的大小取决于扩展周期。
{% endhint %}

<br>

{% hint style="info" %}
   **有关IO字节区，请参阅以下链接。**

   **(["**1.3.8.1 CC-Link从设备规格**](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md))**
{% endhint %}

<br>

**5. 完成设置后，请根据以下程序检查通信状态。**

For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

<br>

**6. 完成通信设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块来使用输入/输出信号。请参阅("[**4. 工业通信IO块分配**](../../../4-io-block-allocation.md)").**
{% endhint %}
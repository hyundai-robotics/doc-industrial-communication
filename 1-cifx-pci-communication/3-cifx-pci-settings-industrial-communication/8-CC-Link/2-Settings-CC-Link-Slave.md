#### 1.3.8.2 CC-Link Slave设置

请按照“[**1.3.1 CIFX PCI槽位设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”流程设置后，再按以下方法进行操作。

<br>

{% hint style="info" %}
   - 关于CC-Link Connector的连接，请参考以下内容。

   - （“[**1.2.2 连接器**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)”）
{% endhint %}

<br>

**1. 使用TP在工业通信固件设置中选择CC-Link Slave，并重启机器人控制器。**

![[图 1.3.8.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控中，确认当前所选通信协议的准备状态。**

![[图 1.3.8.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**：如果用Sycon.net设置的Configuration文件已下载到该PCI插槽，则TP中的设定值将被忽略。
{% endhint %}

<br>

**3. 触摸菜单来进入从站设置界面。**
**\[系统 > 2：控制参数 > 11：工业通信 > 2：PCI从站插槽设置 >  CC-Link Slave]**

![[图 1.3.8.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>) 

![[图 1.3.8.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

**4. 各项目说明**

{% hint style="info" %}
   [Station Address]

   - CC-Link通过Station Address识别Slave。（1～64）
{% endhint %}

{% hint style="info" %}
   [通信速度（Baudrate）]

   - 可选择156、625、2500、5000、10000 Kbit/s。
{% endhint %}

{% hint style="info" %}
   [CC-Link Version]

   - Version 1：可使用IO Station，不可使用Extension Cycle

   - Version 2：不可使用IO Station，可使用Extension Cycle
{% endhint %}

{% hint style="info" %}
   [占用Station数]

   - IO Station：占用1个

   - Remote Device：可选择1~4个

   - 根据占用的 Station 数，分配的 IO Byte 区域大小会有所不同。
{% endhint %}

{% hint style="info" %}
   [Extension Cycle]

   - Version 2可使用

   - Remote Device：可选择1倍（Single）、2倍（Double）、4倍（Quadruple）、8倍（Octuple） 

   - 根据Extension Cycle，分配的IO Byte区域大小会有所不同。
{% endhint %}

<br>

{% hint style="info" %}
   **关于IO Byte区域，请参考以下链接。**

   **（“[**1.3.8.1 CC-Link Slave 规格**](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md)”）**
{% endhint %}

<br>

**5. 设置完成后，请按照以下流程确认通信状态。**

在TP上确认工业通信状态的程序，请参考（“[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”）。

<br>

**6. 通信设置完成后分配IO Block。**

{% hint style="info" %}
   **通信设置完成后，可以通过分配IO Block来使用输入输出信号。请确认（“[**4. 工业通信IO Block分配**](../../../4-io-block-allocation.md)”）。**
{% endhint %}
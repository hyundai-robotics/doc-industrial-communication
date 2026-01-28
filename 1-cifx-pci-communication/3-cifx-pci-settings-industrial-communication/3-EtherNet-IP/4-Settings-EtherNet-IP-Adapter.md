#### 1.3.3.4 EtherNet/IP Adapter设置

请按照“[**1.3.1 CIFX PCI槽位设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”流程设置后，再按以下方法进行操作。

<br>

{% hint style="info" %}
   **[EtherNet/IP Adapter EDS File下载]**

   - 请参考“[**5. Slave设备说明文件**](../../../5-slave-config-file.md)”。
{% endhint %}

<br>

**1. 使用TP在工业通信固件设置中选择EtherNet/IP Slave，并重启机器人控制器。**

![[图 1.3.3.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控中，确认当前所选通信协议的准备状态。**

![[图 1.3.3.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**：如果 Sycon.net 设置的 Configuration 文件已下载到该 PCI 插槽，则 TP 的设定值将被忽略。
{% endhint %}

<br>

**3. 触摸菜单来进入从站设置界面。**

**\[系统 > 2：控制参数 > 11：工业通信 > 2：PCI 从站插槽设置 >  EtherNet/IP Slave]**

![[图 1.3.3.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[图 1.3.3.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

**4. 各项目说明**

{% hint style="info" %}
   [IP设置（IP Setting）]

   - 固定IP：由用户设置IP地址、子网掩码、网关信息。

   - 动态分配（DHCP）：从DHCP服务器获取IP地址。
{% endhint %}

{% hint style="info" %}
   [通信错误时输入（Action in Bus Error）]

   - Clear：当发生通信错误时，则将所有输入初始化为0。

   - Hold：当发生通信错误时，则保持最后的有效输入值。
{% endhint %}

{% hint style="info" %}
   [通信错误允许时间（Error Allowed Time）]

   - 如果通信错误在指定的允许时间内持续存在，则将输出现场总线异常信号及报警。
{% endhint %}

{% hint style="info" %}
   [输入字节数（Input Byte）]

   - 输入字节数：设置Master -> Slave输入的数据大小。

   - O -> T：Originator(Master) -> Target (Slave)
{% endhint %}

{% hint style="info" %}
   - 【输出字节数（Output Byte）】

   - 输出字节数：设置Slave -> Master输出的数据大小。

   - T -> O：Target (Slave) -> Originator(Master)
{% endhint %}

{% hint style="info" %}
   [Run / Idle Header]

   - 应用于控制器的CIFX-50 RE EtherNet/IP Adapter在与Scanner进行IO交换时使用32Bit Run / Idle Header。（Default）

   - 请根据Scanner规格，适当设置输入/输出32Bit Run / Idle Header的使用与否。
{% endhint %}

<br>

{% hint style="info" %}
   [Quick Connect]

   - EtherNet/IP支持Quick Connect功能。

   - 如果需要使用Quick Connect功能，请使用Sycon.net设置EtherNet/IP Adapter。

   - （1） 需要支持Master、Slave Quick Connect的产品  
   - （2） 当使用Auto Negotiation时，则不可使用Quick Connect。  
   - （3） 当使用Auto MDI-X时，则不可使用Quick Connect。
   - （4） 需要使用100 Mbit/s、Full Duplex。
{% endhint %}

<br>

**5. 设置完成后，请按照以下流程确认通信状态。**

在TP上确认工业通信状态的程序，请参考（“[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”）。

![[图 1.3.3.4-5 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_5.png>) 

<br>

**6. 通信设置完成后分配IO Block。**

{% hint style="info" %}
   **通信设置完成后，可以通过分配IO Block来使用输入输出信号。请确认（“[**4. 工业通信IO Block分配**](../../../4-io-block-allocation.md)”）。**
{% endhint %}
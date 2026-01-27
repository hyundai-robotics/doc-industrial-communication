## 1.3.7.4 DeviceNet Slave设置

请按照“[**1.3.1 CIFX PCI槽位设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”流程设置后，再按以下方法进行操作。

<br>

{% hint style="info" %}
\.      **[DeviceNet Slave EDS File下载]**

\.      请参考“[**5. Slave设备说明文件**](../../../5-slave-config-file.md)”。
{% endhint %}

<br>

{% hint style="info" %}
\.      关于DeviceNet连接器的连接，请参考以下内容。

\.      （“[**1.2.2 连接器**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)”）
{% endhint %}

<br>

**1. 使用TP在工业通信固件设置中选择DeviceNet Slave，并重启机器人控制器。**

![[图 1.3.7.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控中，确认当前所选通信协议的准备状态。**

![[图 1.3.7.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**：如果用 Sycon.net 设置的 Configuration 文件已下载到该 PCI 插槽，则 TP 中的设定值将被忽略。
{% endhint %}

<br>

**3. 触摸菜单来进入从站设置界面。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI 从站插槽设置 >  DeviceNet Slave]**

![[图 1.3.7.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_3.png>) 

![[图 1.3.7.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_4.png>) 

<br>

**4. 各项目说明**

{% hint style="info" %}
\.      [Station Address = Mac ID]

\.      DeviceNet通过Station Address（MAC ID）识别Slave。（1～63）
{% endhint %}

{% hint style="info" %}
\.      [通信速度（Baudrate）]

\.      可选择125、250、500 Kbit/s中的一个。
{% endhint %}

{% hint style="info" %}
\.      [输入字节数（Input Byte）]

\.      输入字节数：设置Master -> Slave输入的数据大小。
{% endhint %}

{% hint style="info" %}
\.      [输出字节数（Output Byte）]

\.      输出字节数：设置Slave -> Master输出的数据大小。
{% endhint %}


<br>

**5. 设置完成后，请按照以下流程确认通信状态。**

在TP上确认工业通信状态的程序，请参考（“[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”）。

![[图 1.3.7.4-5 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_5.png>) 

<br>

**6. 通信设置完成后分配IO Block。**

{% hint style="info" %}
\.      **通信设置完成后，可以通过分配IO Block来使用输入输出信号。请确认（“[**4. 工业通信IO Block分配**](../../../4-io-block-allocation.md)”）。**
{% endhint %}
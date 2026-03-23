#### 1.3.7.4 DeviceNet从站设置

请遵循 "[**1.3.1 CIFX PCI插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 过程，然后继续以下方法。

<br>

{% hint style="info" %}
   **[DeviceNet从站EDS文件下载]**

   - 请参考 "[**5. 从设备描述文件**](../../../5-slave-config-file.md)." 
{% endhint %}

<br>

{% hint style="info" %}
   - 关于DeviceNet连接器连接，请参见以下内容。

      ("[**1.2.2 连接器**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. 使用TP，在工业通信固件设置中选择DeviceNet从站，并重新启动机器人控制器。**

![[图 1.3.7.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_1.png>) 

<br>

**2. 检查工业通信监控菜单中的当前通信协议就绪状态。**

![[图 1.3.7.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[警告]**: 如果使用Sycon.net设置的配置文件被下载到相应的PCI插槽，TP设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单以进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从槽设置 > DeviceNet从站]**

![[图 1.3.7.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_3.png>) 

![[图 1.3.7.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_4.png>) 

<br>

**4. 各项描述**

{% hint style="info" %}
   [站地址 = Mac ID]

   - DeviceNet通过站地址（MAC ID）识别从站（1-63）。
{% endhint %}

{% hint style="info" %}
   [通讯速度 (波特率)]

   - 您可以选择125、250和500 Kbit/s。
{% endhint %}

{% hint style="info" %}
   [输入字节计数 (输入字节)]

   - 输入字节计数：设置从主站到从站的数据输入大小。
{% endhint %}

{% hint style="info" %}
   [输出字节计数 (输出字节)]

   - 输出字节计数：设置从站到主站的数据输出大小。
{% endhint %}

<br>

**5. 完成设置后，请按照以下程序检查通信状态。**

有关在TP上检查工业通信状态的程序，请参考 ("[**1.4 CIFX PCI通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。

![[图 1.3.7.4-5 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_5.png>) 

<br>

**6. 完成通信设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块使用输入/输出信号。请参考 ("[**4. 工业通信IO块分配**](../../../4-io-block-allocation.md)").**
{% endhint %}
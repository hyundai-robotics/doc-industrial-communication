#### 1.3.7.4 DeviceNet 从站设置

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   **[DeviceNet 从站 EDS 文件下载]**

   - Please refer to "[6. 从设备描述文件](../../../6-slave-config-file.md)."
{% endhint %}

<br>

{% hint style="info" %}
   - For DeviceNet connector connection, please refer to the following.

      ("[1.2.2 连接器](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. 使用 TP，在工业通信固件设置中选择一个 DeviceNet 从站并重启机器人控制器。**

![[Figure 1.3.7.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查当前通信协议的准备状态。**

![[Figure 1.3.7.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果使用 Sycon.net 设置的配置文件下载到相应的 PCI 插槽，则 TP 设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单以进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI 从站插槽设置 > DeviceNet 从站]**

![[Figure 1.3.7.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_3.png>) 

![[Figure 1.3.7.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_4.png>) 

<br>

**4. 每个项目的描述**

{% hint style="info" %}
   [站地址 = Mac ID]

   - DeviceNet 通过站地址（MAC ID）识别从站（1-63）。
{% endhint %}

{% hint style="info" %}
   [通信速度（波特率）]

   - 您可以选择 125、250 和 500 Kbit/s。
{% endhint %}

{% hint style="info" %}
   [输入字节计数（输入字节）]

   - 输入字节计数：设置从主站 -> 从站的数据大小。
{% endhint %}

{% hint style="info" %}
   [输出字节计数（输出字节）]

   - 输出字节计数：设置从站 -> 主站的数据大小。
{% endhint %}

<br>

**5. 完成设置后，请按照以下程序检查通信状态。**

For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.7.4-5 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_5.png>) 

<br>

**6. 完成通信设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参阅 ("[5. 工业通信 IO 读写](../../../5-io-block-allocation.md)").**
{% endhint %}
#### 1.3.7.4 DeviceNet 从站设置

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   **[DeviceNet 从站 EDS 文件下载]**

   - Please refer to "[6. 从站设备描述文件](../../../6-slave-config-file.md)."
{% endhint %}

<br>

{% hint style="info" %}
   - For DeviceNet 连接器连接, please refer to the following.

      ("[1.2.2 连接器](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. Using the TP, select a DeviceNet 从站 in the industrial communication firmware settings and reboot the robot controller.**

![[Figure 1.3.7.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_1.png>) 

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.7.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the 从站设置 screen.**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI 从站槽设置 > DeviceNet 从站]**

![[Figure 1.3.7.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_3.png>) 

![[Figure 1.3.7.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_4.png>) 

<br>

**4. 每个项目的描述**

{% hint style="info" %}
   [站地址 = Mac ID]

   - The DeviceNet identifies a 从站 through the station address (MAC ID) (1-63).
{% endhint %}

{% hint style="info" %}
   [通信速度 (波特率)]

   - You can select among 125, 250, and 500 Kbit/s.
{% endhint %}

{% hint style="info" %}
   [输入字节计数 (输入字节)]

   - 输入字节计数: Sets the size of the data input from the master -> 从站.
{% endhint %}

{% hint style="info" %}
   [输出字节计数 (输出字节)]

   - 输出字节计数: Sets the size of the data output from the 从站 -> master.
{% endhint %}


<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI 通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.7.4-5 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_5.png>) 

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use 输入/输出 signals by assigning IO blocks. Please refer to ("[5. 工业通信 IO 读取和写入](../../../5-io-block-allocation.md)").**
{% endhint %}
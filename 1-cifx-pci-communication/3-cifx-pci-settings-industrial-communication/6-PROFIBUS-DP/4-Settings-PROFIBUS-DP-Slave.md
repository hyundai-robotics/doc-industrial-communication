#### 1.3.6.4 PROFIBUS-DP 从站设置

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   **[PROFIBUS-DP 从站 GSD 文件下载]**

   - Please refer to "[6. 从设备描述文件](../../../6-slave-config-file.md)".
{% endhint %}

<br>

**1. 使用 TP，在工业通信固件设置中选择一个 PROFIBUS-DP 从站，并重启机器人控制器。**

![[Figure 1.3.6.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查当前通信协议的准备状态。**

![[Figure 1.3.6.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果使用 Sycon.net 设置的配置文件下载到相应的 PCI 插槽，则 TP 设置将被忽略。
{% endhint %}

<br>

**3. 点击菜单进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI 从站插槽设置 > PROFIBUS-DP 从站]**

![[Figure 1.3.6.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.6.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

<br>

**4. 各项目的描述**

{% hint style="info" %}
   [站地址]

   - PROFIBUS-DP 通过站地址识别从站。
{% endhint %}

{% hint style="info" %}
   [输入字节计数（输入字节）]

   - 输入字节计数：设置从主控制器到从站的数据输入大小。
{% endhint %}

{% hint style="info" %}
   [输出字节计数（输出字节）]

   - 输出字节计数：设置从站到主控制器的数据输出大小。
{% endhint %}

{% hint style="info" %}
   [从主控制器设置模块时]

   - 模块应从主控制器指定，以匹配设置的字节计数。

   - 顺序：主输入 (64-1) -> 主输出 (64-1)

   - EX) 主输入 109 字节 <--- 从输出 109 字节   
         - 输入 109 字节 : 64Byte + 32Byte + 8Byte + 4Byte + 1 Byte

   - EX) 主输出 120 字节 ---> 从输入 120 字节   
         - 输出 120 字节 : 64Byte + 32Byte + 16Byte + 8Byte


   - EX) 主输入 12 字节 <--- 从输出 12 字节   
         - 输入 12 字节 : 8Byte + 4Byte

   - EX) 主输出 200 字节 ---> 从输入 200 字节   
         - 输出 200 字节 : 64Byte + 64Byte + 64Byte + 8Byte

   - 输入模块位于输出模块之前。
{% endhint %}

![[Figure 1.3.6.4-5 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>)

<br>

**5. 完成设置后，按照下面的步骤检查通信状态。**

For the procedure to check the industrial communication status on the TP, refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.6.4-6 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>)

<br>

**6. 完成通信设置后，分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，可以通过分配 IO 块来使用输入/输出信号。请参阅 ("[5. 工业通信 IO 读写](../../../5-io-block-allocation.md)")。**
{% endhint %}
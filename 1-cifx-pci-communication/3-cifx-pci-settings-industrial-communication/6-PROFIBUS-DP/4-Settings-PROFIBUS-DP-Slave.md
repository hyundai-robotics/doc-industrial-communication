#### 1.3.6.4 PROFIBUS-DP 从站设置

请按照 "[**1.3.1 CIFX PCI 插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 的程序进行操作，然后继续下面的方法。

<br>

{% hint style="info" %}
   **[PROFIBUS-DP 从站 GSD 文件下载]**

   - 请参考 "[**5. 从设备描述文件**](../../../5-slave-config-file.md)"。
{% endhint %}

<br>

**1. 使用 TP 选择工业通信固件设置中的 PROFIBUS-DP 从站，并重新启动机器人控制器。**

![[Figure 1.3.6.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查当前通信协议的准备状态。**

![[Figure 1.3.6.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**：如果通过 Sycon.net 下载的配置文件被设置到相应的 PCI 插槽，则 TP 设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单以进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI 从站插槽设置 > PROFIBUS-DP 从站]**

![[Figure 1.3.6.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.6.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

<br>

**4. 各项的描述**

{% hint style="info" %}
   [站地址]

   - PROFIBUS-DP 通过站地址识别从站。
{% endhint %}

{% hint style="info" %}
   [输入字节数 (输入字节)]

   - 输入字节数：设置从主设备 -> 从设备的数据输入大小。
{% endhint %}

{% hint style="info" %}
   [输出字节数 (输出字节)]

   - 输出字节数：设置从设备 -> 主设备的数据输出大小。
{% endhint %}

{% hint style="info" %}
   [**从主设备设置模块时**]

   - 模块应从主设备指定以匹配设置的字节数。

   - 顺序：主输入 (64-1) -> 主输出 (64-1)

   - 示例) 主输入 109 字节  <---  从输出 109 字节   
         - 输入 109 字节：64Byte + 32Byte + 8Byte + 4Byte + 1 Byte

   - 示例) 主输出 120 字节  --->  从输入 120 字节   
         - 输出 120 字节：64Byte + 32Byte + 16Byte + 8Byte


   - 示例) 主输入 12 字节  <---  从输出 12 字节   
         - 输入 12 字节：8Byte + 4Byte

   - 示例) 主输出 200 字节  --->  从输入 200 字节   
         - 输出 200 字节：64Byte + 64Byte + 64Byte + 8Byte

   - 输入模块位于输出模块之前。
{% endhint %}

![[Figure 1.3.6.4-5 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>)


<br>

**5. 完成设置后，请按照下面的程序检查通信状态。**

有关在 TP 上检查工业通信状态的程序，请参考 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。

![[Figure 1.3.6.4-6 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>)

<br>

**6. 完成通信设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[**4. 工业通信 IO 块分配**](../../../4-io-block-allocation.md)")。**
{% endhint %}
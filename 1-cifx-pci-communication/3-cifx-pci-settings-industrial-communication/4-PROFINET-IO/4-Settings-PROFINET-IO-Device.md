#### 1.3.4.4 PROFINET IO 设备设置

请遵循 "[1.3.1 CIFX PCI 插槽设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 程序，然后继续以下方法。

<br>

{% hint style="info" %}
   **[PROFINET IO 设备 GSDML 文件下载]**

   - 请参考 "[6. 从设备描述文件](../../../6-slave-config-file.md)"。
{% endhint %}

<br>

**1. 使用 TP，在工业通讯固件设置中选择一个 PROFINET IO 从设备并重启机器人控制器。**

![[Figure 1.3.4.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_1.png>)

<br>

**2. 在工业通讯监控菜单中检查当前通讯协议的准备状态。**

![[Figure 1.3.4.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果使用 Sycon.net 设置的配置文件下载到相应的 PCI 插槽，TP 设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单进入从设备设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通讯 > 2: PCI 从设备插槽设置 > PROFINET IO 从设备]**

![[Figure 1.3.4.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[Figure 1.3.4.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

**4. 各项描述**

{% hint style="info" %}
   [站名]

   - PROFINET IO 通过站名识别从设备。

   - 命名规则
      - 通过 PROFINET IO 连接的设备名称不能重复。  
      - 名称可以设置为最多 240 个字符。  
      - 可以使用特殊字符 "." 和 "-"。  
      - 可以使用小写英文字母和数字。  
      - 名称应以小写英文字母或数字开头和结尾。  
{% endhint %}

{% hint style="info" %}
   [输入字节计数 (Input Byte)]

   - 输入字节计数：设置从主设备到从设备的数据输入大小。
{% endhint %}

{% hint style="info" %}
   [输出字节计数 (Output Byte)]

   - 输出字节计数：设置从从设备到主设备的数据输出大小。
{% endhint %}

<br>

{% hint style="info" %}
   [从主设备设置插槽时]

   - 主设备输入 (32byte)  <--  从设备输出 (32bytes)

   - 主设备输出 (256bytes = 64bytes * 4)  -->  从设备输入 (256bytes)

   - 4, 8, 16, 32 和 64 字节 -> 指定与每个字节计数匹配的插槽  
   - 128 和 256 字节 -> 指定多个 64 字节插槽 (2, 4)

   - 输入插槽位于输出插槽之前。
{% endhint %}

<br>

![[Figure 1.3.4.4-5 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_5.png>) 


<br>

**5. 完成设置后，根据以下程序检查通讯状态。**

有关在 TP 上检查工业通讯状态的程序，请参见 ("[1.4 CIFX PCI 通讯监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。

![[Figure 1.3.4.4-6 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_6.png>)

<br>

**6. 完成通讯设置后分配 IO 块。**

{% hint style="info" %}
   **完成通讯设置后，您可以通过分配 IO 块使用输入/输出信号。请参考 ("[5. 工业通信 IO 读取和写入](../../../5-io-block-allocation.md)")。**
{% endhint %}
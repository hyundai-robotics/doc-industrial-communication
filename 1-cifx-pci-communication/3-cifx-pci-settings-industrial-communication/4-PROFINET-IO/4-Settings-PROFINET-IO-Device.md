#### 1.3.4.4 PROFINET IO设备设置

请遵循"[1.3.1 CIFX PCI插槽设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)"程序，然后继续以下方法。

<br>

{% hint style="info" %}
   **[PROFINET IO设备GSDML文件下载]**

   - 请参阅"[6. 从设备描述文件](../../../6-slave-config-file.md)"。
{% endhint %}

<br>

**1. 使用TP，在工业通信固件设置中选择PROFINET IO从设备并重启机器人控制器。**

![[Figure 1.3.4.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_1.png>)

<br>

**2. 在工业通信监控菜单中检查当前通信协议的就绪状态。**

![[Figure 1.3.4.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果使用Sycon.net设置的配置文件下载到相应的PCI插槽，则TP设置将被忽略。
{% endhint %}

<br>

**3. 点击菜单进入从设备设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从设备插槽设置 > PROFINET IO从设备]**

![[Figure 1.3.4.4-3 从设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[Figure 1.3.4.4-4 从设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

**4. 各项的描述**

{% hint style="info" %}
   [站名]

   - PROFINET IO通过站名识别从设备。

   - 命名规则
      - 通过PROFINET IO连接的设备名称不能重复。  
      - 名称可设置为最多240个字符。  
      - 可以使用特殊字符"."和"-"。  
      - 可以使用小写字母和数字。  
      - 名称应以小写字母或数字开头和结尾。  
{% endhint %}

{% hint style="info" %}
   [输入字节计数（输入字节）]

   - 输入字节计数：设置从主设备->从设备的数据输入大小。
{% endhint %}

{% hint style="info" %}
   [输出字节计数（输出字节）]

   - 输出字节计数：设置从设备->主设备的数据输出大小。
{% endhint %}

<br>

{% hint style="info" %}
   [从主设备设置插槽时]

   - 主设备输入（32字节）  <--  从设备输出（32字节）

   - 主设备输出（256字节 = 64字节 * 4）  -->  从设备输入（256字节）

   - 4, 8, 16, 32和64字节 -> 指定与每个字节计数匹配的插槽  
   - 128和256字节 -> 指定多个64字节插槽（2, 4）

   - 输入插槽位于输出插槽之前。
{% endhint %}

<br>

![[Figure 1.3.4.4-5 从设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_5.png>) 

<br>

**5. 完成设置后，按照以下程序检查通信状态。**

检查TP上工业通信状态的程序，请参阅("[1.4 CIFX PCI通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。

![[Figure 1.3.4.4-6 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_6.png>)

<br>

**6. 完成通信设置后，分配IO块。**

{% hint style="info" %}
   **完成通信设置后，通过分配IO块可以使用输入/输出信号。请参阅("[5. 工业通信IO读写](../../../5-io-block-allocation.md)")。**
{% endhint %}
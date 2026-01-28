#### 1.3.4.4 PROFINET IO Device设置

请按照“[**1.3.1 CIFX PCI槽位设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”流程设置后，再按以下方法进行操作。

<br>

{% hint style="info" %}
   **[PROFINET IO Device GSDML File下载]**

   - 请参考“[**5. Slave设备说明文件**](../../../5-slave-config-file.md)”。
{% endhint %}

<br>

**1. 使用TP在工业通信固件设置中选择PROFINET IO Slave，并重启机器人控制器。**

![[图 1.3.4.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控中，确认当前所选通信协议的准备状态。**

![[图 1.3.4.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果用Sycon.net设置的Configuration文件已下载到该PCI插槽，则TP中的设定值将被忽略。
{% endhint %}

<br>

**3. 触摸菜单来进入从站设置界面。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从站插槽设置 >  PROFINET IO Slave]**

![[图 1.3.4.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[图 1.3.4.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

**4. 各项目说明**

{% hint style="info" %}
   [Station Name]

   - PROFINET IO通过Station Name识别Slave。

   - Naming Rule
      - 通过PROFINET IO连接的Device名称不能重复。  
      - 名称最多可设置为240个字符。  
      - 特殊字符可使用“.”、“-”。  
      - 字符可使用英文小写字母和数字。  
      - 名称的开头和结尾必须以英文小写字母或数字组成。  
{% endhint %}

{% hint style="info" %}
   [输入字节数（Input Byte）]

   - 输入字节数：设置 Master -> Slave 输入的数据大小。
{% endhint %}

{% hint style="info" %}
   [输出字节数（Output Byte）]

   - 输出字节数：设置Slave -> Master输出的数据大小。
{% endhint %}

<br>

{% hint style="info" %}
   [**Master中设置插槽时**]

   - Master Input (32byte)  <--  Slave Output (32bytes)

   - Master Output (256bytes = 64bytes * 4)  -->  Slave Input (256bytes)

   - 4、8、16、32、64 Bytes -> 指定与各字节对应的插槽  
   - 128、256 Bytes -> 指定多个64字节插槽（2个、4个）

   - 输入插槽必须位于输出插槽之前。
{% endhint %}

<br>

![[图 1.3.4.4-5 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_5.png>) 


<br>

**5. 设置完成后，请按照以下流程确认通信状态。**

关于在TP上确认工业通信状态的程序，请参考（“[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”）。

![[图 1.3.4.4-6 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_6.png>)

<br>

**6. 通信设置完成后分配IO Block。**

{% hint style="info" %}
   **通信设置完成后，可以通过分配 IO Block 来使用输入输出信号。请确认（“[**4. 工业通信 IO Block 分配**](../../../4-io-block-allocation.md)”）。**
{% endhint %}
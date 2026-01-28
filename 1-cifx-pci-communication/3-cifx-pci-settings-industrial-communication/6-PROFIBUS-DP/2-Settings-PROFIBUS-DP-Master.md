#### 1.3.6.2 PROFIBUS-DP Master设置


请按照“[**1.3.1 CIFX PCI槽位设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”及“[**1.3.2 SYCON.NET设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)”流程设置后，再按以下方法进行操作。

<br>

{% hint style="info" %}
   - 在使用SYCON.net过程中，如有说明书中解释不足的部分，请参考“[**1.3.2 SYCON.NET帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)”功能。
{% endhint %}

<br>

**1. 在工业通信固件设置中，选择PROFIBUS-DP Master并重启机器人控制器。**

![[图 1.3.6.2-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

**2. 在工业通信监控中，确认所选协议的准备状态。**

![[图 1.3.6.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_2.png>) 

<br>

**3. 使用Sycon.net选择PROFIBUS-DP Master PCI设备。**

![[图 1.3.6.2-3 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[图 1.3.6.2-4 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

**4. 扫描PCI设备并应用PROFIBUS-DP Master（Apply）。**

![[图 1.3.6.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>


**5. 下载设置。**

![[图 1.3.6.2-6 PROFIBUS-DP Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

**6. 准备所要连接到PROFIBUS-DP Master的Slave模块。**
   * 本示例中使用Crevis公司的GN-9222 PROFIBUS-DP Slave。
   * 请提供系统电源及现场电源以激活模块。

![[图 1.3.6.2-7 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_7.png>) 


<br>

**7. Slave设备设置**

{% hint style="info" %}
   - 设置PROFIBUS-DP Slave设备的Node编号及终端。
{% endhint %}

![[图 1.3.6.2-8 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_8.png>) 


{% hint style="info" %}
   - 终端：使用DIP Switch设置终端（示例：终端处理ON）

   - Node ID（Station Number）：使用DIP Switch进行设置。（示例：Node 3号）
{% endhint %}

<br>

**8. 注册Slave设备的GSD文件。**

{% hint style="info" %}
   - 要使用未注册到Sycon.net的Device，就需要GSD文件。

   - GN-9222 Device的GSD文件可在Crevis官网下载。
{% endhint %}

![[图 1.3.6.2-9 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_9.png>)

{% hint style="info" %}
   - 将所下载的 GSD 文件注册到 Sycon.net。

   - 注册 GSD File 时，请确认工业通信协议（PROFIBUS-DP）。
{% endhint %}

![[图 1.3.6.2-10 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_10.png>)

<br>

![[图 1.3.6.5-11 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_11.png>)

![[图 1.3.6.5-12 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_12.png>)



<br>

**9. Network Scan**

{% hint style="warning" %}
   **当进行Network Scan时，请务必确认以下事项。**

   **（1） 电缆连接情况**  
   **（2） 终端DIP Switch使用情况**  
{% endhint %}

{% hint style="info" %}
   - PROFIBUS-DP Master支持Network Scan功能。
{% endhint %}

{% hint style="info" %}
   - 在PROFIBUS-DP Master设备上右击后，点击Network Scan。
{% endhint %}

![[图 1.3.6.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
   - 如果GSD文件未注册，当进行Network Scan时则会显示Slave信息，但无法注册。
{% endhint %}

{% hint style="info" %}
   - 正常注册GSD文件后，可以通过Network Scan添加Slave设备。
{% endhint %}

![[图 1.3.6.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

**10. Slave设备Configuration**

{% hint style="info" %}
   - 为了进行Slave设备Configuration，点击Master设备的Disconnect。
{% endhint %}

![[图 1.3.6.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - 双击Slave设备。
{% endhint %}

![[图 1.3.6.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_16.png>)

{% hint style="info" %}
   - 确认PROFIBUS-DP Slave的设置。

   - Slot 1 : GN-9222  
   - Slot 2 : GT-12DF (Input 2 Byte)  
   - Slot 3 : GT-227F (Output 2 Byte)  
   - Slot 4 : GT-3154 (Input 8 Byte)  
   - Slot 5 : GT-4254 (Output 8 Byte)  
{% endhint %}

![[图 1.3.6.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_17.png>)

<br>

![[图 1.3.6.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_18.png>)


<br>

**11. Master 设备 Configuration**

{% hint style="info" %}
   - 双击 Master 设备。
{% endhint %}

![[图 1.3.6.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_19.png>)


{% hint style="info" %}
   - 设置PROFIBUS-DP通信速度。

   - 9.6 ~ 12000 Kbit/s 
{% endhint %}

![[图 1.3.6.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - 请在Master设备中确认Slave设备的Slot信息是否正确。
{% endhint %}

![[图 1.3.6.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
   - 请在 Address Table 中确认各 Slave Slot 分配的 IO 及起始地址。
{% endhint %}

![[图 1.3.6.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
   - 在 Station Table 中确认各设备是否为激活状态。
{% endhint %}

![[图 1.3.6.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_23.png>)


{% hint style="info" %}
   - 设置完成后，请进行Download。
{% endhint %}

![[图 1.3.6.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

**12. 通信状态确认**

{% hint style="info" %}
   - 在 Sycon.net 及 TP 上确认通信状态。

   - 在TP上确认工业通信状态的程序，请参考（“[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”）。
{% endhint %}

{% hint style="info" %}
   - 双击已Connected的Master设备，可以确认通信状态。
{% endhint %}

![[图 1.3.6.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[图 1.3.6.2-26 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 可以利用Sycon.net的Diagnosis功能，监控通信状态及IO输入输出状态。
{% endhint %}

![[图 1.3.6.2-27 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_27.png>)

<br>

**13. 通信设置完成后分配IO Block。**

{% hint style="info" %}
   **通信设置完成后，可以通过分配IO Block来使用输入输出信号。请确认（“[**4. 工业通信IO Block分配**](../../../4-io-block-allocation.md)”）。**
{% endhint %}

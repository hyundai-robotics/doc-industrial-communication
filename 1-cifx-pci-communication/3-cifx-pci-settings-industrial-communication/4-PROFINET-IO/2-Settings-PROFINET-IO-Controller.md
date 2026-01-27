## 1.3.4.2 PROFINET IO Controller设置

请按照“[**1.3.1 CIFX PCI槽位设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”及“[**1.3.2 SYCON.NET设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)”流程设置后，再按以下方法进行操作。

<br>

{% hint style="info" %}
\.      在使用SYCON.net过程中，如有说明书中解释不足的部分，请参考“[**1.3.2 SYCON.NET帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)”功能。
{% endhint %}

<br>

**1. 在工业通信固件设置中，选择PROFINET IO Master并重启机器人控制器。**

![[图 1.3.4.2-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

**2. 在工业通信监控中，确认所选协议的准备状态。**

![[图 1.3.4.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

**3. 使用Sycon.net选择PROFINET IO Controller PCI设备。**

![[图 1.3.4.2-3 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_3.png>)
![[图 1.3.4.2-4 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

**4. 扫描PCI设备并应用PROFINET IO Controller（Apply）。**

![[图 1.3.4.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

**5. 下载设置。**

![[图 1.3.4.2-6 PROFINET IO Controller Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

**6. 准备所要连接到PROFINET IO Controller的Device（Slave）模块。**
   * 本示例中使用Crevis公司的M9287 PROFINET IO Device。
   * 请提供系统电源及现场电源以激活模块。

![[图 1.3.4.2-7 Crevis M9287]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
\.      使用DIP Switch设置PROFINET IO Device名称的方法

\.      M9287-XX：用Dip Switch设置的编号

\.      本示例中使用1号Dip Switch将名称设置为M9287-01。
{% endhint %}

<br>

**7.（Dip Switch示例）使用DIP Switch设置Slave设备的名称。**
   * 仅将 1 号 DIP Switch 更改为 ON。


![[图 1.3.4.2-8 Crevis M9287 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      DIP Switch 设置完后，请重启设备。
{% endhint %}

<br>

**8. 注册Slave设备的GSDML文件。**

{% hint style="info" %}
\.      要使用未注册到Sycon.net的Device，就需要GSDML文件。

\.      M9287 Device的GSDML文件可以在Crevis官网下载。
{% endhint %}

![[图 1.3.4.2-9 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      将所下载的 GSDML 文件注册到 Sycon.net。

\.      注册 GSDML File 时，请确认工业通信协议（PROFINET IO）。
{% endhint %}

![[图 1.3.4.2-10 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_10.png>)![[图 1.3.4.2-11 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_11.png>)
![[图 1.3.4.2-12 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_12.png>)

![[图 1.3.4.2-13 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_13.png>)


<br>

**9. Network Scan**

{% hint style="info" %}
\.      PROFINET IO Controller 支持 Network Scan 功能。
{% endhint %}

{% hint style="info" %}
\.      在 PROFINET IO Master 设备上右击后，点击 Network Scan。
{% endhint %}

![[图 1.3.4.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      如果 GSDML 文件未注册，当进行 Network Scan 时则会显示 Slave 信息，但无法注册。
{% endhint %}

![[图 1.3.4.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      正常注册GSDML文件后，可以通过Network Scan添加Slave设备。
{% endhint %}

![[图 1.3.4.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_16.png>)

![[图 1.3.4.2-17 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_17.png>)

![[图 1.3.4.2-18 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

**10. Slave（Device）设备 Configuration**

{% hint style="info" %}
\.      为了进行Slave设备Configuration，点击Master设备的Disconnect。
{% endhint %}

![[图 1.3.4.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      双击 Slave 设备。
{% endhint %}

![[图 1.3.4.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      为了设置 PROFINET IO Slave（Device），添加连接到 M9287 的 Slot。

\.      Slot 1 : M7001  
\.      Slot 2 : M12DF  
\.      Slot 3 : M225F  
{% endhint %}

![[图 1.3.4.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_21.png>)

![[图 1.3.4.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

**11. Master（Controller）设备 Configuration**

{% hint style="info" %}
\.      双击 Master 设备。
{% endhint %}

![[图 1.3.4.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      设置 Master 设备及 Slave 设备的 IP 地址。

\.      PROFINET IO Device 的 Slave IP 地址在 Master 中设置。

\.      请确保Master与Slave的IP地址在同一网段内互不重复。
{% endhint %}

![[图 1.3.4.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_24.png>)

![[图 1.3.4.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      请在 Master 设备中确认 Slave 设备的 Slot 信息是否正确。
{% endhint %}

![[图 1.3.4.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.      请在 Address Table 中确认各 Slave Slot 分配的 IO 及起始地址。
{% endhint %}

![[图 1.3.4.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.      请设置PROFINET IO的IO通信速度。
{% endhint %}

![[图 1.3.4.2-28 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.      设置完成后，请进行 Download。
{% endhint %}

![[图 1.3.4.2-29 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

**12. 通信状态确认**

{% hint style="info" %}
\.        在Sycon.net及TP上确认通信状态。

\.        在TP上确认工业通信状态的程序，请参考（“[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”）。
{% endhint %}

{% hint style="info" %}
\.      双击已Connected的Master设备，可以确认通信状态。
{% endhint %}

![[图 1.3.4.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_30.png>)

![[图 1.3.4.2-31 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
\.        可以利用Sycon.net的Diagnosis功能，监控通信状态及IO输入输出状态。
{% endhint %}

![[图 1.3.4.2-32 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_32.png>)

<br>

**13. 通信设置完成后分配IO Block。**

{% hint style="info" %}
\.      **通信设置完成后，可以通过分配IO Block来使用输入输出信号。请确认（“[**4. 工业通信IO Block分配**](../../../4-io-block-allocation.md)”）。**
{% endhint %}
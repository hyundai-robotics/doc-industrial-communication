#### 1.3.3.2 EtherNet/IP Scanner设置

请按照“[**1.3.1 CIFX PCI槽位设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”及“[**1.3.2 SYCON.NET设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)”流程设置后，再按以下方法进行操作。

<br>

{% hint style="info" %}
   - 在使用SYCON.net过程中，如有说明书中解释不足的部分，请参考“[**1.3.2 SYCON.NET帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)”功能。
{% endhint %}

<br>

**1. 在工业通信固件设置中，选择EtherNet/IP Master并重启机器人控制器。**

![[图 1.3.3.2-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_1.png>) 

<br>

**2. 在工业通信监控中，确认所选协议的准备状态。**

![[图 1.3.3.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

**3. 使用Sycon.net选择EtherNet/IP Scanner PCI设备。**

![[图 1.3.3.2-3 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_3.png>)
![[图 1.3.3.2-4 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

**4. 扫描PCI设备并应用EtherNet/IP Scanner（Apply）。**

![[图 1.3.3.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

**5. 下载设置。**

![[图 1.3.3.2-6 EtherNet/IP Scanner Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

**6. 准备所要连接到EtherNet/IP Scanner的Adapter（Slave）模块。**
   * 本示例中使用Crevis公司的M9289 EtherNet/IP Adapter。
   * 请提供系统电源及现场电源以激活模块。

![[图 1.3.3.2-7 Crevis M9289]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

**7. 设置Adapter（Slave）的IP Address，以连接EtherNet/IP通信。**

{% hint style="info" %}
   - 使用 Dip Switch 设置 IP Address
{% endhint %}

![[图 1.3.3.2-8 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
   - 使用 BootpSvr.exe 设置 IP Address 的方法
{% endhint %}

<br>

**8.（Bootp示例）使用Bootp设置Slave设备的IP Address。**
   * 仅将9号DIP Switch更改为ON。

![[图 1.3.3.2-9 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_9.png>)

   * 将PC连接到M9289 Adapter LAN端口。

![[图 1.3.3.2-10 Crevis M9289 LAN Port]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

**9. 在PC上执行BootpSvr.exe。**
   * 该程序由Crevis公司提供。（在官网下载IO Guide Pro后安装）

![[图 1.3.3.2-11 Crevis IO Guide Pro]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_11.png>)

![[图 1.3.3.2-12 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
   - 在按住 Start BootP 的状态下，断开 M9289 模块的电源并重新供电以重启。
{% endhint %}

![[图 1.3.3.2-13 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

**10. 重启Adapter设备后，在BootpSvr.exe程序中会显示Device信息。**

![[图 1.3.3.2-14 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

**11. 选择Device来设置IP。**

![[图 1.3.3.2-15 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_15.png>)![[图 1.3.3.2-16 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

**12. IP设置完成后，将Adapter的DIP Switch全部更改为OFF后重启设备。**

{% hint style="info" %}
   - 请务必确认DIP Switch的状态及Adapter是否重启。
{% endhint %}

![[图 1.3.3.2-17 Crevis DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

**13. 注册Slave设备的EDS文件。**

{% hint style="info" %}
   - 要使用未注册到Sycon.net的Device，就需要EDS文件。

   - M9289 Adapter的EDS文件可以在Crevis官网下载。
{% endhint %}

![[图 1.3.3.2-18 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
   - 将所下载的EDS文件注册到Sycon.net。

   - 注册EDS File时，请确认工业通信协议（EtherNet/IP）。
{% endhint %}

![[图 1.3.3.2-19 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_19.png>)![[图 1.3.3.2-20 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_20.png>)
![[图 1.3.3.2-21 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_21.png>)

![[图 1.3.3.2-22 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

**14. Network Scan**

{% hint style="info" %}
   - EtherNet/IP Scanner不支持Network Scan功能。
{% endhint %}

<br>

**15. Slave（Adapter）设备Configuration**

{% hint style="info" %}
   - 将已注册的Device拖到EtherNet/IP Master总线线路上。
{% endhint %}

![[图 1.3.3.2-23 Sycon.net Bus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - 双击该Device（Adapter）进行设置。

   - 根据安装该Device上的IO设备，适当设置Input / Output字节数。

   - 本示例中按如下设置。
{% endhint %}

<br>

![[图 1.3.3.2-24 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - O -> T : Originator(Master) -> Target (Slave)

   - Output : EtherNet/IP Scanner  -> M9289

   [Output Module]   
      (1) M225F (2Bytes)   
      **=> 2Bytes**   
{% endhint %}

<br>

![[图 1.3.3.2-25 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - T -> O : Target (Slave) -> Originator(Master)

   - Input : M9289 -> EtherNet/IP Scanner

   [Input Module]   
      (1) M7001  (1Byte)   
      (2) M12DF  (2Bytes)   
      **=> 3Bytes**


      (1) M7002 (0Byte)
      (2) M12DF (2Bytes)
      **=> 2Bytes**  
{% endhint %}

<br>

**16. Master（Scanner）设备 Configuration**


{% hint style="info" %}
   - 右击 Master Device 进行 Disconnect。
{% endhint %}

![[图 1.3.3.2-26 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 双击Master Device。

   - 设置Master Device的IP Address。 
{% endhint %}

![[图 1.3.3.2-27 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - 设置Slave Device的IP Address。 
{% endhint %}

![[图 1.3.3.2-28 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - 设置Slave Device的Scan Time。

   - 请调整该值来设置适当的通信速度。
{% endhint %}

![[图 1.3.3.2-29 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
   - 请在Address Table中确认Slave设备的设置。

   - 确认Input / Output IO字节数及起始Address。
{% endhint %}

![[图 1.3.3.2-30 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
   [Quick Connect]

   - EtherNet/IP支持Quick Connect功能。
{% endhint %}

{% hint style="info" %}
   - 要使用Quick Connect功能，就需要满足以下条件。

   - （1） 需要支持Master、Slave Quick Connect的产品  
   - （2） 当使用Auto Negotiation时，则不可使用Quick Connect  
   - （3） 当使用Auto MDI-X时，则不可使用Quick Connect  
   - （4） 需要使用100 Mbit/s、Full Duplex  
{% endhint %}

{% hint style="info" %}
   - 设置完成后，请进行Download。
{% endhint %}

![[图 1.3.3.2-31 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

**17. 通信状态确认**

{% hint style="info" %}
   - 在Sycon.net及TP上确认通信状态。

   - 在TP上确认工业通信状态的程序，请参考（“[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”）。
{% endhint %}

{% hint style="info" %}
   - 双击已 Connected 的 Master 设备，可以确认通信状态。
{% endhint %}

![[图 1.3.3.2-32 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_32.png>)

![[图 1.3.3.2-33 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
   - 可以利用Sycon.net的Diagnosis功能，监控通信状态及IO输入输出状态。
{% endhint %}

![[图 1.3.3.2-34 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_34.png>)

<br>

**18. 通信设置完成后分配IO Block。**

{% hint style="info" %}
   **通信设置完成后，可以通过分配IO Block来使用输入输出信号。请确认（“[**4. 工业通信IO Block分配**](../../../4-io-block-allocation.md)”）。**
{% endhint %}
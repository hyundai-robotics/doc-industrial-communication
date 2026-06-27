#### 1.3.3.2 EtherNet/IP扫描仪设置

请遵循“[1.3.1 CIFX PCI插槽设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”和“[1.3.2 SYCON.NET设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)”程序，然后继续以下方法。

<br>

{% hint style="info" %}
   - 当使用SYCON.net时，如果手册中解释不足，请参考“[1.3.2 SYCON.NET帮助](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)”功能。
{% endhint %}

<br>

**1. 在PCI插槽设置中选择EtherNet/IP主设备并重启机器人控制器。**

![[Figure 1.3.3.2-1 PCI插槽设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_1.png>)

<br>

**2. 在工业通讯监控菜单中检查所选协议的就绪状态。**

<br>

{% hint style="info" %}
   - 检查TP上的工业通信状态的程序，请参阅（"[1.4 CIFX PCI通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)"）。
{% endhint %}

<br>

![[Figure 1.3.3.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

**3. 使用Sycon.net选择EtherNet/IP扫描仪PCI设备。**

![[Figure 1.3.3.2-3 EtherNet/IP主PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_3.png>)
![[Figure 1.3.3.2-4 EtherNet/IP主PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

**4. 扫描PCI设备并应用EtherNet/IP扫描仪。**

![[Figure 1.3.3.2-5 Sycon.net扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

**5. 下载设置。**

![[Figure 1.3.3.2-6 EtherNet/IP扫描仪下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

**6. 准备连接到EtherNet/IP扫描仪的适配器（从设备）模块。**
   * 在这个例子中，我们使用来自Crevis的M9289 EtherNet/IP适配器。
   * 请提供系统电源和现场电源以激活模块。

![[Figure 1.3.3.2-7 Crevis M9289]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

**7. 设置适配器（从设备）的IP地址以进行EtherNet/IP通信连接。**

{% hint style="info" %}
   - 使用拨码开关设置IP地址。
{% endhint %}

![[Figure 1.3.3.2-8 Crevis M9289拨码开关]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
   - 使用BootpSvr.exe设置IP地址的方法
{% endhint %}

<br>

**8. (Bootp示例) 使用Bootp设置从设备的IP地址。**
   * 仅将拨码开关9更改为ON。

![[Figure 1.3.3.2-9 Crevis M9289拨码开关]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_9.png>)

   * 将PC连接到M9289适配器的LAN端口。

![[Figure 1.3.3.2-10 Crevis M9289 LAN端口]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

**9. 在PC上执行BootpSvr.exe。**
   * 该程序由Crevis提供。（从网站下载并安装IO Guide Pro。）

![[Figure 1.3.3.2-11 Crevis IO Guide Pro]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_11.png>)

![[Figure 1.3.3.2-12 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
   - 按下“启动BootP”后，断开并重新施加电源给M9289模块以重新启动它。
{% endhint %}

![[Figure 1.3.3.2-13 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

**10. 当适配器设备重新启动时，设备信息将出现在BootpSvr.exe程序中。**

![[Figure 1.3.3.2-14 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

**11. 选择设备并设置IP。**

![[Figure 1.3.3.2-15 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_15.png>)![[Figure 1.3.3.2-16 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

**12. 设置完IP后，将适配器的所有拨码开关关闭并重启设备。**

{% hint style="info" %}
   - 一定要检查拨码开关状态以及适配器是否重新启动。
{% endhint %}

![[Figure 1.3.3.2-17 Crevis DIP开关]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

**13. 注册从设备EDS文件。**

{% hint style="info" %}
   - 使用未在Sycon.net中注册的设备需要EDS文件。

   - M9289适配器的EDS文件可以从Crevis网站下载。
{% endhint %}

![[Figure 1.3.3.2-18 Crevis EDS文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
   - 在Sycon.net中注册下载的EDS文件。

   - 在注册EDS文件时，请检查工业通信协议（EtherNet/IP）。
{% endhint %}

![[Figure 1.3.3.2-19 Crevis EDS文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_19.png>)![[Figure 1.3.3.2-20 Crevis EDS文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_20.png>)
![[Figure 1.3.3.2-21 Crevis EDS文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_21.png>)

![[Figure 1.3.3.2-22 Crevis EDS文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

**14. 网络扫描**

{% hint style="info" %}
   - EtherNet/IP扫描仪不支持网络扫描功能。
{% endhint %}

<br>

**15. 配置从设备（适配器）**

{% hint style="info" %}
   - 拖动注册的设备并将其放置在EtherNet/IP主总线线。
{% endhint %}

![[Figure 1.3.3.2-23 Sycon.net总线]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - 双击设备（适配器）以进行设置。

   - 设置适配器中安装的IO设备的输入/输出字节数。

   - 在此示例中，设置如下。
{% endhint %}

<br>

![[Figure 1.3.3.2-24 适配器设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - O -> T : 发起者（主设备）-> 目标（从设备）

   - 输出 : EtherNet/IP扫描仪  -> M9289

   [输出模块]   
      (1) M225F (2Bytes)   
      **=> 2Bytes**   
{% endhint %}

<br>

![[Figure 1.3.3.2-25 适配器设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - T -> O : 目标（从设备）-> 发起者（主设备）

   - 输入 : M9289 -> EtherNet/IP扫描仪

   [输入模块]
      (1) M7001  (1Byte)
      (2) M12DF  (2Bytes)
      **=> 3Bytes**


      (1) M7002 (0Byte)
      (2) M12DF (2Bytes)
      **=> 2Bytes**  
{% endhint %}

<br>

**16. 配置主设备（扫描仪）**


{% hint style="info" %}
   - 右键单击主设备以断开连接。
{% endhint %}

![[Figure 1.3.3.2-26 适配器设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 双击主设备。

   - 设置主设备的IP地址。 
{% endhint %}

![[Figure 1.3.3.2-27 适配器设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - 设置从设备的IP地址。
{% endhint %}

![[Figure 1.3.3.2-28 扫描仪设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - 设置从设备的扫描时间。 

   - 请调整相应的值以设置适当的通信速度。
{% endhint %}

![[Figure 1.3.3.2-29 扫描仪设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
   - 在地址表中检查从设备的设置。

   - 检查输入/输出IO字节数和起始地址。
{% endhint %}

![[Figure 1.3.3.2-30 扫描仪设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
   [快速连接]

   - EtherNet/IP支持快速连接功能。
{% endhint %}

{% hint style="info" %}
   - 使用快速连接功能需要满足以下条件。

      (1) 需要支持快速连接功能的主设备和从设备  
      (2) 在使用自动协商时无法使用快速连接  
      (3) 在使用自动MDI-X时无法使用快速连接  
      (4) 需要100 Mbit/s，全双工  
{% endhint %}

{% hint style="info" %}
   - 设置完成后，进行下载。
{% endhint %}

![[Figure 1.3.3.2-31 扫描仪设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

**17. 检查通信状态**

{% hint style="info" %}
   - 在Sycon.net和TP中检查通信状态。

   - 检查TP上的工业通信状态的程序，请参阅（"[1.4 CIFX PCI通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)"）。
{% endhint %}

{% hint style="info" %}
   - 双击连接的主设备以检查通信状态。
{% endhint %}

![[Figure 1.3.3.2-32 通信状态]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_32.png>)

![[Figure 1.3.3.2-33 通信状态]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
   - 使用Sycon.net的诊断功能，可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.3.2-34 通信状态]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_34.png>)

<br>

**18. 完成通信设置后分配IO块。**

{% hint style="info" %}
**完成通信设置后，可以通过分配 IO 块来使用输入/输出信号。请参考 ("[5. 工业通信 IO 读取和写入](../../../5-io-block-allocation.md)")。**  
{% endhint %}
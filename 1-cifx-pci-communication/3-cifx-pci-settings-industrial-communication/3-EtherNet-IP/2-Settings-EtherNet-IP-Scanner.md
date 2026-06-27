#### 1.3.3.2 EtherNet/IP 扫描器设置

请遵循 "[1.3.1 CIFX PCI 插槽设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 和 "[1.3.2 SYCON.NET 设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 过程，然后按照以下方法进行。

<br>

{% hint style="info" %}
   - 在使用 SYCON.net 时，如果手册中缺乏说明，请参阅 "[1.3.2 SYCON.NET 帮助](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" 功能。
{% endhint %}

<br>

**1. 在 PCI 插槽设置中选择 EtherNet/IP 主机并重启机器人控制器。**

![[Figure 1.3.3.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_1.png>)

<br>

**2. 在工业通信监控菜单中检查所选协议的就绪状态。**

<br>

{% hint style="info" %}
   - 要查看在 TP 上检查工业通信状态的过程，请参阅 ("[1.4 CIFX PCI 通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

<br>

![[Figure 1.3.3.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

**3. 使用 Sycon.net 选择 EtherNet/IP 扫描器 PCI 设备。**

![[Figure 1.3.3.2-3 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_3.png>)
![[Figure 1.3.3.2-4 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

**4. 扫描 PCI 设备并应用 EtherNet/IP 扫描器。**

![[Figure 1.3.3.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

**5. 下载设置。**

![[Figure 1.3.3.2-6 EtherNet/IP Scanner Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

**6. 准备要连接到 EtherNet/IP 扫描器的适配器（从设备）模块。**
   * 在本例中，我们使用 Crevis 的 M9289 EtherNet/IP 适配器。
   * 请供电给系统电源和现场电源以启用该模块。

![[Figure 1.3.3.2-7 Crevis M9289]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

**7. 设置适配器（从设备）的 IP 地址以进行 EtherNet/IP 通信连接。**

{% hint style="info" %}
   - 使用拨码开关设置 IP 地址。
{% endhint %}

![[Figure 1.3.3.2-8 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
   - 如何使用 BootpSvr.exe 设置 IP 地址
{% endhint %}

<br>

**8. （Bootp 示例）使用 Bootp 设置从设备的 IP 地址。**
   * 仅将 DIP 开关 9 更改为 ON。

![[Figure 1.3.3.2-9 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_9.png>)

   * 将 PC 连接到 M9289 适配器的 LAN 端口。

![[Figure 1.3.3.2-10 Crevis M9289 LAN Port]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

**9. 在 PC 上执行 BootpSvr.exe。**
   * 该程序由 Crevis 提供。 （从网站下载并安装 IO Guide Pro。）

![[Figure 1.3.3.2-11 Crevis IO Guide Pro]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_11.png>)

![[Figure 1.3.3.2-12 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
   - 按下“开始 BootP”时，请断开并重新供电给 M9289 模块以重新启动其。
{% endhint %}

![[Figure 1.3.3.2-13 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

**10. 当适配器设备重新启动时，设备信息将出现在 BootpSvr.exe 程序中。**

![[Figure 1.3.3.2-14 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

**11. 选择设备并设置 IP。**

![[Figure 1.3.3.2-15 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_15.png>)![[Figure 1.3.3.2-16 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

**12. 设置 IP 后，将适配器的所有 DIP 开关都切换为 OFF 并重启设备。**

{% hint style="info" %}
   - 确保检查 DIP 开关状态及适配器是否已重新启动。
{% endhint %}

![[Figure 1.3.3.2-17 Crevis DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

**13. 注册从设备 EDS 文件。**

{% hint style="info" %}
   - 使用未在 Sycon.net 中注册的设备需要 EDS 文件。

   - M9289 适配器的 EDS 文件可以从 Crevis 网站下载。
{% endhint %}

![[Figure 1.3.3.2-18 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
   - 在 Sycon.net 中注册下载的 EDS 文件。

   - 注册 EDS 文件时，请检查工业通信协议（EtherNet/IP）。
{% endhint %}

![[Figure 1.3.3.2-19 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_19.png>)![[Figure 1.3.3.2-20 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_20.png>)
![[Figure 1.3.3.2-21 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_21.png>)

![[Figure 1.3.3.2-22 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

**14. 网络扫描**

{% hint style="info" %}
   - EtherNet/IP 扫描器不支持网络扫描功能。
{% endhint %}

<br>

**15. 配置从设备（适配器）**

{% hint style="info" %}
   - 拖动注册的设备并将其放置在 EtherNet/IP 主站总线线中。
{% endhint %}

![[Figure 1.3.3.2-23 Sycon.net Bus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - 双击设备（适配器）以继续设置。

   - 设置适合安装在该设备中的 IO 设备的输入/输出字节数。

   - 在本例中，设置如下。
{% endhint %}

<br>

![[Figure 1.3.3.2-24 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - O -> T : 原发器（主机） -> 目标（从设备）

   - 输出 : EtherNet/IP 扫描器  -> M9289

   [输出模块]   
      (1) M225F (2Bytes)   
      **=> 2Bytes**   
{% endhint %}

<br>

![[Figure 1.3.3.2-25 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - T -> O : 目标（从设备） -> 原发器（主机）

   - 输入 : M9289 -> EtherNet/IP 扫描器

   [输入模块]
      (1) M7001  (1Byte)
      (2) M12DF  (2Bytes)
      **=> 3Bytes**


      (1) M7002 (0Byte)
      (2) M12DF (2Bytes)
      **=> 2Bytes**  
{% endhint %}

<br>

**16. 配置主设备（扫描器）。**

{% hint style="info" %}
   - 右键单击主设备以断开连接。
{% endhint %}

![[Figure 1.3.3.2-26 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 双击主设备。

   - 设置主设备 IP 地址。 
{% endhint %}

![[Figure 1.3.3.2-27 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - 设置从设备 IP 地址。
{% endhint %}

![[Figure 1.3.3.2-28 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - 设置从设备扫描时间。 

   - 请调整相应的值以设置适当的通信速度。
{% endhint %}

![[Figure 1.3.3.2-29 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
   - 在地址表中检查从设备设置。

   - 检查输入/输出 IO 字节数和起始地址。
{% endhint %}

![[Figure 1.3.3.2-30 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
   [快速连接]

   - EtherNet/IP 支持快速连接功能。
{% endhint %}

{% hint style="info" %}
   - 使用快速连接功能需满足以下条件。

      (1) 必须有支持快速连接功能的主机和从设备  
      (2) 使用自动协商时不能使用快速连接  
      (3) 使用自动 MDI-X 时不能使用快速连接  
      (4) 需要 100 Mbit/s, 全双工  
{% endhint %}

{% hint style="info" %}
   - 完成设置后，进行下载。
{% endhint %}

![[Figure 1.3.3.2-31 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

**17. 检查通信状态**

{% hint style="info" %}
   - 在 Sycon.net 和 TP 中检查通信状态。

   - 要查看在 TP 上检查工业通信状态的过程，请参阅 ("[1.4 CIFX PCI 通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

{% hint style="info" %}
   - 双击连接的主设备以检查通信状态。
{% endhint %}

![[Figure 1.3.3.2-32 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_32.png>)

![[Figure 1.3.3.2-33 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
   - 使用 Sycon.net 的诊断功能，您可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.3.2-34 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_34.png>)

<br>

**18. 完成通信设置后分配 IO 块。**

{% hint style="info" %}
**完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**  
{% endhint %}
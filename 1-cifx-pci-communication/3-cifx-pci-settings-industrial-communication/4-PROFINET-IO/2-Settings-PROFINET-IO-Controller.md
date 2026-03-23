#### 1.3.4.2 PROFINET IO 控制器设置

请遵循 "[**1.3.1 CIFX PCI 插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 和 "[**1.3.2 SYCON.NET 设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 程序，然后继续以下方法。

<br>

{% hint style="info" %}
   - 使用 SYCON.net 时，如果手册中的说明不足，请参考 "[**1.3.2 SYCON.NET 帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" 功能。
{% endhint %}

<br>

**1. 在 PCI 插槽设置中选择 PROFINET IO 主控并重启机器人控制器。**

![[Figure 1.3.4.2-1 PCI 插槽设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查所选协议的就绪状态。**

<br>

{% hint style="info" %}
   - 有关在 TP 上检查工业通信状态的程序，请参考 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

<br>

![[Figure 1.3.4.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

**3. 使用 Sycon.net 选择 PROFINET IO 控制器 PCI 设备。**

![[Figure 1.3.4.2-3 PROFINET IO 主控 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_3.png>)
![[Figure 1.3.4.2-4 PROFINET IO 主控 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

**4. 扫描 PCI 设备并应用 PROFINET IO 控制器。**

![[Figure 1.3.4.2-5 Sycon.net 扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

**5. 下载设置。**

![[Figure 1.3.4.2-6 PROFINET IO 控制器下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

**6. 准备要连接到 PROFINET IO 控制器的设备（从属）模块。**
   * 在本示例中，我们使用 Crevis 的 M9287 PROFINET IO 设备。
   * 请供应系统电源和现场电源以激活模块。

![[Figure 1.3.4.2-7 Crevis M9287]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
   - 如何使用 DIP 开关设置 PROFINET IO 设备名称

   - M9287-XX: 使用 DIP 开关设置的编号

   - 在本示例中，名称使用 DIP 开关 1 设置为 M9287-01。
{% endhint %}

<br>

**7. （DIP 开关使用示例）使用 DIP 开关设置从属设备名称。**
   * 仅更改 DIP 开关 1 为 ON。

![[Figure 1.3.4.2-8 Crevis M9287 DIP 开关]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
   - 设置 DIP 开关后，请重启设备。
{% endhint %}

<br>

**8. 注册从属设备 GSDML 文件。**

{% hint style="info" %}
   - 使用未在 Sycon.net 中注册的设备时，需要 GSDML 文件。

   - M9287 设备的 GSDML 文件可以从 Crevis 网站下载。
{% endhint %}

![[Figure 1.3.4.2-9 Crevis GSDML 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
   - 在 Sycon.net 中注册下载的 GSDML 文件。

   - 注册 GSDML 文件时，请检查工业通信协议（PROFINET IO）。
{% endhint %}

![[Figure 1.3.4.2-10 Crevis GSDML 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_10.png>)![[Figure 1.3.4.2-11 Crevis GSDML 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_11.png>)
![[Figure 1.3.4.2-12 Crevis GSDML 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_12.png>)

![[Figure 1.3.4.2-13 Crevis GSDML 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_13.png>)

<br>

**9. 网络扫描**

{% hint style="info" %}
   - PROFINET IO 控制器支持网络扫描功能。
{% endhint %}

{% hint style="info" %}
   - 右击 PROFINET IO 主控设备并单击网络扫描。
{% endhint %}

![[Figure 1.3.4.2-14 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
   - 如果没有注册 GSDML 文件，则在执行网络扫描功能时，将出现从属信息，但无法注册。
{% endhint %}

![[Figure 1.3.4.2-15 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - 如果正常注册了 GSDML 文件，则可以使用网络扫描功能添加从属设备。
{% endhint %}

![[Figure 1.3.4.2-16 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_16.png>)

![[Figure 1.3.4.2-17 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_17.png>)

![[Figure 1.3.4.2-18 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

**10. 配置从属（设备）。**

{% hint style="info" %}
   - 单击主控设备上的断开连接以配置从属设备。
{% endhint %}

![[Figure 1.3.4.2-19 从属配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - 双击从属设备。
{% endhint %}

![[Figure 1.3.4.2-20 从属配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - 添加连接到 M9287 的插槽以设置 PROFINET IO 从属（设备）。

   - 插槽 1 : M7001  
   - 插槽 2 : M12DF  
   - 插槽 3 : M225F  
{% endhint %}

![[Figure 1.3.4.2-21 从属配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_21.png>)

![[Figure 1.3.4.2-22 从属配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

**11. 配置主控（控制器）设备**

{% hint style="info" %}
   - 双击主控设备。
{% endhint %}

![[Figure 1.3.4.2-23 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - 设置主控和从属设备的 IP 地址。

   - PROFINET IO 设备的从属 IP 地址应从主控设置。

   - 请确保主控和从属的 IP 地址在同一段内不重叠。
{% endhint %}

![[Figure 1.3.4.2-24 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_24.png>)

![[Figure 1.3.4.2-25 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - 从主控设备检查从属设备的插槽信息是否正确。
{% endhint %}

![[Figure 1.3.4.2-26 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 在地址表中检查每个从属插槽的 IO 和起始地址分配。
{% endhint %}

![[Figure 1.3.4.2-27 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - 设置 PROFINET IO 的 IO 通信速度。
{% endhint %}

![[Figure 1.3.4.2-28 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - 完成设置后，请继续下载。
{% endhint %}

![[Figure 1.3.4.2-29 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

**12. 检查通信状态。**

{% hint style="info" %}
   - 在 Sycon.net 和 TP 中检查通信状态。

   - 有关在 TP 上检查工业通信状态的程序，请参阅 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

{% hint style="info" %}
   - 双击连接的主控设备以检查通信状态。
{% endhint %}

![[Figure 1.3.4.2-30 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_30.png>)

![[Figure 1.3.4.2-31 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
   - 使用 Sycon.net 的诊断功能，您可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.4.2-32 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_32.png>)

<br>

**13. 在完成设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参见 ("[**4. 工业通信 IO 块分配**](../../../4-io-block-allocation.md)")。**
{% endhint %}
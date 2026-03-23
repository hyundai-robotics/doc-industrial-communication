#### 1.3.5.2 EtherCAT主控设置

请遵循 "[**1.3.1 CIFX PCI插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 和 "[**1.3.2 SYCON.NET设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 的步骤，然后按下面的方法进行。

<br>

{% hint style="info" %}
   - 使用SYCON.net时，如果手册中的解释不足，请参考 "[**1.3.2 SYCON.NET帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" 功能。
{% endhint %}

<br>

**1.在PCI插槽设置中选择EtherCAT主控并重启机器人控制器。**

![[Figure 1.3.5.2-1 PCI插槽设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_1.png>) 

<br>

**2.在工业通信监控菜单中检查所选协议的就绪状态。**

<br>

{% hint style="info" %}
   - 检查TP上工业通信状态的程序，请参阅 ("[**1.4 CIFX PCI通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

<br>

![[Figure 1.3.5.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_2.png>) 

<br>

**3.使用Sycon.net选择EtherCAT主控PCI设备。**

![[Figure 1.3.5.2-3 EtherCAT主控PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_3.png>)
![[Figure 1.3.5.2-4 EtherCAT主控PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_4.png>) 

<br>

**4.扫描PCI设备并应用EtherCAT主控。**

![[Figure 1.3.5.2-5 Sycon.net扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_5.png>) 

<br>

**5.下载设置。**

![[Figure 1.3.5.2-6 EtherCAT主控下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_6.png>) 

<br>

**6.准备要连接到EtherCAT主控的从模块。**
   * 在本例中，我们使用Crevis的M9386 EtherCAT从设备。
   * 请供电系统电源和现场电源以激活模块。

![[Figure 1.3.5.2-7 Crevis M9386]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_7.png>) 

<br>

**7.从设备站地址**

{% hint style="info" %}
   - EtherCAT从设备的站地址由主控设置。
{% endhint %}

<br>

**8.注册从设备XML文件。**

{% hint style="info" %}
   - 使用未在Sycon.net中注册的设备需要XML文件。

   - M9386设备的XML文件可以从Crevis官网上下载。
{% endhint %}

![[Figure 1.3.5.2-8 Crevis XML文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_8.png>)

{% hint style="info" %}
   - 在Sycon.net中注册下载的XML文件。

   - 注册XML文件时，请检查工业通信协议（EtherCAT）。
{% endhint %}

![[Figure 1.3.5.2-9 Crevis XML文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_9.png>)

<br>

![[Figure 1.3.5.5-10 Crevis XML文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.5.2-11 Crevis XML文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_11.png>)

<br>

![[Figure 1.3.5.2-12 Crevis XML文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_12.png>)


<br>

**9.网络扫描**

{% hint style="warning" %}
   **对于EtherCAT，指定了可用的电缆连接和端口。**

   **为了顺畅的通信连接，务必检查 ("[**1.3.5.5 EtherCAT电缆布线**](../5-EtherCAT/5-EtherCAT-Topology.md)")。**
{% endhint %}

{% hint style="info" %}
   - EtherCAT主控支持网络扫描功能。
{% endhint %}

{% hint style="info" %}
   - 右键单击EtherCAT主控设备，点击网络扫描。
{% endhint %}

![[Figure 1.3.5.2-13 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_13.png>)

{% hint style="warning" %}
   - 如果没有注册XML文件，进行网络扫描功能时将出现从设备信息，但无法注册。
{% endhint %}

{% hint style="info" %}
   - 如果XML文件正常注册，则可以使用网络扫描功能添加从设备。
{% endhint %}

![[Figure 1.3.5.2-14 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_14.png>)

<br>

**10.配置从设备。**

{% hint style="info" %}
   - 点击主控设备上的断开以配置从设备。
{% endhint %}

![[Figure 1.3.5.2-15 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - 双击从设备。
{% endhint %}

![[Figure 1.3.5.2-16 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_16.png>)

{% hint style="info" %}
   - 添加连接到M9386的插槽以设置EtherCAT从设备。

   - 插槽1：M7001  
   - 插槽2：M12DF  
   - 插槽3：M225F  
{% endhint %}

![[Figure 1.3.5.2-17 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_17.png>)

![[Figure 1.3.5.2-18 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_18.png>)


<br>

**11.配置主设备。**

{% hint style="info" %}
   - 双击主设备。
{% endhint %}

![[Figure 1.3.5.2-19 主设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - 同步：选择Freerun/DC（分布时钟）。

   - 是否使用冗余（不能与分布时钟同时使用）

   - 总线周期时间：至少支持250 us。（建议1 ms或更长。）
{% endhint %}

<br>

{% hint style="info" %}
   - 您可以为每个从设备设置站地址。
{% endhint %}

![[Figure 1.3.5.2-20 主设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - 检查地址表中每个从设备插槽的分配IO和起始地址。
{% endhint %}

![[Figure 1.3.5.2-21 主设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_21.png>)


{% hint style="info" %}
   - 完成设置后，继续下载。
{% endhint %}

![[Figure 1.3.5.2-22 主设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_22.png>)

<br>

**12.检查通信状态。**

{% hint style="info" %}
   - 在Sycon.net和TP中检查通信状态。

   - 检查TP上的工业通信状态程序，请参阅 ("[**1.4 CIFX PCI通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

{% hint style="info" %}
   - 双击连接的主设备以检查通信状态。
{% endhint %}

![[Figure 1.3.5.2-23 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_23.png>)

![[Figure 1.3.5.2-24 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - 使用Sycon.net的诊断功能，您可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.5.2-25 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_25.png>)

<br>

**13.完成设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块来使用输入/输出信号。请参阅 ("[**4.工业通信IO块分配**](../../../4-io-block-allocation.md)")。**
{% endhint %}
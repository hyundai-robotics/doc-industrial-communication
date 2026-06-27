#### 1.3.6.2 PROFIBUS-DP 主设置

请按照 "[1.3.1 CIFX PCI 插槽设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 和 "[1.3.2 SYCON.NET 设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 的程序，然后进行以下方法。

<br>

{% hint style="info" %}
   - 使用 SYCON.net 时，如果手册中没有足够的说明，请参考 "[1.3.2 SYCON.NET 帮助](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" 功能。
{% endhint %}

<br>

**1. 在 PCI 插槽设置中选择 PROFIBUS-DP 主站并重启机器人控制器。**

![[Figure 1.3.6.2-1 PCI 插槽设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查所选协议的就绪状态。**

<br>

{% hint style="info" %}
   - 检查 TP 上工业通信状态的步骤，请参考 ("[1.4 CIFX PCI 通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

<br>

![[Figure 1.3.6.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_2.png>)

<br>

**3. 使用 Sycon.net 选择 PROFIBUS-DP 主 PCI 设备。**

![[Figure 1.3.6.2-3 PROFIBUS-DP 主 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[Figure 1.3.6.2-4 PROFIBUS-DP 主 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

**4. 扫描 PCI 设备并应用 PROFIBUS-DP 主站。**

![[Figure 1.3.6.2-5 Sycon.net 扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>

**5. 下载设置。**

![[Figure 1.3.6.2-6 PROFIBUS-DP 主下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

**6. 准备要连接到 PROFIBUS-DP 主站的从模块。**
   * 在本例中，我们使用来自 Crevis 的 GN-9222 PROFIBUS-DP 从属设备。
   * 请提供系统电源和现场电源以启动模块。

![[Figure 1.3.6.2-7 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_7.png>) 

<br>

**7. 设置从设备**

{% hint style="info" %}
   - 设置 PROFIBUS-DP 从设备的节点号和终端。
{% endhint %}

![[Figure 1.3.6.2-8 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
   - 终端：使用 DIP 开关设置（示例：终端处理开启）

   - 节点 ID（站号）：使用 DIP 开关设置（示例：节点 3）
{% endhint %}

<br>

**8. 注册从设备 GSD 文件。**

{% hint style="info" %}
   - 使用未在 Sycon.net 中注册的设备需要 GSD 文件。

   - GN-9222 设备的 GSD 文件可以从 Crevis 网站下载。
{% endhint %}

![[Figure 1.3.6.2-9 Crevis GSD 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_9.png>)

{% hint style="info" %}
   - 在 Sycon.net 中注册下载的 GSD 文件。

   - 注册 GSD 文件时，请检查工业通信协议（PROFIBUS-DP）。
{% endhint %}

![[Figure 1.3.6.2-10 Crevis GSD 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.6.5-11 Crevis GSD 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_11.png>)

![[Figure 1.3.6.5-12 Crevis GSD 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_12.png>)

<br>

**9. 网络扫描**

{% hint style="warning" %}
   **进行网络扫描功能时，请确保检查以下内容。**

   **(1) 是否连接了电缆。**  
   **(2) 是否使用了终端 DIP 开关。**  
{% endhint %}

{% hint style="info" %}
   - PROFIBUS-DP 主站支持网络扫描功能。
{% endhint %}

{% hint style="info" %}
   - 右键单击 PROFIBUS-DP 主设备并单击网络扫描。
{% endhint %}

![[Figure 1.3.6.2-13 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
   - 如果没有注册 GSD 文件，执行网络扫描功能时会出现从设备信息，但无法注册。
{% endhint %}

{% hint style="info" %}
   - 如果 GSD 文件正常注册，可以使用网络扫描功能添加从设备。
{% endhint %}

![[Figure 1.3.6.2-14 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

**10. 配置从设备**

{% hint style="info" %}
   - 点击主设备上的断开连接，以配置从设备。
{% endhint %}

![[Figure 1.3.6.2-15 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - 双击从设备。
{% endhint %}

![[Figure 1.3.6.2-16 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_16.png>)

{% hint style="info" %}
   - 检查 PROFIBUS-DP 从设备设置。

   - 插槽 1 : GN-9222  
   - 插槽 2 : GT-12DF（输入 2 字节）  
   - 插槽 3 : GT-227F（输出 2 字节）  
   - 插槽 4 : GT-3154（输入 8 字节）  
   - 插槽 5 : GT-4254（输出 8 字节）  
{% endhint %}

![[Figure 1.3.6.2-17 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_17.png>)

<br>

![[Figure 1.3.6.2-18 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_18.png>)

<br>

**11. 配置主设备。**

{% hint style="info" %}
   - 双击主设备。
{% endhint %}

![[Figure 1.3.6.2-19 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - 设置 PROFIBUS-DP 通信速度。

   - 9.6 - 12000 Kbit/s 
{% endhint %}

![[Figure 1.3.6.2-20 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - 从主设备检查从设备的插槽信息是否正确。
{% endhint %}

![[Figure 1.3.6.2-21 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
   - 在地址表中检查每个从插槽分配的 IO 和起始地址。
{% endhint %}

![[Figure 1.3.6.2-22 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
   - 检查站表中的每个设备是否处于活动状态。
{% endhint %}

![[Figure 1.3.6.2-23 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - 完成设置后，请继续下载。
{% endhint %}

![[Figure 1.3.6.2-24 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

**12. 检查通信状态。**

{% hint style="info" %}
   - 在 Sycon.net 和 TP 中检查通信状态。

   - 检查 TP 上工业通信状态的过程，请参考 ("[1.4 CIFX PCI 通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

{% hint style="info" %}
   - 双击连接的主设备以检查通信状态。
{% endhint %}

![[Figure 1.3.6.2-25 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[Figure 1.3.6.2-26 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 使用 Sycon.net 的诊断功能，您可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.6.2-27 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_27.png>)

<br>

**13. 完成设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[5. 工业通信 IO 读取和写入](../../../5-io-block-allocation.md)")。**
{% endhint %}
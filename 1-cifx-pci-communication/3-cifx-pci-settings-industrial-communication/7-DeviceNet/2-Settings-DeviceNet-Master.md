#### 1.3.7.2 DeviceNet 主设置

请遵循 "[1.3.1 CIFX PCI 插槽设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 和 "[1.3.2 SYCON.NET 设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 程序，然后继续下面的方法。

<br>

{% hint style="info" %}
   - 使用 SYCON.net 时，如果手册中说明不够，请参阅 "[1.3.2 SYCON.NET 帮助](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" 功能。
{% endhint %}

<br>

{% hint style="info" %}
   - 有关 DeviceNet 连接器连接，请参阅以下内容。

      ("[1.2.2 连接器](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. 在 PCI 插槽设置中选择 DeviceNet 主设备，并重启机器人控制器。**

![[Figure 1.3.7.2-1 PCI 插槽设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_1.png>)

<br>

**2. 在工业通信监控菜单中检查所选协议的准备状态。**

<br>

{% hint style="info" %}
   - 有关在 TP 上检查工业通信状态的程序，请参阅 ("[1.4 CIFX PCI 通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

<br>

![[Figure 1.3.7.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_2.png>)

<br>

**3. 使用 Sycon.net 选择 DeviceNet 主 PCI 设备。**

![[Figure 1.3.7.2-3 DeviceNet 主 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_3.png>)
![[Figure 1.3.7.2-4 DeviceNet 主 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_4.png>)

<br>

**4. 扫描 PCI 设备并应用 DeviceNet 主设备。**

![[Figure 1.3.7.2-5 Sycon.net 扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_5.png>)

<br>

**5. 设置通信速度。**

{% hint style="warning" %}
   - 如果主设备和从设备之间通信速度不同，则网络扫描功能无法正常工作。
{% endhint %}

![[Figure 1.3.7.2-6 DeviceNet 主下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_6.png>)

<br>

**6. 下载设置。**

![[Figure 1.3.7.2-7 DeviceNet 主下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_7.png>)

<br>

**7. 准备要连接到 DeviceNet 主设备的从模块。**
   * 在此示例中，我们使用来自 Crevis 的 NA-9211 DeviceNet 从设备。
   * 请为模块提供系统电源和现场电源以激活模块。

![[Figure 1.3.7.2-8 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_8.png>)

<br>

**8. 设置从设备。**

{% hint style="info" %}
   - 设置 DeviceNet 从设备的 MAC ID、通信速度和终端电阻。
{% endhint %}

![[Figure 1.3.7.2-9 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_9.png>)

![[Figure 1.3.7.2-10 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_10.png>)

{% hint style="info" %}
   [示例设置]

   - 终端电阻：通过安装在电缆中使用（终端 DIP 开关关闭）

   - MAC ID（站号）：设置为 4（仅 DIP 开关 3 为开启状态。）

   - 通信速度（波特率）：设置为自动（DIP 开关 7 和 8 为开启状态。）
{% endhint %}

<br>

**9. 注册从设备 EDS 文件。**

{% hint style="info" %}
   - 使用未在 Sycon.net 中注册的设备时需要 EDS 文件。

   - NA-9211 设备的 EDS 文件可以从 Crevis 网站下载。
{% endhint %}

![[Figure 1.3.7.2-11 Crevis EDS 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_11.png>)

{% hint style="info" %}
   - 在 Sycon.net 中注册所有下载的 EDS 文件。

   - 注册 EDS 文件时，请检查工业通信协议（DeviceNet）。
{% endhint %}

![[Figure 1.3.7.2-12 Crevis EDS 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_12.png>)

<br>

![[Figure 1.3.7.5-13 Crevis EDS 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_13.png>)

<br>

**10. 网络扫描**

{% hint style="warning" %}
   **进行网络扫描功能时，请务必检查以下内容。**

   **(1) 是否连接了电缆。**  
   **(2) 是否连接了终端电阻或使用了终端 DIP 开关。**  
   **(3) 主从通信速度是否设置。**  

   **为了实现顺畅的通信连接，请务必检查 ("[1.3.7.5 DeviceNet 错误处理](../7-DeviceNet/5-Error-DeviceNet.md)")。**
{% endhint %}

{% hint style="info" %}
   - DeviceNet 主设备支持网络扫描功能。
{% endhint %}

{% hint style="info" %}
   - 右键单击 DeviceNet 主设备并单击网络扫描。
{% endhint %}

![[Figure 1.3.7.2-14 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
   - 如果没有注册 EDS 文件，则在执行网络扫描功能时会显示从设备信息，但无法注册。
{% endhint %}

{% hint style="info" %}
   - 如果正常注册了 EDS 文件，则可以使用网络扫描功能添加从设备。
{% endhint %}

![[Figure 1.3.7.2-15 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_15.png>)
![[Figure 1.3.7.2-16 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_16.png>)

<br>

**11. 配置从设备**

{% hint style="info" %}
   - 单击主设备上的断开连接以配置从设备。
{% endhint %}

![[Figure 1.3.7.2-17 从配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
   - 双击从设备。
{% endhint %}

![[Figure 1.3.7.2-18 从配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_18.png>)

<br>

{% hint style="info" %}
   - 设置从设备的连接类型。

   - 选择 DeviceNet 通信连接的消息传输方式。

   **如果未选中 UCMM 复选框，则默认值设置为 UCMM 组 2。**

   - UCMM 组 1 : IO 消息  
   - UCMM 组 2: 网络初始化期间的主从连接消息（默认设置）  
   - UCMM 组 3: 明确消息  

   - 对于某些设备，UCMM 组 3 可能会被使用，因此在进行之前请检查产品规格。
{% endhint %}

![[Figure 1.3.7.2-19 从配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_19.png>)

<br>

{% hint style="info" %}
   - 对于 Crevis NA-9211，进行时无需勾选 UCMM 复选框。（使用组 2 默认值。）
{% endhint %}

![[Figure 1.3.7.2-20 从配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_20.png>)

<br>

{% hint style="info" %}
   - 检查 DeviceNet 从设备的设置。

   - 输出：ST-2318 (1 字节)  
   - 输入：ST-1218 (1 字节)  
{% endhint %}

<br>

{% hint style="info" %}
   - 需要根据通信方式（轮询、状态变化、循环、位取样）进行设置。
{% endhint %}

<br>

![[Figure 1.3.7.2-21 从配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_21.png>)

<br>

{% hint style="info" %}
   [生产抑制时间]

   - 设置从设备的 IO 数据生成周期（毫秒）

   - 例如）10 毫秒：每 10 毫秒生成 IO 数据。  
   - 例如）0 毫秒：从设备尽可能快地产生 IO 数据。  

   - 周期越短，从设备的负载可能越大。（需要检查每个从设备的规格。） 
{% endhint %}

<br>

{% hint style="info" %}
   [预期数据包率]

   - 设置主设备和从设备之间 IO 数据更新的时间。  
{% endhint %}

<br>

![[Figure 1.3.7.2-22 从配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_22.png>)

<br>

**12. 配置主设备**

{% hint style="info" %}
   - 双击主设备。
{% endhint %}

![[Figure 1.3.7.2-23 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - 设置 DeviceNet 通信速度（与从设备通信速度相同）。
{% endhint %}

![[Figure 1.3.7.2-24 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - 检查地址表中每个从设备插槽的分配 IO 和起始地址。
{% endhint %}

![[Figure 1.3.7.2-25 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - 设置是否使用快速连接功能。
{% endhint %}

![[Figure 1.3.7.2-26 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 设置完成后，继续下载。
{% endhint %}

![[Figure 1.3.7.2-27 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_27.png>)

<br>

**13. 检查通信状态。**

{% hint style="info" %}
   - 在 Sycon.net 和 TP 中检查通信状态。

   - 有关在 TP 上检查工业通信状态的程序，请参阅 ("[1.4 CIFX PCI 通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

{% hint style="info" %}
   - 双击连接的主设备以检查通信状态。
{% endhint %}

![[Figure 1.3.7.2-28 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_28.png>)

![[Figure 1.3.7.2-29 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_29.png>)

{% hint style="info" %}
   - 使用 Sycon.net 的诊断功能，可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.7.2-30 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_30.png>)

<br>

**14. 在完成通信设置后分配 IO 块。**
{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块来使用输入/输出信号。请参考 ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
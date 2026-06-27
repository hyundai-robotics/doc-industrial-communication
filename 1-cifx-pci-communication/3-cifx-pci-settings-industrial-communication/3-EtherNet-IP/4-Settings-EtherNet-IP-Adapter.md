#### 1.3.3.4 EtherNet/IP 适配器设置

请遵循 "[1.3.1 CIFX PCI 插槽设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 程序，然后继续以下方法。

<br>

{% hint style="info" %}
   **[EtherNet/IP 适配器 EDS 文件下载]**

   - 请参考 "[6. 从设备描述文件](../../../6-slave-config-file.md)"。
{% endhint %}

<br>

**1. 使用 TP，在工业通信固件设置中选择 EtherNet/IP 从设备并重启机器人控制器。**

![[Figure 1.3.3.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查当前通信协议准备状态。**

![[Figure 1.3.3.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果使用 Sycon.net 设置的配置文件下载到相应的 PCI 插槽，TP 设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单以进入从设备设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI 从设备插槽设置 > EtherNet/IP 从设备]**

![[Figure 1.3.3.4-3 从设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.3.4-4 从设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

**4. 每个项目的描述**

{% hint style="info" %}
   [IP 设置]

   - 固定 IP: 用户设置 IP 地址、子网掩码和网关信息。

   - 动态分配 (DHCP): 从 DHCP 服务器分配一个 IP 地址。
{% endhint %}

{% hint style="info" %}
   [通信错误时输入 (总线错误下的操作)]

   - 清除: 当发生通信错误时，将所有输入初始化为 0。

   - 保持: 当发生通信错误时，保持最后有效的输入值。
{% endhint %}

{% hint style="info" %}
   [通信错误允许时间 (允许的错误时间)]

   - 如果通信错误持续超过指定的允许时间，将输出现场总线错误信号和警报。
{% endhint %}

{% hint style="info" %}
   [输入字节计数 (输入字节)]

   - 输入字节计数: 设置从主设备 -> 从设备的数据输入大小。

   - O -> T: 发起者(主设备) -> 目标 (从设备)
{% endhint %}

{% hint style="info" %}
   [输出字节计数 (输出字节)]

   - 输出字节计数: 设置从从设备 -> 主设备的数据输出大小。

   - T -> O: 目标 (从设备) -> 发起者 (主设备)
{% endhint %}

{% hint style="info" %}
   [运行 / 待机标头]

   - 应用于控制器的 CIFX-50 RE EtherNet/IP 适配器在与扫描仪交换 IO 时使用 32 位运行/待机标头 (默认)。

   - 请根据扫描仪规格适当设置是否使用输入和输出 32 位运行/待机标头。
{% endhint %}

<br>

{% hint style="info" %}
   [快速连接]

   - EtherNet/IP 支持快速连接功能。

   - 如果需要快速连接功能，请使用 Sycon.net 设置 EtherNet/IP 适配器。

      (1) 需要支持主设备和从设备的快速连接功能的产品  
      (2) 使用自动协商时无法使用快速连接  
      (3) 使用自动 MDI-X 时无法使用快速连接  
      (4) 需要 100 Mbit/s，双工  
{% endhint %}

<br>

**5. 完成设置后，请按照以下程序检查通信状态。**

有关在 TP 上检查工业通信状态的程序，请参考 ("[1.4 CIFX PCI 通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。

![[Figure 1.3.3.4-5 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_5.png>)

<br>

**6. 在完成通信设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[5. 工业通信 IO 读取和写入](../../../5-io-block-allocation.md)")。**
{% endhint %}
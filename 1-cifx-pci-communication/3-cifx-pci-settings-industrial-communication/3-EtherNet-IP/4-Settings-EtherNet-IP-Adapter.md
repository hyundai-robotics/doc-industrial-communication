#### 1.3.3.4 EtherNet/IP适配器设置

请遵循“[1.3.1 CIFX PCI插槽设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”程序，然后继续下面的方法。

<br>

{% hint style="info" %}
   **[EtherNet/IP适配器EDS文件下载]**

   - 请参考“[6. 从设备描述文件](../../../6-slave-config-file.md)”。
{% endhint %}

<br>

**1. 使用TP，在工业通信固件设置中选择EtherNet/IP从设备并重启机器人控制器。**

![[Figure 1.3.3.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查当前通信协议准备状态。**

![[Figure 1.3.3.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果使用Sycon.net下载的配置文件设置到相应的PCI插槽，TP设置将被忽略。
{% endhint %}

<br>

**3. 点击菜单以进入从设备设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从设备插槽设置 > EtherNet/IP从设备]**

![[Figure 1.3.3.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.3.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

**4. 各项说明**

{% hint style="info" %}
   [IP设置]

   - 固定IP：用户设置IP地址、子网掩码和网关信息。

   - 动态分配（DHCP）：从DHCP服务器分配IP地址。
{% endhint %}

{% hint style="info" %}
   [通信错误时输入（总线错误中的操作）]

   - 清除：当发生通信错误时，将所有输入初始化为0。

   - 保持：当发生通信错误时，保持最后有效的输入值。
{% endhint %}

{% hint style="info" %}
   [通信错误允许时间（错误允许时间）]

   - 如果通信错误持续超过指定的允许时间，将输出现场总线错误信号和报警。
{% endhint %}

{% hint style="info" %}
   [输入字节计数（输入字节）]

   - 输入字节计数：设置来自主设备->从设备的数据大小。

   - O -> T：起始设备（主设备）-> 目标设备（从设备）
{% endhint %}

{% hint style="info" %}
   [输出字节计数（输出字节）]

   - 输出字节计数：设置从设备->主设备的数据大小。

   - T -> O：目标设备（从设备）-> 起始设备（主设备）
{% endhint %}

{% hint style="info" %}
   [运行/闲置头]

   - 应用于控制器的CIFX-50 RE EtherNet/IP适配器在与扫描器交换IO时使用32位运行/闲置头（默认）。

   - 请根据扫描器规格适当设置是否使用输入和输出32位运行/闲置头。
{% endhint %}

<br>

{% hint style="info" %}
   [快速连接]

   - EtherNet/IP支持快速连接功能。

   - 如果需要快速连接功能，请使用Sycon.net设置EtherNet/IP适配器。

      (1) 需要支持快速连接功能的主设备和从设备  
      (2) 使用自动协商时无法使用快速连接  
      (3) 使用自动MDI-X时无法使用快速连接  
      (4) 需要100 Mbit/s，全双工  
{% endhint %}

<br>

**5. 完成设置后，请按照下面的程序检查通信状态。**

有关在TP上检查工业通信状态的程序，请参考（"[1.4 CIFX PCI通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)"）。

![[Figure 1.3.3.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_5.png>)

<br>

**6. 完成通信设置后，分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块使用输入/输出信号。请参考（"[5. 工业通信IO读写](../../../5-io-block-allocation.md)"）。**
{% endhint %}
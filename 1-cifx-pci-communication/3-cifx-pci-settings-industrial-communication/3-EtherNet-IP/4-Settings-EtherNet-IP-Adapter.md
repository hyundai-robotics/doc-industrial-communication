#### 1.3.3.4 EtherNet/IP适配器设置

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   **[EtherNet/IP适配器EDS文件下载]**

   - Please refer to "[**5. 从设备描述文件**](../../../5-slave-config-file.md)".
{% endhint %}

<br>

**1. 使用TP，选择工业通信固件设置中的EtherNet/IP从设备，并重新启动机器人控制器。**

![[Figure 1.3.3.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

**2. 检查工业通信监控菜单中的当前通信协议就绪状态。**

![[Figure 1.3.3.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**: 如果使用Sycon.net下载配置文件到相应的PCI插槽，TP设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单以进入从设备设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从设备插槽设置 > EtherNet/IP从设备]**

![[Figure 1.3.3.4-3 从设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.3.4-4 从设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

**4. 各项描述**

{% hint style="info" %}
   [IP设置]

   - 固定IP：用户设置IP地址、子网掩码和网关信息。

   - 动态分配（DHCP）：从DHCP服务器分配IP地址。
{% endhint %}

{% hint style="info" %}
   [通信错误时的输入（总线错误时的操作）]

   - 清除：当发生通信错误时将所有输入初始化为0。

   - 保持：当发生通信错误时保持最后有效的输入值。
{% endhint %}

{% hint style="info" %}
   [通信错误允许时间（允许的错误时间）]

   - 如果通信错误持续超过指定的允许时间，将输出现场总线错误信号和报警。
{% endhint %}

{% hint style="info" %}
   [输入字节计数（输入字节）]

   - 输入字节计数：设置从主设备到从设备的数据输入大小。

   - O -> T：发起者（主设备）-> 目标（从设备）
{% endhint %}

{% hint style="info" %}
   [输出字节计数（输出字节）]

   - 输出字节计数：设置从从设备到主设备的数据输出大小。

   - T -> O：目标（从设备）-> 发起者（主设备）
{% endhint %}

{% hint style="info" %}
   [运行/空闲头]

   - 应用于控制器的CIFX-50 RE EtherNet/IP适配器在与扫描仪交换IO时使用32位运行/空闲头（默认）。

   - 请根据扫描仪规格适当设置是否使用输入和输出32位运行/空闲头。
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

**5. 完成设置后，请按照以下程序检查通信状态。**

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.3.4-5 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_5.png>)

<br>

**6. 完成通信设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块使用输入/输出信号。请参考 ("[**4. 工业通信IO块分配**](../../../4-io-block-allocation.md)").**
{% endhint %}
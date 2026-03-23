#### 1.3.10.1 EtherNet/IP - 标准远程IO连接设置

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

**1. 在工业通信固件设置中选择EtherNet/IP主站，并重启机器人控制器。**

![[Figure 1.3.10.1-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查所选协议的就绪状态。**

![[Figure 1.3.10.1-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

**3. 连接PCI和远程IO电缆等进行通信，并检查状态。**

![[Figure 1.3.10.1-3 硬件连接]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[Figure 1.3.10.1-4 硬件连接]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

<br>

{% hint style="info" %}
   - 请使用LAN电缆连接PCI和远程IO。

   - 将远程IO的所有DIP开关设置为OFF。

   - 同时连接远程IO电源和现场电源（24 V DC）。
{% endhint %}

<br>

{% hint style="info" %}
   - Crevis M9289远程IO的出厂默认IP为192.168.100.99。

   - 为了启用通信连接，远程IO IP应设置为192.168.100.99。

   - "[**1.3.10.2 远程IO IP设置**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

**4. 触摸菜单以进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从站插槽设置 > EtherNet/IP远程IO设置]**

![[Figure 1.3.10.1-5 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>)

![[Figure 1.3.10.1-6 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>)

<br>

{% hint style="info" %}
   - IP设置为固定值。

   - 检查输入和输出字节计数。

   - 选择的输入和输出字节计数应小于或等于安装在远程IO槽中的卡的IO字节计数。
{% endhint %}

<br>

{% hint style="info" %}
   - 输入模块  
   - M12DF: 数字16点  
   - M3534: 模拟4点  
{% endhint %}

{% hint style="info" %}
   - 输出模块  
   - M225F: 数字16点  
   - M226F: 数字16点  
   - M2768: 数字8点   
   - M4534: 模拟4点  
{% endhint %}

{% hint style="info" %}
   - 特殊模块  
   - M5112 : 输送机I/F
{% endhint %}

<br>

**5. 完成设置后重启控制器。**

![[Figure 1.3.10.1-7 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>)

![[Figure 1.3.10.1-8 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
   - 请在完成设置后重启控制器。
{% endhint %}

<br>

**6. 确认设置值反映后，检查通信状态。**

![[Figure 1.3.10.1-9 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>)

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.10.1-10 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>)

{% hint style="info" %}
   - 如果通信未连接，您应检查远程IO IP。

   - 请遵循以下步骤。（如果不是192.168.100.99）

   - "[**1.3.10.2 远程IO IP设置**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

![[Figure 1.3.10.1-11 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>) 

![[Figure 1.3.10.1-12 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>)

<br>

**7. 完成通信设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块来使用输入/输出信号。请参考 ("[**4. 工业通信IO块分配**](../../../4-io-block-allocation.md)")。**
{% endhint %}
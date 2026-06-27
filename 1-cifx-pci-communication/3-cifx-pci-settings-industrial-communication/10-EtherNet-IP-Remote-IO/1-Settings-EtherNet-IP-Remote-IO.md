#### 1.3.10.1 EtherNet/IP - 标准远程 IO 连接设置

请遵循 "[1.3.1 CIFX PCI 插槽设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 程序，然后继续以下方法。

<br>

**1. 在工业通信固件设置中选择 EtherNet/IP 主站并重启机器人控制器。**

![[Figure 1.3.10.1-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查所选协议的就绪状态。**

![[Figure 1.3.10.1-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

**3. 连接 PCI 和远程 IO 电缆等以进行通信并检查状态。**

![[Figure 1.3.10.1-3 Hardware Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[Figure 1.3.10.1-4 Hardware Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

<br>

{% hint style="info" %}
   - 请使用 LAN 电缆连接 PCI 和远程 IO。

   - 将远程 IO 的所有 DIP 开关设置为 OFF。

   - 同时连接远程 IO 电源和现场电源 (24 V DC)。
{% endhint %}

<br>

{% hint style="info" %}
   - Crevis M9289 远程 IO 的工厂默认 IP 为 192.168.100.99。

   - 远程 IO IP 应设置为 192.168.100.99 以启用通信连接。

   - "[1.3.10.2 远程 IO IP 设置](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

**4. 触摸菜单以进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI 从站插槽设置 > EtherNet/IP 远程 IO 设置]**

![[Figure 1.3.10.1-5 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>)

![[Figure 1.3.10.1-6 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>)

<br>

{% hint style="info" %}
   - IP 被设置为固定值。

   - 检查输入和输出字节计数。

   - 所选的输入和输出字节计数应小于或等于安装在远程 IO 插槽中的卡的 IO 字节计数。
{% endhint %}

<br>

{% hint style="info" %}
   - 输入模块  
   - M12DF: 数字 16 点  
   - M3534: 模拟 4 点  
{% endhint %}

{% hint style="info" %}
   - 输出模块  
   - M225F: 数字 16 点  
   - M226F: 数字 16 点  
   - M2768: 数字 8 点   
   - M4534: 模拟 4 点  
{% endhint %}

{% hint style="info" %}
   - 特殊模块  
   - M5112 : 输送机 I/F
{% endhint %}

<br>

**5. 完成设置后重启控制器。**

![[Figure 1.3.10.1-7 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>)

![[Figure 1.3.10.1-8 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
   - 请在完成设置后重启控制器。
{% endhint %}

<br>

**6. 在确认设置值已反映后，检查通信状态。**

![[Figure 1.3.10.1-9 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>)

要查看 TP 上工业通信状态的程序，请参考 ("[1.4 CIFX PCI 通信监控](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。

![[Figure 1.3.10.1-10 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>)

{% hint style="info" %}
   - 如果通信未连接，您应检查远程 IO IP。

   - 请遵循以下步骤。 (如果不是 192.168.100.99)

   - "[1.3.10.2 远程 IO IP 设置](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

![[Figure 1.3.10.1-11 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>) 

![[Figure 1.3.10.1-12 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>)

<br>

**7. 在完成通信设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[5. 工业通信 IO 读取和写入](../../../5-io-block-allocation.md)")。**
{% endhint %}
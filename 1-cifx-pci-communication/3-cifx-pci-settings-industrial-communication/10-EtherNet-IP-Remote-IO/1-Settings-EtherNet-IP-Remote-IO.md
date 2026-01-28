#### 1.3.10.1 EtherNet/IP - 标准Remote IO连接设置

请按照“[**1.3.1 CIFX PCI槽位设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”流程设置后，再按以下方法进行操作。

<br>

**1. 在工业通信固件设置中，选择EtherNet/IP Master并重启机器人控制器。**

![[图1.3.10.1-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>)

<br>

**2. 在工业通信监控中，确认所选协议的准备状态。**

![[图 1.3.10.1-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

**3. 为了实现通信，连接PCI与Remote IO的电缆等并确认状态。**

![[图 1.3.10.1-3 硬件连接]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[图 1.3.10.1-4 硬件连接]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

<br>

{% hint style="info" %}
   - 请用LAN电缆连接PCI和Remote IO。

   - 请将Remote IO的DIP Switch全部设置为OFF。

   - 请全部连接Remote IO电源和Field Power。（24V DC）
{% endhint %}

<br>

{% hint style="info" %}
   - Remote IO Crevis M9289的出厂设置IP（默认值）为192.168.100.99。

   - Remote IO的IP必须设置为192.168.100.99才能正常连接通信。

   - “[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)”
{% endhint %}

<br>

**4. 触摸菜单来进入从站设置界面。**

**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从站插槽设置 > EtherNet/IP Remote IO Setting]**

![[图 1.3.10.1-5 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>) 

![[图 1.3.10.1-6 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>) 

<br>

{% hint style="info" %}
   - IP 已被设置为固定值。

   - 确认 Input、Output 字节数。

   - 所选的 Input、Output 字节数必须小于或等于安装在 Remote IO Slot 中的卡件 IO 数量。
{% endhint %}

<br>

{% hint style="info" %}
   - Input Module  
   - M12DF：Digital 16点  
   - M3534：Analog 4点  
{% endhint %}

{% hint style="info" %}
   - Output Module  
   - M225F：Digital 16点  
   - M226F：Digital 16点  
   - M2768：Digital 8点   
   - M4534：Analog 4点  
{% endhint %}

{% hint style="info" %}
   - Special Module  
   - M5112 : Conveyer I/F 
{% endhint %}

<br>

**5. 设置完成后重启控制器。**

![[图 1.3.10.1-7 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>) 

![[图 1.3.10.1-8 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
   - 设置完成后，请重启控制器。
{% endhint %}

<br>

**6. 确认设定值是否已反映，并确认通信状态。**

![[图 1.3.10.1-9 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>) 

在TP上确认工业通信状态的程序，请参考（“[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”）。

![[图1.3.10.1-10 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>) 

{% hint style="info" %}
   - 如果通信无法连接，需要确认Remote IO的IP。

   - 请按照以下步骤进行确认。（若不是192.168.100.99）

   - “[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)”
{% endhint %}

![[图 1.3.10.1-11 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>)

![[图 1.3.10.1-12 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>)

<br>

**7. 通信设置完成后分配IO Block。**

{% hint style="info" %}
   **通信设置完成后，可以通过分配 IO Block 来使用输入输出信号。请确认（“[**4. 工业通信 IO Block 分配**](../../../4-io-block-allocation.md)”）。**
{% endhint %}
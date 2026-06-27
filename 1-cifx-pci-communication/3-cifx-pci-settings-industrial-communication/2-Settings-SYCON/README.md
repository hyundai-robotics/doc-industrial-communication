### 1.3.2 SYCON.NET 设置

对于 PCI 通信卡，使用 "**Sycon.net**" 程序进行工业通信设置。设置方法如下。 (请参考 "[1.1 Sycon.net 安装](../../1-cifx-pci-install-program/1-sycon-net.md)" 进行安装。)

<br>

**1. 将安装了 Sycon.net 的 PC 连接到机器人控制器的一般 LAN 端口（不是 PCI LAN 端口）。**
触摸 **\[System > 2: 控制参数 > 9: 网络]** 菜单以检查一般 LAN 端口的 IP。请通过 ping 测试等检查连接状态。

<br>

![[Figure 1.3.2-1 网络 IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_1.png>)

<br>

{% hint style="info" %}
   - IP 地址可以根据用户设置进行更改。
{% endhint %}

<br>

**2. 执行 Sycon.net。**

![[Figure 1.3.2-2 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_2.png>)

<br>

**3. 在屏幕右侧的设备目录菜单中，单击与设置的通信协议匹配的项目，然后将其拖放到中间的总线线路上。**

![[Figure 1.3.2-3 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_3.png>)
![[Figure 1.3.2-4 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_4.png>)

<br>

**4. 双击导入的项目进行设置。**

{% hint style="info" %}
   - “双击”导入的 CIFX PCI（图）。

   - 设置 -> 驱动程序

   - 选择 netX 驱动程序。
{% endhint %}

![[Figure 1.3.2-5 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_5.png>)

{% hint style="info" %}
   - 设置 -> 驱动程序 -> netX 驱动程序 -> TCP 连接

   - IP 地址：请输入连接控制器的一般 LAN 端口 IP 地址。
{% endhint %}

![[Figure 1.3.2-6 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_6.png>)

{% hint style="info" %}
   - 设备分配 -> 点击扫描

   - 选择通信（检查通道协议），然后“应用”和“确定”。
{% endhint %}

{% hint style="warning" %}
**\[注意]**：请务必检查通道协议和插槽编号。
{% endhint %}

{% hint style="warning" %}
**\[注意]**：如果扫描不起作用，请检查与控制器的电缆连接状态以及固件设置。
{% endhint %}

![[Figure 1.3.2-7 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_7.png>)


{% hint style="info" %}
   - 右键单击 CIFX PCI 图形 -> 下载
{% endhint %}

![[Figure 1.3.2-8 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_8.png>)
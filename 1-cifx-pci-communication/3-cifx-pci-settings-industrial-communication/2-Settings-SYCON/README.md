## 1.3.2 SYCON.NET设置

Hi6控制器使用“**Sycon.net**”程序进行工业通信设置。具体的设置方法如下。（请参考“[**1.1 Sycon.net安装**](../../1-cifx-pci-install-program/1-sycon-net.md)”进行安装。）

<br>

**1. 连接已安装Sycon.net的PC与机器人控制器的通用LAN端口。（PCI LAN Port X）**
触摸 **\[系统 > 2: 控制参数 > 9: 网络]** 菜单，确认通用LAN端口的IP。请通过Ping Test等确认是否连接。

![[图1.3.2-1 网络 IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_1.png>)
![[图 1.3.2-2 网络 IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_2.png>) 

{% hint style="info" %}
\.      IP Address 可根据用户设置进行更改。
{% endhint %}

<br>

**2. 执行 Sycon.net。**

![[图 1.3.2-3 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_3.png>)

<br>

**3. 在屏幕右侧 Device Catalog 中点击与已设置的通信协议对应的项目，通过拖放（Drag & Drop）放置到中央的总线线上。**

![[图 1.3.2-4 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_4.png>)
![[图 1.3.2-5 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_5.png>)

<br>

**4. 双击导入的项目进行设置。**

{% hint style="info" %}
\.      导入的CIFX PCI（图）“Double Click”

\.      Settings -> Driver

\.      选择netX Driver。
{% endhint %}

![[图 1.3.2-6 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_6.png>)

{% hint style="info" %}
\.     Setting -> Driver -> netX Driver -> TCP Connection 

\.     IP Address：请输入已连接控制器的通用LAN Port IP地址。
{% endhint %}

![[图 1.3.2-7 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_7.png>)

{% hint style="info" %}
\.      Device Assignment -> 点击Scan

\.      选择通信（确认Channel Protocol）后，先点“Apply”，再点“OK”。
{% endhint %}

{% hint style="warning" %}
**\[注意]**：请务必确认Channel Protocol和Slot编号。
{% endhint %}

{% hint style="warning" %}
**\[注意]**: Scan 无法进行时，请检查与控制器的电缆连接状态、固件设置。
{% endhint %}

![[图 1.3.2-8 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_8.png>)


{% hint style="info" %}
\.      右击 CIFX PCI 图 -> DOWNLOAD
{% endhint %}

![[图 1.3.2-9 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_9.png>)
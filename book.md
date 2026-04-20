
[__SOURCE](README.md)
# Hi7 控制器功能手册 - 工业通信
[__SOURCE](0-about-this-manual/precautions.md)
# 注意事项

{% include file="zh/precautions.md" %}
[__SOURCE](1-cifx-pci-communication/README.md)
# 1. CIFX PCI 通信

这是一个关于使用 CIFX PCI 的工业通信手册。
[__SOURCE](1-cifx-pci-communication/1-cifx-pci-install-program/README.md)
## 1.1 CIFX PCI 程序安装

这是安装与工业通信相关程序的方法。
[__SOURCE](1-cifx-pci-communication/1-cifx-pci-install-program/1-sycon-net.md)
### 1.1.1 SYCON.net 安装

"Sycon.net" 是 Hilscher 提供的用于配置 PCI 通信卡的程序。

<br>

**1. SYCON.net 最新版本下载路径**

{% hint style="info" %}
   - 点击 **[https://hilscher.atlassian.net/](https://hilscher.atlassian.net/wiki/spaces/HILKB/overview?mode=global) -> Software -> SYCON.net**。
{% endhint %}

<br>

![[Figure 1.1.1-1 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_1.png>)

<br>

![[Figure 1.1.1-2 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_2.png>)

<br>

{% hint style="info" %}
   - 选择最新版本（当前发布）并下载。
{% endhint %}

<br>

![[Figure 1.1.1-3 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_3.png>)

<br>

![[Figure 1.1.1-4 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_4.png>)

<br>

{% hint style="info" %}
   - 执行下载的 SYCON.NET Setup.exe 文件以安装程序。
{% endhint %}

<br>

![[Figure 1.1.1-5 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_5.png>)

<br>

![[Figure 1.1.1-6 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_6.png>)

<br>

{% hint style="info" %}
   - 执行已安装的 SYCON.NET 程序以检查安装是否成功完成。
{% endhint %}

<br>

![[Figure 1.1.1-7 Sycon.net Installation Screen]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_7.png>)

<br>


**2. 从现代机器人官网下载程序。**

{% hint style="info" %}
   - 从 [www.hd-hyundairobotics.com](https://hd-hyundairobotics.com/) -> 工业机器人网站 -> 客户支持 -> 应用软件下载 "**Sycon.net**"。
{% endhint %}

<br>

{% hint style="info" %}
   - 解压 -> 执行 SYCON.NET Setup.exe 文件以安装程序。
{% endhint %}

<br>

{% hint style="info" %}
   - 我们网站提供的 SYCON.net 程序可能与最新版本不同。
{% endhint %}

<br>
[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/README.md)
## 1.2 CIFX PCI 通信卡安装和设置

要使用工业通信，需要一个 PCI 通信卡（来自 Hilscher）。根据所需通信设置通信卡并连接连接器。
[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)
### 1.2.1 PCI 工业通信卡


<br>

**1. 将购买的 PCI 通信卡安装在控制器的主模块内。**

<br>

**2. 旋转 PCI 通信卡的旋转开关以设置插槽编号。**

{% hint style="warning" %}
**\[注意]**: PCI 插槽的物理位置与通信卡上的旋转开关设置无关。
{% endhint %}

<br>

**3. 为每个 PCI 通信卡单独设置插槽编号，编号范围为 1 \~ 3。**
  (当使用多个 PCI 通信卡时，必须为每张卡设置不同的编号。)

![[Figure 1.2.1-1 PCI Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_2.png>)

<br>

![[Figure 1.2.1-2 PCI Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_3.png>)

{% hint style="warning" %}
**\[注意]**: 请为每张 PCI 卡设置不同的旋转开关编号。
{% endhint %}
[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)
### 1.2.2 连接器

<br>

**使用适合工业通信方式的连接器和电缆。**

![[Figure 1.2.2-1 Industrial Communication Connector]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector/image_2.png>)

{% hint style="info" %}
   - DeviceNet 终端电阻：120 欧姆

   - CC-Link 终端电阻：110 欧姆
{% endhint %}

<br>

{% hint style="warning" %}
**\[注意]**：请为通信电缆和IO使用独立的电源。
{% endhint %}

<br>
[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led.md)
### 1.2.3 LED 描述

<br>

**PCI LED 描述**

<br>

![[Figure 1.2.3-1 PCI Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_2.png>)

<br>

![[Figure 1.2.3-3 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_3.png>)

<br>

![[Figure 1.2.3-4 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_4.png>)

<br>

![[Figure 1.2.3-5 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_5.png>)

<br>

![[Figure 1.2.3-6 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_6.png>)

<br>

![[Figure 1.2.3-7 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_7.png>)

<br>

![[Figure 1.2.3-8 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_8.png>)

<br>

![[Figure 1.2.3-9 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_9.png>)

<br>

![[Figure 1.2.3-10 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_10.png>)

<br>

![[Figure 1.2.3-11 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_11.png>)

<br>

![[Figure 1.2.3-12 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_12.png>)

<br>

![[Figure 1.2.3-13 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_13.png>)

<br>

![[Figure 1.2.3-14 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_14.png>)

<br>

![[Figure 1.2.3-15 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_15.png>)

<br>

![[Figure 1.2.3-16 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_16.png>)

<br>

![[Figure 1.2.3-17 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_17.png>)

<br>

![[Figure 1.2.3-18 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_18.png>)

<br>

![[Figure 1.2.3-19 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_19.png>)

<br>

![[Figure 1.2.3-20 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_20.png>)

<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/README.md)
## 1.3 CIFX PCI 通信设置

要使用工业通信，请安装 PCI 通信卡，并使用教学挂件和 Sycon.net 程序进行设置。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)
### 1.3.1 CIFX PCI插槽设置

配置CIFX PCI插槽的通信方法。要应用设置，请断开控制器电源，然后重新供电。

<br>

请参考"[**1.2.1 PCI工业通信卡**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)"并按照以下方法进行操作。

<br>

**1. 点击菜单进入插槽设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 1: PCI插槽设置 > 通道1]** 

<br>

**2. 请参考下面的屏幕选择插槽、通信方法（主/从）和协议。**
   * 插槽号是PCI通信卡的旋转开关编号。
   * 如果您不想更改通信设置，请点击**\[确定]**按钮退出。

{% hint style="warning" %}
**\[注意]**: 点击**\[初始化]**或**\[应用]**按钮将初始化当前选项卡上的插槽信息。配置文件也将被初始化，请注意。
{% endhint %}

![[图 1.3.1-1 PCI插槽设置]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[图 1.3.1-2 PCI插槽设置（主）]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[图 1.3.1-3 PCI插槽设置（从）]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

**3. 完成插槽设置。**
点击**\[应用]**菜单。

![[图 1.3.1-4 PCI插槽设置]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[注意]**

<1>. 当通过点击**\[应用]**按钮来应用设置时，所有应用于相应插槽的CONFIG文件将被删除并更改。建议在更改通信时保留现有设置的单独备份。

<2>. 如果您在未点击**\[应用]**按钮的情况下点击**\[确定]**按钮，所选的通信将不会被应用。
{% endhint %}

<br>

**4. 对每个插槽重复步骤2. ~ 3.**

<br>

**5. 重新启动控制器以应用所设置的通信。**
点击**\[服务 > 19: 工业通信监控]**菜单以检查所设置的通信是否已被应用。

![[图 1.3.1-5 工业通信设置屏幕]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)

{% hint style="warning" %}
**\[注意]**: 在插槽设置后，重新启动控制器时会应用设置。
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)
### 1.3.2 SYCON.NET 设置

对于 PCI 通信卡，请使用 "**Sycon.net**" 程序进行工业通信设置。设置方法如下。 (请参考 "[**1.1 Sycon.net 安装**](../../1-cifx-pci-install-program/1-sycon-net.md)" 进行安装。)

<br>

**1. 将安装了 Sycon.net 的 PC 连接到机器人控制器的一般 LAN 端口 (而不是 PCI LAN 端口)。**
触摸 **\[System > 2: Control Parameters > 9: Network]** 菜单以检查一般 LAN 端口的 IP。请通过 ping 测试等检查连接状态。

![[Figure 1.3.2-1 Network IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_1.png>)
![[Figure 1.3.2-2 Network IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_2.png>) 

{% hint style="info" %}
   - IP 地址可以根据用户设置进行更改。
{% endhint %}

<br>

**2. 执行 Sycon.net。**

![[Figure 1.3.2-3 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_3.png>)

<br>

**3. 在屏幕右侧的设备目录菜单中，单击与设置的通信协议匹配的项目，并将其通过拖放放置在中间的总线行上。**

![[Figure 1.3.2-4 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_4.png>)
![[Figure 1.3.2-5 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_5.png>)

<br>

**4. 双击导入的项目以进行设置。**

{% hint style="info" %}
   - "双击" 导入的 CIFX PCI (图)。

   - 设置 -> 驱动程序

   - 选择 netX 驱动程序。
{% endhint %}

![[Figure 1.3.2-6 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_6.png>)

{% hint style="info" %}
   - 设置 -> 驱动程序 -> netX 驱动程序 -> TCP 连接

   - IP 地址：请输入连接控制器的一般 LAN 端口 IP 地址。
{% endhint %}

![[Figure 1.3.2-7 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_7.png>)

{% hint style="info" %}
   - 设备分配 -> 点击扫描

   - 选择通信 (检查通道协议) 然后 "应用" 和 "确定。"
{% endhint %}

{% hint style="warning" %}
**\[注意]**：请务必检查通道协议和插槽编号。
{% endhint %}

{% hint style="warning" %}
**\[注意]**：如果扫描不起作用，请检查与控制器之间的电缆连接状态以及固件设置。
{% endhint %}

![[Figure 1.3.2-8 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_8.png>)


{% hint style="info" %}
   - 右键单击 CIFX PCI 图形 -> 下载
{% endhint %}

![[Figure 1.3.2-9 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_9.png>)
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)
#### 1.3.2.1 SYCON.NET 帮助



<br>

**使用 SYCON.net 时，如果手册中解释不够，请参考下面的 "帮助" 功能。**

<br>

![[Figure 1.3.2.1-1 SYCON.net help]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/1-Help-SYCON/image_1.png>) 

<br>

![[Figure 1.3.2.1-2 SYCON.net help]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/1-Help-SYCON/image_2.png>) 

<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/README.md)
### 1.3.3 EtherNet/IP

本章描述了EtherNet/IP主设备（扫描器）和从设备（适配器）的特性及其设置方法。

<br>

**EtherNet/IP 概述**

EtherNet/IP是由CI（ControlNet International）和ODVA（Open DeviceNet Vendors Association）开发的基于以太网的开放工业通信协议。

在工厂中，各种设备如传感器、远程IO、驱动器、HMI、PLC和机器人控制器可以无论制造商如何连接到一个EtherNet/IP网络。

![[Figure 1.3.3-1 EtherNet/IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/image_1.png>)


<br>

EtherNet/IP根据通信功能分类如下。

**扫描器类**
   * 对应现有现场总线主设备的产品，可以请求EtherNet/IP适配器或扫描器执行I/O数据连接。

<br>

**适配器类**
  * 对应现有现场总线从设备的产品，是EtherNet/IP扫描器请求的实时I/O数据连接的目标。

  * 适配器不能在没有扫描器的情况下自行发送和接收实时I/O数据。

<br>

**消息类**
   * 可以发送和接收所有类别产品的明确消息的产品，但不支持实时I/O数据的传输和接收。

   * 例如，这些产品可以是用于程序上传/下载和网络设置工具的计算机接口卡等。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/1-Specification-EtherNet-IP-Scanner.md)
#### 1.3.3.1 EtherNet/IP 扫描仪规格

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>最大可连接从设备数量</td>
		<td>64</td>
	</tr>
    <tr>
		<td>最大输入大小</td>
		<td>1200 字节</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>1200 字节</td>
	</tr>
    <tr>
		<td>最大输入大小（1 个从设备）</td>
		<td>504 字节</td>
	</tr>
    <tr>
		<td>最大输出大小（1 个从设备）</td>
		<td>504 字节</td>
	</tr>
    <tr>
		<td>IO 连接</td>
		<td>周期性</td>
	</tr>
    <tr>
		<td>IO 更新周期</td>
		<td>最小 1 毫秒</td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>10 或 100 Mbit/s</td>
	</tr>
    <tr>
		<td>拓扑</td>
		<td>树形、线性、环形</td>
	</tr>
    <tr>
		<td>网络从设备扫描</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>DLR（设备级环）</td>
		<td>基于信标的 '环节点'</td>
	</tr>
    <tr>
		<td>附加特性</td>
		<td>支持 DHCP、BOOTP、ACD</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>以太网 II，IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>10 或 100 BASE-T 以太网</td>
	</tr>
    <tr>
		<td>自动协商</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>集线器</td>
		<td>允许</td>
	</tr>
    <tr>
		<td>交换机</td>
		<td>允许</td>
	</tr>
</tbody>
</table>
<br>

**连接**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>电缆</td>
		<td>最低 Cat5，STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最大 100m</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Settings-EtherNet-IP-Scanner.md)
#### 1.3.3.2 EtherNet/IP 扫描器设置

请遵循 "[**1.3.1 CIFX PCI 插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 和 "[**1.3.2 SYCON.NET 设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 的程序，然后继续下面的方法。

<br>

{% hint style="info" %}
   - 使用 SYCON.net 时，如果手册中的说明不足，请参考 "[**1.3.2 SYCON.NET 帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" 功能。
{% endhint %}

<br>

**1. 在 PCI 插槽设置中选择 EtherNet/IP 主设备并重新启动机器人控制器。**

![[Figure 1.3.3.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_1.png>)

<br>

**2. 在工业通信监控菜单中检查所选协议的就绪状态。**

<br>

{% hint style="info" %}
   - 有关如何在 TP 上检查工业通信状态的程序，请参见 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

<br>

![[Figure 1.3.3.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

**3. 使用 Sycon.net 选择 EtherNet/IP 扫描器 PCI 设备。**

![[Figure 1.3.3.2-3 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_3.png>)
![[Figure 1.3.3.2-4 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

**4. 扫描 PCI 设备并应用 EtherNet/IP 扫描器。**

![[Figure 1.3.3.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

**5. 下载设置。**

![[Figure 1.3.3.2-6 EtherNet/IP Scanner Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

**6. 准备要连接到 EtherNet/IP 扫描器的适配器（从属）模块。**
   * 在本例中，我们使用 Crevis 的 M9289 EtherNet/IP 适配器。
   * 请提供系统电源和现场电源以激活模块。

![[Figure 1.3.3.2-7 Crevis M9289]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

**7. 为 EtherNet/IP 通信连接设置适配器（从属）的 IP 地址。**

{% hint style="info" %}
   - 使用拨码开关设置 IP 地址。
{% endhint %}

![[Figure 1.3.3.2-8 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
   - 使用 BootpSvr.exe 设置 IP 地址的方法
{% endhint %}

<br>

**8. （Bootp 示例）使用 Bootp 设置从属设备的 IP 地址。**
   * 仅将 DIP 开关 9 改为 ON。

![[Figure 1.3.3.2-9 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_9.png>)

   * 将 PC 连接到 M9289 适配器 LAN 端口。

![[Figure 1.3.3.2-10 Crevis M9289 LAN Port]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

**9. 在 PC 上执行 BootpSvr.exe。**
   * 该程序由 Crevis 提供。（从网站下载并安装 IO Guide Pro。）

![[Figure 1.3.3.2-11 Crevis IO Guide Pro]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_11.png>)

![[Figure 1.3.3.2-12 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
   - 按下开始 BootP 后，断开并重新供电给 M9289 模块以重新启动它。
{% endhint %}

![[Figure 1.3.3.2-13 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

**10. 当适配器设备重新启动时，设备信息将出现在 BootpSvr.exe 程序中。**

![[Figure 1.3.3.2-14 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

**11. 选择设备并设置 IP。**

![[Figure 1.3.3.2-15 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_15.png>)![[Figure 1.3.3.2-16 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

**12. 设置 IP 后，将适配器的所有 DIP 开关设置为 OFF 并重新启动设备。**

{% hint style="info" %}
   - 一定要检查 DIP 开关状态以及适配器是否已重新启动。
{% endhint %}

![[Figure 1.3.3.2-17 Crevis DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

**13. 注册从属设备 EDS 文件。**

{% hint style="info" %}
   - 使用未在 Sycon.net 中注册的设备需要 EDS 文件。

   - M9289 适配器的 EDS 文件可以从 Crevis 网站下载。
{% endhint %}

![[Figure 1.3.3.2-18 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
   - 在 Sycon.net 中注册下载的 EDS 文件。

   - 注册 EDS 文件时，请检查工业通信协议（EtherNet/IP）。
{% endhint %}

![[Figure 1.3.3.2-19 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_19.png>)![[Figure 1.3.3.2-20 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_20.png>)
![[Figure 1.3.3.2-21 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_21.png>)

![[Figure 1.3.3.2-22 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

**14. 网络扫描**

{% hint style="info" %}
   - EtherNet/IP 扫描器不支持网络扫描功能。
{% endhint %}

<br>

**15. 配置从属（适配器）设备**

{% hint style="info" %}
   - 将注册的设备拖放到 EtherNet/IP 主设备总线线路上。
{% endhint %}

![[Figure 1.3.3.2-23 Sycon.net Bus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - 双击设备（适配器）以继续设置。

   - 设置适合安装在该设备上的 IO 设备的输入/输出字节数。

   - 在本例中，设置如下。
{% endhint %}

<br>

![[Figure 1.3.3.2-24 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - O -> T : 发起者（主设备） -> 目标（从设备）

   - 输出 : EtherNet/IP 扫描器  -> M9289

   [输出模块]   
      (1) M225F (2Bytes)   
      **=> 2Bytes**   
{% endhint %}

<br>

![[Figure 1.3.3.2-25 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - T -> O : 目标（从设备） -> 发起者（主设备）

   - 输入 : M9289 -> EtherNet/IP 扫描器

   [输入模块]
      (1) M7001  (1Byte)
      (2) M12DF  (2Bytes)
      **=> 3Bytes**


      (1) M7002 (0Byte)
      (2) M12DF (2Bytes)
      **=> 2Bytes**  
{% endhint %}

<br>

**16. 配置主（扫描器）设备。**

{% hint style="info" %}
   - 右键单击主设备以断开连接。
{% endhint %}

![[Figure 1.3.3.2-26 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 双击主设备。

   - 设置主设备 IP 地址。 
{% endhint %}

![[Figure 1.3.3.2-27 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - 设置从设备 IP 地址。
{% endhint %}

![[Figure 1.3.3.2-28 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - 设置从设备扫描时间。 

   - 请调整相应的值以设置适当的通信速度。
{% endhint %}

![[Figure 1.3.3.2-29 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
   - 检查地址表中的从设备设置。

   - 检查输入/输出 IO 字节数和起始地址。
{% endhint %}

![[Figure 1.3.3.2-30 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
   [快速连接]

   - EtherNet/IP 支持快速连接功能。
{% endhint %}

{% hint style="info" %}
   - 使用快速连接功能需要满足以下条件。

      (1) 必须有支持快速连接功能的主设备和从设备  
      (2) 使用自动协商时无法使用快速连接  
      (3) 使用自动 MDI-X 时无法使用快速连接  
      (4) 需要 100 Mbit/s 全双工  
{% endhint %}

{% hint style="info" %}
   - 完成设置后，继续下载。
{% endhint %}

![[Figure 1.3.3.2-31 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

**17. 检查通信状态**

{% hint style="info" %}
   - 在 Sycon.net 和 TP 中检查通信状态。

   - 有关在 TP 上检查工业通信状态的程序，请参见 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

{% hint style="info" %}
   - 双击已连接的主设备以检查通信状态。
{% endhint %}

![[Figure 1.3.3.2-32 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_32.png>)

![[Figure 1.3.3.2-33 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_33.png>)

{% hint style="info" %}
   - 使用 Sycon.net 的诊断功能，您可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.3.2-34 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_34.png>)

<br>

**18. 在完成通信设置后分配 IO 块。**
**完成通信设置后，您可以通过分配 IO 块使用输入/输出信号。请参阅 ("[**4. 工业通信 IO 块分配**](../../../4-io-block-allocation.md)").**  
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/3-Specification-EtherNet-IP-Adapter.md)
#### 1.3.3.3 EtherNet/IP 适配器规格

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>最大输入大小</td>
		<td>240 字节 (TP) / 504 字节 (Sycon.net)</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>240 字节 (TP) / 504 字节 (Sycon.net)</td>
	</tr>
    <tr>
		<td>IO 连接</td>
		<td>1 个独占所有者 <br>1 个仅监听 <br>1 个仅输入</td>
	</tr>
    <tr>
		<td>IO 更新周期</td>
		<td>最小 1 毫秒</td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>10 或 100 Mbit/s</td>
	</tr>
    <tr>
		<td>拓扑</td>
		<td>树形, 线形, 环形</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>DLR V2 (设备级环)</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>附加功能</td>
		<td>支持 DHCP, BOOTP, ACD</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>10 或 100 BASE-T 以太网</td>
	</tr>
    <tr>
		<td>自动协商</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>集线器</td>
		<td>允许</td>
	</tr>
    <tr>
		<td>交换机</td>
		<td>允许</td>
	</tr>
</tbody>
</table>
<br>

**连接**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>电缆</td>
		<td>至少 Cat5, STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最大 100 米</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Settings-EtherNet-IP-Adapter.md)
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
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error-EtherNet-IP.md)
#### 1.3.3.5 EtherNet/IP 错误处理

这是解决在 EtherNet/IP 设置过程中可能发生的重大错误的方法。

可以使用 Sycon.Net 的诊断功能检查错误。

<br>

请参阅 "[**1.4.1 错误代码**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"。

<br>

**1. 通信电缆断开错误**

{% hint style="info" %}
   - 请检查 LAN 电缆的连接状态。

   - 检查适配器设备的电源是否开着。
{% endhint %}

![[Figure 1.3.3.5-1 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_1.png>) 


<br>

**2. IP 地址设置错误**

{% hint style="info" %}
   - 请检查主设备和从设备的 IP 地址。

   - 如果适配器设备的设置 IP 地址与在 Sycon.net 中输入的值不同，则会发生错误。

{% endhint %}

![[Figure 1.3.3.5-2 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_2.png>) 

![[Figure 1.3.3.5-3 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_3.png>) 
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/README.md)
### 1.3.4 PROFINET IO

本章描述了PROFINET IO主站（控制器）和从站（设备）的特性，以及如何设置它们。

<br>

**PROFINET IO 概述**

PROFINET IO是一种基于以太网的开放工业通信协议，逐步从PROFIBUS-DP和工业以太网演变而来。

![[Figure 1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>) 

<br>

它遵循提供者-消费者模型进行数据交换，可以分为以下三类产品。

**IO 控制器类**
   * 对应现有PROFIBUS-DP类别1主站的产品，是运行自动化程序（例如PLC）的产品类型。

   * IO控制器向设置的IO设备提供输出数据，并从它们处获取输入数据。

<br>

**IO 设备类**
  * 对应现有PROFIBUS-DP从站的产品，通过PROFINET IO与PLC等IO控制器连接。

  * IO设备向IO控制器提供输出数据，提供输入数据，并消耗输出数据。

<br>

**IO 监视器类**
   * 对应现有PROFIBUS-DP类别2主站的产品，包括用于网络配置和诊断的编程设备、PC、HMI等。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/1-Specification-PROFINET-IO-Controller.md)
#### 1.3.4.1 PROFINET IO 控制器规格

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>最大可连接从站数量</td>
		<td>128</td>
	</tr>
    <tr>
		<td>最大输入大小</td>
		<td>1200 字节</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>1200 字节</td>
	</tr>
    <tr>
		<td>最大输入大小 (1 个从站)</td>
		<td>1024 字节</td>
	</tr>
    <tr>
		<td>最大输出大小 (1 个从站)</td>
		<td>1024 字节</td>
	</tr>
    <tr>
		<td>IO 连接</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 更新周期</td>
		<td>最小 1ms</td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>100 Mbit/s (全双工)</td>
	</tr>
    <tr>
		<td>拓扑</td>
		<td>树形, 线形</td>
	</tr>
    <tr>
		<td>网络从站扫描</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>DCP</td>
		<td>支持</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>以太网 II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>100 BASE-T 以太网</td>
	</tr>
    <tr>
		<td>自动协商</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>集线器</td>
		<td>禁止</td>
	</tr>
    <tr>
		<td>交换机</td>
		<td>仅在交换机支持时允许，优先级标记和 LLDP</td>
	</tr>
</tbody>
</table>
<br>

**连接**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>电缆</td>
		<td>至少 Cat5, STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最长 100m</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Settings-PROFINET-IO-Controller.md)
#### 1.3.4.2 PROFINET IO 控制器设置

请遵循 "[**1.3.1 CIFX PCI 插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 和 "[**1.3.2 SYCON.NET 设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 程序，然后继续以下方法。

<br>

{% hint style="info" %}
   - 使用 SYCON.net 时，如果手册中的说明不足，请参考 "[**1.3.2 SYCON.NET 帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" 功能。
{% endhint %}

<br>

**1. 在 PCI 插槽设置中选择 PROFINET IO 主控并重启机器人控制器。**

![[Figure 1.3.4.2-1 PCI 插槽设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查所选协议的就绪状态。**

<br>

{% hint style="info" %}
   - 有关在 TP 上检查工业通信状态的程序，请参考 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

<br>

![[Figure 1.3.4.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

**3. 使用 Sycon.net 选择 PROFINET IO 控制器 PCI 设备。**

![[Figure 1.3.4.2-3 PROFINET IO 主控 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_3.png>)
![[Figure 1.3.4.2-4 PROFINET IO 主控 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

**4. 扫描 PCI 设备并应用 PROFINET IO 控制器。**

![[Figure 1.3.4.2-5 Sycon.net 扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

**5. 下载设置。**

![[Figure 1.3.4.2-6 PROFINET IO 控制器下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

**6. 准备要连接到 PROFINET IO 控制器的设备（从属）模块。**
   * 在本示例中，我们使用 Crevis 的 M9287 PROFINET IO 设备。
   * 请供应系统电源和现场电源以激活模块。

![[Figure 1.3.4.2-7 Crevis M9287]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
   - 如何使用 DIP 开关设置 PROFINET IO 设备名称

   - M9287-XX: 使用 DIP 开关设置的编号

   - 在本示例中，名称使用 DIP 开关 1 设置为 M9287-01。
{% endhint %}

<br>

**7. （DIP 开关使用示例）使用 DIP 开关设置从属设备名称。**
   * 仅更改 DIP 开关 1 为 ON。

![[Figure 1.3.4.2-8 Crevis M9287 DIP 开关]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
   - 设置 DIP 开关后，请重启设备。
{% endhint %}

<br>

**8. 注册从属设备 GSDML 文件。**

{% hint style="info" %}
   - 使用未在 Sycon.net 中注册的设备时，需要 GSDML 文件。

   - M9287 设备的 GSDML 文件可以从 Crevis 网站下载。
{% endhint %}

![[Figure 1.3.4.2-9 Crevis GSDML 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
   - 在 Sycon.net 中注册下载的 GSDML 文件。

   - 注册 GSDML 文件时，请检查工业通信协议（PROFINET IO）。
{% endhint %}

![[Figure 1.3.4.2-10 Crevis GSDML 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_10.png>)![[Figure 1.3.4.2-11 Crevis GSDML 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_11.png>)
![[Figure 1.3.4.2-12 Crevis GSDML 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_12.png>)

![[Figure 1.3.4.2-13 Crevis GSDML 文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_13.png>)

<br>

**9. 网络扫描**

{% hint style="info" %}
   - PROFINET IO 控制器支持网络扫描功能。
{% endhint %}

{% hint style="info" %}
   - 右击 PROFINET IO 主控设备并单击网络扫描。
{% endhint %}

![[Figure 1.3.4.2-14 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
   - 如果没有注册 GSDML 文件，则在执行网络扫描功能时，将出现从属信息，但无法注册。
{% endhint %}

![[Figure 1.3.4.2-15 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - 如果正常注册了 GSDML 文件，则可以使用网络扫描功能添加从属设备。
{% endhint %}

![[Figure 1.3.4.2-16 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_16.png>)

![[Figure 1.3.4.2-17 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_17.png>)

![[Figure 1.3.4.2-18 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

**10. 配置从属（设备）。**

{% hint style="info" %}
   - 单击主控设备上的断开连接以配置从属设备。
{% endhint %}

![[Figure 1.3.4.2-19 从属配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - 双击从属设备。
{% endhint %}

![[Figure 1.3.4.2-20 从属配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - 添加连接到 M9287 的插槽以设置 PROFINET IO 从属（设备）。

   - 插槽 1 : M7001  
   - 插槽 2 : M12DF  
   - 插槽 3 : M225F  
{% endhint %}

![[Figure 1.3.4.2-21 从属配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_21.png>)

![[Figure 1.3.4.2-22 从属配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

**11. 配置主控（控制器）设备**

{% hint style="info" %}
   - 双击主控设备。
{% endhint %}

![[Figure 1.3.4.2-23 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - 设置主控和从属设备的 IP 地址。

   - PROFINET IO 设备的从属 IP 地址应从主控设置。

   - 请确保主控和从属的 IP 地址在同一段内不重叠。
{% endhint %}

![[Figure 1.3.4.2-24 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_24.png>)

![[Figure 1.3.4.2-25 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - 从主控设备检查从属设备的插槽信息是否正确。
{% endhint %}

![[Figure 1.3.4.2-26 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 在地址表中检查每个从属插槽的 IO 和起始地址分配。
{% endhint %}

![[Figure 1.3.4.2-27 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - 设置 PROFINET IO 的 IO 通信速度。
{% endhint %}

![[Figure 1.3.4.2-28 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - 完成设置后，请继续下载。
{% endhint %}

![[Figure 1.3.4.2-29 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

**12. 检查通信状态。**

{% hint style="info" %}
   - 在 Sycon.net 和 TP 中检查通信状态。

   - 有关在 TP 上检查工业通信状态的程序，请参阅 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

{% hint style="info" %}
   - 双击连接的主控设备以检查通信状态。
{% endhint %}

![[Figure 1.3.4.2-30 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_30.png>)

![[Figure 1.3.4.2-31 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
   - 使用 Sycon.net 的诊断功能，您可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.4.2-32 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_32.png>)

<br>

**13. 在完成设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参见 ("[**4. 工业通信 IO 块分配**](../../../4-io-block-allocation.md)")。**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/3-Specification-PROFINET-IO-Device.md)
#### 1.3.4.3 PROFINET IO设备规格

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>最大输入大小</td>
		<td>256字节 (TP) / 1024字节 (Sycon.net)</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>256字节 (TP) / 1024字节 (Sycon.net)</td>
	</tr>
    <tr>
		<td>IO连接</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO更新周期</td>
		<td>最小1ms</td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>100 Mbit/s (全双工)</td>
	</tr>
    <tr>
		<td>拓扑</td>
		<td>树形，线形</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>DCP</td>
		<td>支持</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>自动协商</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>集线器</td>
		<td>禁止</td>
	</tr>
    <tr>
		<td>交换机</td>
		<td>仅在交换机支持优先级标记和LLDP时允许</td>
	</tr>
</tbody>
</table>
<br>

**连接**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>电缆</td>
		<td>至少为Cat5，STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最大100m</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Settings-PROFINET-IO-Device.md)
#### 1.3.4.4 PROFINET IO设备设置

请遵循 "[**1.3.1 CIFX PCI槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 程序，然后继续下面的方法。

<br>

{% hint style="info" %}
   **[PROFINET IO设备GSDML文件下载]**

   - 请参阅 "[**5. 从设备描述文件**](../../../5-slave-config-file.md)"。
{% endhint %}

<br>

**1. 使用TP，在工业通信固件设置中选择PROFINET IO从设备并重启机器人控制器。**

![[Figure 1.3.4.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_1.png>)

<br>

**2. 检查工业通信监控菜单中当前通信协议的就绪状态。**

![[Figure 1.3.4.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意\]**: 如果使用Sycon.net设置的配置文件下载到相应的PCI槽，则TP设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单进入从设备设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从槽设置 > PROFINET IO从设备]**

![[Figure 1.3.4.4-3 从设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[Figure 1.3.4.4-4 从设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

**4. 每个项目的说明**

{% hint style="info" %}
   [站点名称]

   - PROFINET IO通过站点名称识别从设备。

   - 命名规则
      - 通过PROFINET IO连接的设备名称不能重复。  
      - 名称最多可以设置为240个字符。  
      - 可以使用特殊字符"."和"-"。  
      - 可以使用小写英文字母和数字。  
      - 名称应以小写英文字母或数字开头和结尾。  
{% endhint %}

{% hint style="info" %}
   [输入字节数（输入字节）]

   - 输入字节数：设置从主设备->从设备的数据输入大小。
{% endhint %}

{% hint style="info" %}
   [输出字节数（输出字节）]

   - 输出字节数：设置从设备->主设备的数据输出大小。
{% endhint %}

<br>

{% hint style="info" %}
   [**从主设备设置一个槽时**]

   - 主输入（32字节）  <--  从输出（32字节）

   - 主输出（256字节 = 64字节 * 4）  -->  从输入（256字节）

   - 4, 8, 16, 32和64字节 -> 指定与每个字节数匹配的槽  
   - 128和256字节 -> 指定多个64字节槽（2, 4）

   - 输入槽位于输出槽之前。
{% endhint %}

<br>

![[Figure 1.3.4.4-5 从设备设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_5.png>) 

<br>

**5. 完成设置后，按照以下程序检查通信状态。**

有关在TP上检查工业通信状态的程序，请参阅 ("[**1.4 CIFX PCI通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。

![[Figure 1.3.4.4-6 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_6.png>)

<br>

**6. 完成通信设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块使用输入/输出信号。请参阅 ("[**4. 工业通信IO块分配**](../../../4-io-block-allocation.md)")。**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/5-Error-PROFINET-IO.md)
#### 1.3.4.5 PROFINET IO 错误处理

<br>

请参考 "[**1.4.1 错误代码**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/README.md)
### 1.3.5 EtherCAT

本章描述了EtherCAT主设备和从设备的特性以及如何设置它们。

<br>

**EtherCAT概述**

EtherCAT是由Beckhoff Automation开发的基于以太网的现场总线系统。

EtherCAT协议提供了非常快速的IO数据更新和精确的同步功能。

<br>

**EtherCAT主设备**
   * 对应现有现场总线主设备的产品，并可以请求EtherCAT从设备执行I/O数据连接。

<br>

**EtherCAT从设备**
   * 对应现有现场总线从设备的产品，并连接到EtherCAT主设备。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/1-Specification-EtherCAT-Master.md)
#### 1.3.5.1 EtherCAT Master Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>最大可连接从设备数量</td>
		<td>200</td>
	</tr>
    <tr>
		<td>最大输入大小</td>
		<td>1200 字节</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>1200 字节</td>
	</tr>
    <tr>
		<td>最大输入大小（1 个从设备）</td>
		<td>256 字节</td>
	</tr>
    <tr>
		<td>最大输出大小（1 个从设备）</td>
		<td>256 字节</td>
	</tr>
    <tr>
		<td>IO 连接</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 更新周期</td>
		<td>最小 250us (推荐 1ms)</td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>100 Mbit/s (全双工)</td>
	</tr>
    <tr>
		<td>拓扑结构</td>
		<td>线型，环形</td>
	</tr>
    <tr>
		<td>网络从设备扫描</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>冗余</td>
		<td>支持（与同步无法同时应用）</td>
	</tr>
    <tr>
		<td>同步</td>
		<td>DC（分布式时钟）</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>自动协商</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>集线器</td>
		<td>禁止</td>
	</tr>
    <tr>
		<td>交换机</td>
		<td>仅允许在主设备和第一个从设备之间</td>
	</tr>
</tbody>
</table>
<br>

**连接**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>电缆</td>
		<td>最低 Cat5，STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最大 100m</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Settings-EtherCAT-Master.md)
#### 1.3.5.2 EtherCAT主控设置

请遵循 "[**1.3.1 CIFX PCI插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 和 "[**1.3.2 SYCON.NET设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 的步骤，然后按下面的方法进行。

<br>

{% hint style="info" %}
   - 使用SYCON.net时，如果手册中的解释不足，请参考 "[**1.3.2 SYCON.NET帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" 功能。
{% endhint %}

<br>

**1.在PCI插槽设置中选择EtherCAT主控并重启机器人控制器。**

![[Figure 1.3.5.2-1 PCI插槽设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_1.png>) 

<br>

**2.在工业通信监控菜单中检查所选协议的就绪状态。**

<br>

{% hint style="info" %}
   - 检查TP上工业通信状态的程序，请参阅 ("[**1.4 CIFX PCI通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

<br>

![[Figure 1.3.5.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_2.png>) 

<br>

**3.使用Sycon.net选择EtherCAT主控PCI设备。**

![[Figure 1.3.5.2-3 EtherCAT主控PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_3.png>)
![[Figure 1.3.5.2-4 EtherCAT主控PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_4.png>) 

<br>

**4.扫描PCI设备并应用EtherCAT主控。**

![[Figure 1.3.5.2-5 Sycon.net扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_5.png>) 

<br>

**5.下载设置。**

![[Figure 1.3.5.2-6 EtherCAT主控下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_6.png>) 

<br>

**6.准备要连接到EtherCAT主控的从模块。**
   * 在本例中，我们使用Crevis的M9386 EtherCAT从设备。
   * 请供电系统电源和现场电源以激活模块。

![[Figure 1.3.5.2-7 Crevis M9386]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_7.png>) 

<br>

**7.从设备站地址**

{% hint style="info" %}
   - EtherCAT从设备的站地址由主控设置。
{% endhint %}

<br>

**8.注册从设备XML文件。**

{% hint style="info" %}
   - 使用未在Sycon.net中注册的设备需要XML文件。

   - M9386设备的XML文件可以从Crevis官网上下载。
{% endhint %}

![[Figure 1.3.5.2-8 Crevis XML文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_8.png>)

{% hint style="info" %}
   - 在Sycon.net中注册下载的XML文件。

   - 注册XML文件时，请检查工业通信协议（EtherCAT）。
{% endhint %}

![[Figure 1.3.5.2-9 Crevis XML文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_9.png>)

<br>

![[Figure 1.3.5.5-10 Crevis XML文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.5.2-11 Crevis XML文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_11.png>)

<br>

![[Figure 1.3.5.2-12 Crevis XML文件]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_12.png>)


<br>

**9.网络扫描**

{% hint style="warning" %}
   **对于EtherCAT，指定了可用的电缆连接和端口。**

   **为了顺畅的通信连接，务必检查 ("[**1.3.5.5 EtherCAT电缆布线**](../5-EtherCAT/5-EtherCAT-Topology.md)")。**
{% endhint %}

{% hint style="info" %}
   - EtherCAT主控支持网络扫描功能。
{% endhint %}

{% hint style="info" %}
   - 右键单击EtherCAT主控设备，点击网络扫描。
{% endhint %}

![[Figure 1.3.5.2-13 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_13.png>)

{% hint style="warning" %}
   - 如果没有注册XML文件，进行网络扫描功能时将出现从设备信息，但无法注册。
{% endhint %}

{% hint style="info" %}
   - 如果XML文件正常注册，则可以使用网络扫描功能添加从设备。
{% endhint %}

![[Figure 1.3.5.2-14 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_14.png>)

<br>

**10.配置从设备。**

{% hint style="info" %}
   - 点击主控设备上的断开以配置从设备。
{% endhint %}

![[Figure 1.3.5.2-15 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - 双击从设备。
{% endhint %}

![[Figure 1.3.5.2-16 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_16.png>)

{% hint style="info" %}
   - 添加连接到M9386的插槽以设置EtherCAT从设备。

   - 插槽1：M7001  
   - 插槽2：M12DF  
   - 插槽3：M225F  
{% endhint %}

![[Figure 1.3.5.2-17 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_17.png>)

![[Figure 1.3.5.2-18 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_18.png>)


<br>

**11.配置主设备。**

{% hint style="info" %}
   - 双击主设备。
{% endhint %}

![[Figure 1.3.5.2-19 主设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - 同步：选择Freerun/DC（分布时钟）。

   - 是否使用冗余（不能与分布时钟同时使用）

   - 总线周期时间：至少支持250 us。（建议1 ms或更长。）
{% endhint %}

<br>

{% hint style="info" %}
   - 您可以为每个从设备设置站地址。
{% endhint %}

![[Figure 1.3.5.2-20 主设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - 检查地址表中每个从设备插槽的分配IO和起始地址。
{% endhint %}

![[Figure 1.3.5.2-21 主设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_21.png>)


{% hint style="info" %}
   - 完成设置后，继续下载。
{% endhint %}

![[Figure 1.3.5.2-22 主设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_22.png>)

<br>

**12.检查通信状态。**

{% hint style="info" %}
   - 在Sycon.net和TP中检查通信状态。

   - 检查TP上的工业通信状态程序，请参阅 ("[**1.4 CIFX PCI通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

{% hint style="info" %}
   - 双击连接的主设备以检查通信状态。
{% endhint %}

![[Figure 1.3.5.2-23 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_23.png>)

![[Figure 1.3.5.2-24 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - 使用Sycon.net的诊断功能，您可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.5.2-25 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_25.png>)

<br>

**13.完成设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块来使用输入/输出信号。请参阅 ("[**4.工业通信IO块分配**](../../../4-io-block-allocation.md)")。**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/3-Specification-EtherCAT-Slave.md)
#### 1.3.5.3 EtherCAT从站规范

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>最大输入大小</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>IO连接</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO更新周期</td>
		<td>最小250us（推荐1ms）</td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>100 Mbit/s （全双工）</td>
	</tr>
    <tr>
		<td>拓扑</td>
		<td>线型，环型</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>同步</td>
		<td>DC（分布式时钟）</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>Ethernet II，IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>自动协商</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>集线器</td>
		<td>禁止</td>
	</tr>
    <tr>
		<td>交换机</td>
		<td>仅允许在主设备和第一个从设备之间</td>
	</tr>
</tbody>
</table>
<br>

**连接**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>电缆</td>
		<td>至少Cat5，STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最大100m</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Settings-EtherCAT-Slave.md)
#### 1.3.5.4 EtherCAT 从站设置

手册正在准备中。

<br>

{% hint style="info" %}
   **[EtherCAT 从站 ESI 文件下载]**

   - 请参考 "[**5. 从站设备描述文件**](../../../5-slave-config-file.md)"。
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-EtherCAT-Topology.md)
#### 1.3.5.5 EtherCAT 电缆接线（拓扑）

<br>

与现有的工业通信不同，EtherCAT 在电缆接线和可用以太网端口方面有限制。

**1. 以太网端口**

{% hint style="info" %}
   - 连接 EtherCAT 主站和从站时，应使用端口 0。
{% endhint %}

![[Figure 1.3.5.5-1 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
   - 当一个从站连接到主站时
{% endhint %}

![[Figure 1.3.5.5-2 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
   - 当两个或更多从站连接到主站时

   - 从从站端口 1 连接到下一个从站端口 0。
{% endhint %}

![[Figure 1.3.5.5-3 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_3.png>)

<br>

**2. 冗余**

{% hint style="info" %}
   - 在主站中使用冗余功能时

   - 连接最后一个从站的端口 1 和主站的端口 1 以形成环结构。
{% endhint %}

![[Figure 1.3.5.5-4 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_4.png>) 


<br>

**3. 电缆接线错误**


请参考 "[**1.4.1 错误代码**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"。

<br>

{% hint style="info" %}
   - 如果网络扫描功能不起作用。

   - 请检查连接到主站的端口和电缆。
{% endhint %}

![[Figure 1.3.5.5-5 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
   - 拓扑错误（配置错误）

   - 请检查主站和从站之间的电缆接线。
{% endhint %}

![[Figure 1.3.5.5-6 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
   - 拓扑错误 2（配置时正常，但诊断时出现错误）

   - 请检查主站和从站之间的电缆接线。

   - 请检查从站之间的电缆接线。
{% endhint %}

![[Figure 1.3.5.5-7 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_7.png>)

![[Figure 1.3.5.5-8 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
   - 必须的从站缺失错误

   - 请检查从站之间的电缆接线。
{% endhint %}

![[Figure 1.3.5.5-9 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_9.png>)
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/README.md)
### 1.3.6 PROFIBUS-DP

本章描述了PROFIBUS-DP主设备和从设备的特性以及如何设置它们。

<br>

**现场总线概述**

现场总线是一个行业标准，旨在通过单一电缆将传感器、按钮、电机驱动器和操作界面等设备连接到PLC（可编程逻辑控制器）并在工厂中运行。

现场总线提供智能服务，例如对整个网络状态的中央监控和网络的重新配置。

例如，可以为传感器和开关设置详细的信息、操作和模式，而不仅仅是简单的开/关。

使用单一电缆可以减少布线的时间和成本，简化配置，并提供维护上的优势。

此外，与一般通信的非确定性响应特性协议不同，现场总线保证数据响应速度以满足对时间特性重要的工业应用。

![[Figure 1.3.6-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/image_1.png>)

<br>

一个现场总线网络连接一个主设备和多个从设备。 主设备搜索和管理整个网络，并与从设备交换数据。

通常，PLC是主设备，而传感器、按钮、控制器等可以配置为从设备。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/1-Specification-PROFIBUS-DP-Master.md)
#### 1.3.6.1 PROFIBUS-DP Master Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>最大可连接从设备数</td>
		<td>125</td>
	</tr>
    <tr>
		<td>最大输入大小</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>最大输入大小（1 个从设备）</td>
		<td>244 bytes</td>
	</tr>
    <tr>
		<td>最大输出大小（1 个从设备）</td>
		<td>244 bytes</td>
	</tr>
    <tr>
		<td>IO 连接</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 更新周期</td>
		<td> - </td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>9.6 ~ 12,000 Kbit/s</td>
	</tr>
    <tr>
		<td>拓扑结构</td>
		<td> - </td>
	</tr>
    <tr>
		<td>网络从设备扫描</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>自动波特率检测</td>
		<td>不支持</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>PROFIBUS FDL</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Settings-PROFIBUS-DP-Master.md)
#### 1.3.6.2 PROFIBUS-DP 主控设置

请遵循 "[**1.3.1 CIFX PCI 插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 和 "[**1.3.2 SYCON.NET 设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 的程序，然后继续进行以下方法。

<br>

{% hint style="info" %}
   - 使用 SYCON.net 时，如果手册中的解释不够，请参考 "[**1.3.2 SYCON.NET 帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" 功能。
{% endhint %}

<br>

**1. 在 PCI 插槽设置中选择 PROFIBUS-DP 主控，并重启机器人控制器。**

![[Figure 1.3.6.2-1 PCI 插槽设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查选定协议的准备状态。**

<br>

{% hint style="info" %}
   - 有关在 TP 上检查工业通信状态的程序，请参考 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

<br>

![[Figure 1.3.6.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_2.png>)

<br>

**3. 使用 Sycon.net 选择 PROFIBUS-DP 主控 PCI 设备。**

![[Figure 1.3.6.2-3 PROFIBUS-DP 主控 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[Figure 1.3.6.2-4 PROFIBUS-DP 主控 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

**4. 扫描 PCI 设备并应用 PROFIBUS-DP 主控。**

![[Figure 1.3.6.2-5 Sycon.net 扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>

**5. 下载设置。**

![[Figure 1.3.6.2-6 PROFIBUS-DP 主控下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

**6. 准备要连接到 PROFIBUS-DP 主控的从设备模块。**
   * 在此示例中，我们使用来自 Crevis 的 GN-9222 PROFIBUS-DP 从设备。
   * 请提供系统电源和现场电源以激活模块。

![[Figure 1.3.6.2-7 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_7.png>) 

<br>

**7. 设置从设备**

{% hint style="info" %}
   - 设置 PROFIBUS-DP 从设备的节点编号和终止。
{% endhint %}

![[Figure 1.3.6.2-8 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
   - 终止：使用 DIP 开关设置（示例：终止处理开启）

   - 节点 ID（站号）：使用 DIP 开关设置（示例：节点 3）
{% endhint %}

<br>

**8. 注册从设备 GSD 文件。**

{% hint style="info" %}
   - 使用未在 Sycon.net 注册的设备时需要 GSD 文件。

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
   **执行网络扫描功能时，请务必检查以下内容。**

   **(1) 电缆是否连接。**  
   **(2) 是否使用终止 DIP 开关。**  
{% endhint %}

{% hint style="info" %}
   - PROFIBUS-DP 主控支持网络扫描功能。
{% endhint %}

{% hint style="info" %}
   - 右键单击 PROFIBUS-DP 主控设备，然后单击网络扫描。
{% endhint %}

![[Figure 1.3.6.2-13 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
   - 如果没有注册 GSD 文件，执行网络扫描功能时会显示从设备信息，但无法注册。
{% endhint %}

{% hint style="info" %}
   - 如果 GSD 文件正常注册，则可以使用网络扫描功能添加从设备。
{% endhint %}

![[Figure 1.3.6.2-14 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

**10. 配置从设备**

{% hint style="info" %}
   - 点击主控设备上的断开以配置从设备。
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

**11. 配置主控设备。**

{% hint style="info" %}
   - 双击主控设备。
{% endhint %}

![[Figure 1.3.6.2-19 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - 设置 PROFIBUS-DP 通信速度。

   - 9.6 - 12000 Kbit/s 
{% endhint %}

![[Figure 1.3.6.2-20 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - 从主控设备检查从设备的插槽信息是否正确。
{% endhint %}

![[Figure 1.3.6.2-21 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
   - 检查地址表中每个从设备的分配 IO 和起始地址。
{% endhint %}

![[Figure 1.3.6.2-22 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
   - 检查站表中每个设备是否处于活动状态。
{% endhint %}

![[Figure 1.3.6.2-23 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - 完成设置后，继续下载。
{% endhint %}

![[Figure 1.3.6.2-24 主控配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

**12. 检查通信状态。**

{% hint style="info" %}
   - 在 Sycon.net 和 TP 中检查通信状态。

   - 有关在 TP 上检查工业通信状态的程序，请参考 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

{% hint style="info" %}
   - 双击连接的主控设备以检查通信状态。
{% endhint %}

![[Figure 1.3.6.2-25 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[Figure 1.3.6.2-26 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 使用 Sycon.net 的诊断功能，您可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.6.2-27 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_27.png>)

<br>

**13. 在完成设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[**4. 工业通信 IO 块分配**](../../../4-io-block-allocation.md)")。**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/3-Specification-PROFIBUS-DP-Slave.md)
#### 1.3.6.3 PROFIBUS-DP Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>最大输入大小</td>
		<td>244 字节</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>244 字节</td>
	</tr>
    <tr>
		<td>IO连接</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO更新周期</td>
		<td> - </td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>9.6 ~ 12,000 Kbit/s</td>
	</tr>
    <tr>
		<td>拓扑结构</td>
		<td> - </td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>自动波特率检测</td>
		<td>支持</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>PROFIBUS FDL</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Settings-PROFIBUS-DP-Slave.md)
#### 1.3.6.4 PROFIBUS-DP 从站设置

请按照 "[**1.3.1 CIFX PCI 插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 的程序进行操作，然后继续下面的方法。

<br>

{% hint style="info" %}
   **[PROFIBUS-DP 从站 GSD 文件下载]**

   - 请参考 "[**5. 从设备描述文件**](../../../5-slave-config-file.md)"。
{% endhint %}

<br>

**1. 使用 TP 选择工业通信固件设置中的 PROFIBUS-DP 从站，并重新启动机器人控制器。**

![[Figure 1.3.6.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查当前通信协议的准备状态。**

![[Figure 1.3.6.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[注意]**：如果通过 Sycon.net 下载的配置文件被设置到相应的 PCI 插槽，则 TP 设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单以进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI 从站插槽设置 > PROFIBUS-DP 从站]**

![[Figure 1.3.6.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.6.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

<br>

**4. 各项的描述**

{% hint style="info" %}
   [站地址]

   - PROFIBUS-DP 通过站地址识别从站。
{% endhint %}

{% hint style="info" %}
   [输入字节数 (输入字节)]

   - 输入字节数：设置从主设备 -> 从设备的数据输入大小。
{% endhint %}

{% hint style="info" %}
   [输出字节数 (输出字节)]

   - 输出字节数：设置从设备 -> 主设备的数据输出大小。
{% endhint %}

{% hint style="info" %}
   [**从主设备设置模块时**]

   - 模块应从主设备指定以匹配设置的字节数。

   - 顺序：主输入 (64-1) -> 主输出 (64-1)

   - 示例) 主输入 109 字节  <---  从输出 109 字节   
         - 输入 109 字节：64Byte + 32Byte + 8Byte + 4Byte + 1 Byte

   - 示例) 主输出 120 字节  --->  从输入 120 字节   
         - 输出 120 字节：64Byte + 32Byte + 16Byte + 8Byte


   - 示例) 主输入 12 字节  <---  从输出 12 字节   
         - 输入 12 字节：8Byte + 4Byte

   - 示例) 主输出 200 字节  --->  从输入 200 字节   
         - 输出 200 字节：64Byte + 64Byte + 64Byte + 8Byte

   - 输入模块位于输出模块之前。
{% endhint %}

![[Figure 1.3.6.4-5 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>)


<br>

**5. 完成设置后，请按照下面的程序检查通信状态。**

有关在 TP 上检查工业通信状态的程序，请参考 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。

![[Figure 1.3.6.4-6 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>)

<br>

**6. 完成通信设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[**4. 工业通信 IO 块分配**](../../../4-io-block-allocation.md)")。**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/5-Error-PROFIBUS-DP.md)
#### 1.3.6.5 PROFIBUS-DP 错误处理

<br>

请参阅 "[**1.4.1 错误代码**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/README.md)
### 1.3.7 DeviceNet

本章描述了DeviceNet主设备和从设备的特性以及如何设置它们。

<br>

**现场总线概述**

现场总线是一种行业标准，已开放用于连接传感器、按钮、电机驱动器和操作接口等设备到PLC（可编程逻辑控制器），通过单根电缆在工厂中操作它们。

现场总线提供智能服务，例如对整个网络状态的集中监控和网络的重新配置。

例如，可以为传感器和开关设置详细信息、操作和模式，而不仅仅是简单的开/关。

使用单根电缆减少了布线的时间和成本，简化了配置，并在维护上提供了优势。

此外，与一般通讯的非确定性响应特性的协议不同，现场总线路由确保数据响应速度，以满足对关键时间特性要求高的工业应用。

![[Figure 1.3.7-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/image_1.png>)

<br>

一个现场总线网络连接一个主设备和多个从设备。
主设备搜索并管理整个网络，并与从设备交换数据。

通常，PLC是主设备，而传感器、按钮、控制器等可以配置为从设备。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/1-Specification-DeviceNet-Master.md)
#### 1.3.7.1 DeviceNet 主设备规格

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>最大可连接从设备数量</td>
		<td>63</td>
	</tr>
    <tr>
		<td>最大输入大小</td>
		<td>1200 字节</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>1200 字节</td>
	</tr>
    <tr>
		<td>最大输入大小 (1 个从设备)</td>
		<td>255 字节</td>
	</tr>
    <tr>
		<td>最大输出大小 (1 个从设备)</td>
		<td>255 字节</td>
	</tr>
    <tr>
		<td>IO 连接</td>
		<td>位脉冲 <br>状态变化 <br>循环 <br>轮询</td>
	</tr>
    <tr>
		<td>IO 更新周期</td>
		<td> - </td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>125 ~ 500 Kbit/s</td>
	</tr>
    <tr>
		<td>拓扑结构</td>
		<td> - </td>
	</tr>
    <tr>
		<td>网络从设备扫描</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>自动波特率检测</td>
		<td>不支持</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>CAN 帧</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Settings-DeviceNet-Master.md)
#### 1.3.7.2 DeviceNet 主设置

请遵循 "[**1.3.1 CIFX PCI 插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 和 "[**1.3.2 SYCON.NET 设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 的程序，然后按照下面的方法进行操作。

<br>

{% hint style="info" %}
   - 使用 SYCON.net 时，如果手册中说明不够详细，请参考 "[**1.3.2 SYCON.NET 帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" 功能。
{% endhint %}

<br>

{% hint style="info" %}
   - 有关 DeviceNet 连接器连接，请参考以下内容。

      ("[**1.2.2 连接器**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. 在 PCI 插槽设置中选择 DeviceNet 主控器，并重启机器人控制器。**

![[Figure 1.3.7.2-1 PCI 插槽设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_1.png>)

<br>

**2. 在工业通信监控菜单中检查所选协议的准备状态。**

<br>

{% hint style="info" %}
   - 有关在 TP 上检查工业通信状态的程序，请参见 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

<br>

![[Figure 1.3.7.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_2.png>) 

<br>

**3. 使用 Sycon.net 选择 DeviceNet 主 PCI 设备。**

![[Figure 1.3.7.2-3 DeviceNet 主 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_3.png>)
![[Figure 1.3.7.2-4 DeviceNet 主 PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_4.png>) 

<br>

**4. 扫描 PCI 设备并应用 DeviceNet 主控器。**

![[Figure 1.3.7.2-5 Sycon.net 扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_5.png>) 

<br>

**5. 设置通信速率。**

{% hint style="warning" %}
   - 如果主控器和从设备之间的通信速率不同，网络扫描功能将无法正常工作。
{% endhint %}

![[Figure 1.3.7.2-6 DeviceNet 主下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_6.png>) 

<br>

**6. 下载设置。**

![[Figure 1.3.7.2-7 DeviceNet 主下载]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_7.png>) 

<br>

**7. 准备要连接到 DeviceNet 主控器的从模块。**
   * 在本示例中，我们使用 Crevis 的 NA-9211 DeviceNet 从设备。
   * 请供电以激活该模块。

![[Figure 1.3.7.2-8 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_8.png>) 

<br>

**8. 设置从设备。**

{% hint style="info" %}
   - 设置 DeviceNet 从设备的 MAC ID、通信速率和终结电阻。
{% endhint %}

![[Figure 1.3.7.2-9 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_9.png>) 

![[Figure 1.3.7.2-10 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_10.png>)

{% hint style="info" %}
   [示例设置]

   - 终结电阻：通过安装在电缆中使用（终结 DIP 开关关闭）

   - MAC ID（站号）：设置为 4（仅 DIP 开关 3 开启）

   - 通信速率（波特率）：设置为自动（DIP 开关 7 和 8 开启）
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
   **执行网络扫描功能时，请务必检查以下内容。**

   **(1) 是否连接了电缆。**  
   **(2) 是否连接了终结电阻或使用了终结 DIP 开关。**  
   **(3) 主设备和从设备的通信速率是否设置。**  

   **为了顺畅的通信连接，请务必检查 ("[**1.3.7.5 DeviceNet 错误处理**](../7-DeviceNet/5-Error-DeviceNet.md)")。**
{% endhint %}

{% hint style="info" %}
   - DeviceNet 主控器支持网络扫描功能。
{% endhint %}

{% hint style="info" %}
   - 右键单击 DeviceNet 主设备并单击网络扫描。
{% endhint %}

![[Figure 1.3.7.2-14 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
   - 如果没有注册 EDS 文件，执行网络扫描功能时将显示从设备信息，但无法注册。
{% endhint %}

{% hint style="info" %}
   - 如果 EDS 文件正常注册，则可以使用网络扫描功能添加从设备。
{% endhint %}

![[Figure 1.3.7.2-15 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_15.png>)

![[Figure 1.3.7.2-16 网络扫描]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_16.png>)

<br>

**11. 配置从设备**

{% hint style="info" %}
   - 单击主设备上的断开连接以配置从设备。
{% endhint %}

![[Figure 1.3.7.2-17 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
   - 双击从设备。
{% endhint %}

![[Figure 1.3.7.2-18 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_18.png>)

<br>

{% hint style="info" %}
   - 设置从设备的连接类型。

   - 选择用于 DeviceNet 通信连接的信息传输方式。

   **如果未选中 UCMM 复选框，则默认值设置为 UCMM 第 2 组。**   

   - UCMM 第 1 组 : IO 消息   
   - UCMM 第 2 组: 网络初始化期间的主 - 从连接消息（默认设置）   
   - UCMM 第 3 组: 明确消息   

   - 对于某些设备，可能会使用 UCMM 第 3 组，因此请在进行操作前查看产品规格。
{% endhint %}

![[Figure 1.3.7.2-19 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_19.png>)

<br>

{% hint style="info" %}
   - 对于 Crevis NA-9211，请在不勾选 UCMM 复选框的情况下进行操作。（使用第 2 组默认值。）
{% endhint %}

![[Figure 1.3.7.2-20 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_20.png>)

<br>

{% hint style="info" %}
   - 检查 DeviceNet 从设备设置。

   - 输出：ST-2318 (1 字节)  
   - 输入：ST-1218 (1 字节)  
{% endhint %}

<br>

{% hint style="info" %}
   - 根据通信方式（轮询、状态变化、周期、位脉冲）进行设置。
{% endhint %}

<br>

![[Figure 1.3.7.2-21 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_21.png>)

<br>

{% hint style="info" %}
   [生产抑制时间]

   - 设置从设备的 IO 数据生成周期（毫秒）  

   - 示例） 10 毫秒：每 10 毫秒生成一次 IO 数据。  
   - 示例） 0 毫秒：从设备尽快生成 IO 数据。  

   - 周期越短，从设备上的负载可能越大。（需要检查每个从设备的规格。） 
{% endhint %}

<br>

{% hint style="info" %}
   [预期数据包速率]

   - 设置主设备和从设备之间的 IO 数据更新间隔。  
{% endhint %}

<br>

![[Figure 1.3.7.2-22 从设备配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_22.png>)

<br>

**12. 配置主设备**

{% hint style="info" %}
   - 双击主设备。
{% endhint %}

![[Figure 1.3.7.2-23 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - 设置 DeviceNet 通信速率（与从设备通信速率相同）。
{% endhint %}

![[Figure 1.3.7.2-24 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - 在地址表中检查每个从设备插槽的分配的 IO 和起始地址。
{% endhint %}

![[Figure 1.3.7.2-25 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - 设置是否使用快速连接功能。
{% endhint %}

![[Figure 1.3.7.2-26 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - 设置完成后，继续进行下载。
{% endhint %}

![[Figure 1.3.7.2-27 主配置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_27.png>)

<br>

**13. 检查通信状态。**

{% hint style="info" %}
   - 检查 Sycon.net 和 TP 中的通信状态。

   - 有关在 TP 上检查工业通信状态的程序，请参见 ("[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。
{% endhint %}

{% hint style="info" %}
   - 双击已连接的主设备以检查通信状态。
{% endhint %}

![[Figure 1.3.7.2-28 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_28.png>)

![[Figure 1.3.7.2-29 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_29.png>)

{% hint style="info" %}
   - 使用 Sycon.net 的诊断功能，您可以监控通信状态和输入/输出状态。
{% endhint %}

![[Figure 1.3.7.2-30 状态诊断]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_30.png>)
<br>

**14. 完成通信设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Specification-DeviceNet-Slave.md)
#### 1.3.7.3 DeviceNet 从设备规格

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>最大输入大小</td>
		<td>255 字节</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>255 字节</td>
	</tr>
    <tr>
		<td>IO 连接</td>
		<td>位触发 <br>状态变化 <br>周期 <br>轮询</td>
	</tr>
    <tr>
		<td>IO 更新周期</td>
		<td> - </td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>125 ~ 500 Kbit/s</td>
	</tr>
    <tr>
		<td>拓扑结构</td>
		<td> - </td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td> - </td>
	</tr>
    <tr>
		<td>自动波特率检测</td>
		<td>不支持</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>CAN 帧</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Settings-DeviceNet-Slave.md)
#### 1.3.7.4 DeviceNet从站设置

请遵循 "[**1.3.1 CIFX PCI插槽设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 过程，然后继续以下方法。

<br>

{% hint style="info" %}
   **[DeviceNet从站EDS文件下载]**

   - 请参考 "[**5. 从设备描述文件**](../../../5-slave-config-file.md)." 
{% endhint %}

<br>

{% hint style="info" %}
   - 关于DeviceNet连接器连接，请参见以下内容。

      ("[**1.2.2 连接器**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. 使用TP，在工业通信固件设置中选择DeviceNet从站，并重新启动机器人控制器。**

![[图 1.3.7.4-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_1.png>) 

<br>

**2. 检查工业通信监控菜单中的当前通信协议就绪状态。**

![[图 1.3.7.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[警告]**: 如果使用Sycon.net设置的配置文件被下载到相应的PCI插槽，TP设置将被忽略。
{% endhint %}

<br>

**3. 触摸菜单以进入从站设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从槽设置 > DeviceNet从站]**

![[图 1.3.7.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_3.png>) 

![[图 1.3.7.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_4.png>) 

<br>

**4. 各项描述**

{% hint style="info" %}
   [站地址 = Mac ID]

   - DeviceNet通过站地址（MAC ID）识别从站（1-63）。
{% endhint %}

{% hint style="info" %}
   [通讯速度 (波特率)]

   - 您可以选择125、250和500 Kbit/s。
{% endhint %}

{% hint style="info" %}
   [输入字节计数 (输入字节)]

   - 输入字节计数：设置从主站到从站的数据输入大小。
{% endhint %}

{% hint style="info" %}
   [输出字节计数 (输出字节)]

   - 输出字节计数：设置从站到主站的数据输出大小。
{% endhint %}

<br>

**5. 完成设置后，请按照以下程序检查通信状态。**

有关在TP上检查工业通信状态的程序，请参考 ("[**1.4 CIFX PCI通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")。

![[图 1.3.7.4-5 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_5.png>) 

<br>

**6. 完成通信设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块使用输入/输出信号。请参考 ("[**4. 工业通信IO块分配**](../../../4-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error-DeviceNet.md)
#### 1.3.7.5 DeviceNet 错误处理

<br>

请参阅 "[**1.4.1 错误代码**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"。

<br>

**1. DeviceNet 终端电阻**

{% hint style="info" %}
   - 连接 DeviceNet 电缆时，应在终端处添加电阻器。

   - 如果网络扫描功能无法正常工作，请检查终端电阻器。

   - DeviceNet 终端电阻：120 欧姆
{% endhint %}

{% hint style="info" %}
   - 如下图所示，如果 CIFX-50 DN PCI 位于 DeviceNet 终端，请添加终端电阻。
{% endhint %}

![[Figure 1.3.7.5-1 DeviceNet Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_1.png>) 

{% hint style="info" %}
   - 如下图所示，如果 DeviceNet 远程 IO 位于终端，请添加终端电阻或操作 DIP 开关。
{% endhint %}

![[Figure 1.3.7.5-2 DeviceNet Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_2.png>) 

<br>

**2. 通信速度**

{% hint style="info" %}
   - 如果 DeviceNet 主设备和从设备之间的通信速度不同，则网络扫描功能可能无法正常工作。

   - 如果网络扫描功能无法正常工作，请检查通信速度。
{% endhint %}

![[Figure 1.3.7.5-3 DeviceNet Baudrate]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_3.png>) 

<br>

**3. DeviceNet 错误**

{% hint style="info" %}
   - 如果未向 DeviceNet 电缆提供 24V 电源，则会出现以下错误。

   - 请检查 24V 电源供应。
{% endhint %}

![[Figure 1.3.7.5-4 DeviceNet Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_4.png>)
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-DeviceNet-Object.md)
#### 1.3.7.6 DeviceNet 对象


<br>

**1. 对象**


DeviceNet 设备内部由一系列对象组成。每个对象代表设备内部的一个特定组件。

<br>

![[Figure 1.3.7.6-1 DeviceNet 对象]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_1.png>) 


<br>

单独的对象通过类代码区分。

<br>

![[Figure 1.3.7.6-2 DeviceNet 对象]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_2.png>)

<br>

一个对象内部由实例编号和属性 ID 组成。

<br>

DeviceNet 主站可以通过显性消息访问特定从站的对象。

<br>

{% hint style="info" %}
   - EX) Crevis GN-9212 的对象（相应的信息可以在 Crevis 手册中找到。）

   - 读取身份对象的供应商 ID 值（类代码 0x01）

   - 实例 : 1

   - 属性 ID : 1

   - 权限: 获取（仅允许读取）
{% endhint %}


![[Figure 1.3.7.6-3 DeviceNet 对象 Crevis GN-9212]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_3.png>)


<br>

每个对象、实例和属性内部具有不同的访问权限。

<br>

{% hint style="info" %}
   - 访问权限

   - 获取: 读取权限

   - 设置: 写入权限 

   - 属性单个: 一次只能访问一个属性项目。

   - 属性全部: 可以一次访问实例中的所有属性。
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/README.md)
### 1.3.8 CC-Link

本章描述了CC-Link从设备的特性及其设置方法。

<br>

**现场总线概述**

现场总线是一种行业标准，旨在通过单根电缆连接传感器、按钮、电机驱动器和操作接口等设备与PLC（可编程逻辑控制器），并在工厂中进行操作。

现场总线提供智能服务，如对整个网络状态的中央监控和网络的重新配置。

例如，可以为传感器和开关设置详细信息、操作和模式，而不仅仅是简单的开/关。

使用单根电缆可减少布线时间和成本，简化配置，并在维护上提供优势。

此外，与一般通信的非确定性响应特性不同，现场总线保证数据响应速度以满足对时间特性要求严格的工业应用。

![[Figure 1.3.8-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/image_1.png>)

<br>

一个现场总线网络连接一个主设备和多个从设备。
主设备搜索和管理整个网络，并与从设备交换数据。

通常，PLC是主设备，而传感器、按钮、控制器等可以配置为从设备。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md)
#### 1.3.8.1 CC-Link 从站规格

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=3, class='powderblued'>类别</th>
		<th class='powderblued'>规格 (版本 1.11)</th>
		<th class='powderblued'>规格 (版本 2.0)</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td colspan=3>最大输入大小</td>
		<td>48 字节</td>
		<td>368 字节</td>
	</tr>
    <tr>
		<td colspan=3>最大输出大小</td>
		<td>48 字节</td>
		<td>368 字节</td>
	</tr>
    <tr>
		<td rowspan=6>IO 大小</td>
		<td rowspan=2>IO 站</td>
        <td>RY</td>
		<td>4 字节</td>
		<td>不支持</td>
	</tr>
    <tr>
        <td>RX</td>
		<td>4 字节</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td rowspan=4>远程设备</td>
        <td>RY</td>
		<td>16 字节</td>
		<td>112 字节</td>
	</tr>
    <tr>
        <td>RX</td>
		<td>16 字节</td>
		<td>112 字节</td>
	</tr>
    <tr>
        <td>RWw</td>
		<td>32 字节</td>
		<td>256 字节</td>
	</tr>
    <tr>
        <td>RWr</td>
		<td>32 字节</td>
		<td>256 字节</td>
	</tr>
    <tr>
        <td colspan=2, rowspan=2>占用站</td>
        <td>IO 站</td>
		<td>1</td>
		<td> - </td>
	</tr>
    <tr>
        <td>远程设备</td>
		<td>1 ~ 4</td>
		<td>1 ~ 4</td>
	</tr>
    <tr>
        <td colspan=3>扩展周期</td>
		<td>不支持</td>
		<td>1, 2, 4, 8</td>
	</tr>
   <tr>
		<td colspan=3>通信速度</td>
		<td colspan=2>156 kbit/s ~ 10 Mbit/s</td>
	</tr>
</tbody>
</table>
<br>

**CC-Link IO 映射**

<br>

{% hint style="info" %}
   - CC-Link 版本 1
{% endhint %}

<br>

![[图 1.3.8.1-1 CC-Link IO 映射]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
   - CC-Link 版本 2

   - 扩展周期 : 单个
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO 映射]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
   - CC-Link 版本 2

   - 扩展周期 : 双重
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO 映射]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
   - CC-Link 版本 2

   - 扩展周期: 四重
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO 映射]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
   - CC-Link 版本 2

   - 扩展周期 : 八重
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO 映射]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_5.png>)
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/2-Settings-CC-Link-Slave.md)
#### 1.3.8.2 CC-Link从设备设置

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
   - For CC-Link connector connection, please refer to the following.

      ("[**1.2.2 Connector**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. 使用TP选择工业通信固件设置中的CC-Link从设备，并重启机器人控制器。**

![[Figure 1.3.8.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查当前通信协议准备状态。**

![[Figure 1.3.8.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[警告]**: 如果使用Sycon.net设置的配置文件被下载到相应的PCI插槽，TP设置将被忽略。
{% endhint %}

<br>

**3. 点击菜单以进入从设备设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从设备插槽设置 > CC-Link从设备]**

![[Figure 1.3.8.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>) 

![[Figure 1.3.8.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

**4. 每个项目的描述**

{% hint style="info" %}
   [站点地址]

   - CC-Link通过站点地址（1-64）识别从设备。
{% endhint %}

{% hint style="info" %}
   [通信速度（波特率）]

   - 您可以从156、625、2500、5000和10000 Kbit/s中选择。
{% endhint %}

{% hint style="info" %}
   [CC-Link版本]

   - 版本1: 可用IO站，扩展周期不可用

   - 版本2: 不可用IO站，扩展周期可用
{% endhint %}

{% hint style="info" %}
   [占用站点计数]

   - IO站: 占用1

   - 远程设备: 可选择1-4

   - 分配的IO字节区的大小取决于占用的站点数量。
{% endhint %}

{% hint style="info" %}
   [扩展周期]

   - 版本2可用

   - 远程设备: 您可以选择单组（1x）、双组（2x）、四组（4x）和八组（8x）。

   - 分配的IO字节区的大小取决于扩展周期。
{% endhint %}

<br>

{% hint style="info" %}
   **有关IO字节区，请参阅以下链接。**

   **(["**1.3.8.1 CC-Link从设备规格**](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md))**
{% endhint %}

<br>

**5. 完成设置后，请根据以下程序检查通信状态。**

For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

<br>

**6. 完成通信设置后分配IO块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配IO块来使用输入/输出信号。请参阅("[**4. 工业通信IO块分配**](../../../4-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Error-CC-Link.md)
#### 1.3.8.3 CC-Link 从站错误处理

<br>

请参考 "[**1.4.1 错误代码**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"。

<br>

**1. CC-Link 终端电阻**

{% hint style="info" %}
   - 在连接 CC-Link 电缆时，应在终端处添加电阻。

   - 如果通信未连接，请检查终端电阻。

   - CC-Link 终端电阻：110 欧姆
{% endhint %}

{% hint style="info" %}
   - 如下图所示，如果 CIFX-50 CC PCI 在 CC-Link 终端，请添加终端电阻。
{% endhint %}

![[Figure 1.3.8.5-1 CC-Link Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/5-Error/image_1.png>) 



**2. CC-Link 错误**

{% hint style="info" %}
   - CC-Link 电缆需要 24V 电源以进行通信连接。

   - 如果通信未连接，请检查 24V 电源。
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/README.md)
### 1.3.9 CC-Link IE Field

本章描述了 CC-Link IE 现场从设备的特性及其设置方法。

<br>

**现场总线概述**

现场总线是一种行业标准，旨在通过单一电缆将传感器、按钮、电机驱动器和操作界面等设备连接到 PLC（可编程逻辑控制器），并在工厂中进行操作。

现场总线提供智能服务，例如对整个网络状态的集中监控或网络的重新配置。

例如，有可能为传感器和开关设置详细信息、操作和模式，而不仅仅是简单的开/关。

使用单根电缆减少了布线的时间和成本，简化了配置，并在维护方面提供了优势。

此外，与一般通信的非确定性响应特性协议不同，现场总线保证数据响应速度，以满足对时间特性关键的工业应用。

![[Figure 1.3.9-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/image_1.png>)

<br>

一个现场总线网络连接一个主设备和多个从设备。
主设备搜索并管理整个网络，并与从设备交换数据。

通常，PLC 是主设备，而传感器、按钮、控制器等可以配置为从设备。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/1-Specification-CC-Link-IE-Field-Slave.md)
#### 1.3.9.1 CC-Link IE Field Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=2, class='powderblued'>类别</th>
		<th colspan=2, class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td colspan=2>网络编号</td>
		<td colspan=2>1-239</td>
	</tr>
    <tr>
		<td colspan=2>站号</td>
		<td colspan=2>1-120</td>
	</tr>
    <tr>
		<td colspan=2>通信速度</td>
		<td colspan=2>1Gbps</td>
	</tr>
    <tr>
		<td colspan=2>设备类型</td>
		<td>智能设备站</td>
        <td>远程设备站</td>
	</tr>
    <tr>
		<td rowspan=4>IO大小</td>
        <td>RY数据</td>
		<td>4-256字节 (32-2048位)</td>
        <td>4-16字节 (32-128位)</td>
	</tr>
    <tr>
        <td>RX数据</td>
		<td>0 - 256字节 (0 - 2048位)</td>
        <td>0 - 16字节 (0 - 128位)</td>
	</tr>
    <tr>
        <td>RWw数据</td>
		<td>0 - 1024字</td>
        <td>0 - 64字</td>
	</tr>
    <tr>
        <td>RWr数据</td>
		<td>0-1024字</td>
        <td>0-64字</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>1000 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>自协商</td>
		<td>始终开启</td>
	</tr>
    <tr>
		<td>自交叉</td>
		<td>始终开启</td>
	</tr>
</tbody>
</table>
<br>

**连接**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>电缆</td>
		<td>至少Cat6，STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最大100m</td>
	</tr>
	<tr>
		<td>接线</td>
		<td>完全占用的电缆（所有8个电缆核心）</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/2-Settings-CC-Link-IE-Field-Slave.md)
#### 1.3.9.2 CC-Link IE Field Slave Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.


<br>

**1. Using the TP, select a CC-Link IE Field slave in the industrial communication firmware settings and reboot the robot controller.**

![[Figure 1.3.9.2-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_1.png>) 

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.9.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: 如果使用 Sycon.net 配置的文件下载到相应的 PCI 槽，TP 设置将被忽略。
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > CC-Link IE Field Slave]**

![[Figure 1.3.9.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>) 

![[Figure 1.3.9.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
   [Network Number]

   - CC-Link IE field network number (1-239)
{% endhint %}

{% hint style="info" %}
   [Station Address]

   - 连接网络中的设备 ID (1-120)
{% endhint %}

{% hint style="info" %}
   [IO Type]

   - IO 类型由主设备设置决定。   
      - Mixed: 输入和输出使用不同的索引（不同的地址）。   
      - Input: 仅输入   
      - Output: 仅输出   
      - FrontBackMixture: 输入和输出使用相同的索引（相同的地址）。   
{% endhint %}

{% hint style="info" %}
   [Device Type]

   - 可设置的最大 IO 大小因设备类型而异。

   - Intelligent Device Station   
      - RY, RX (max): 256 bytes   
      - RWw, RWr (max): 1024 words

   - Remote Device Station   
      - RY, RX (max): 16 bytes   
      - RWw, RWr (max): 64 words
{% endhint %}

{% hint style="info" %}
   [IO Size]

   - Master -> Slave
      - RWw (字数据)
      - RY (位数据)

   - Slave -> Master   
      - RWr (字数据)   
      - RX (位数据)  
{% endhint %}

<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参阅 ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)")。**
{% endhint %}

<br>

![[Figure 1.3.9.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>)
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/3-Error-CC-Link-IE-Field.md)
#### 1.3.9.3 CC-Link IE Field Slave 错误处理

<br>

请参阅"[**1.4.1 错误代码**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"。
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/README.md)
### 1.3.10 EtherNet/IP - 标准远程 IO 连接

<br>

本章解释如何使用 EtherNet/IP 扫描仪（主设备）连接我们公司选择的多个标准远程 IO 模块。

<br>

{% hint style="info" %}
   - EtherNet/IP 扫描仪（主设备）使用 CIFX-50 实时以太网 PCI。


   - 远程 IO 模块使用 Crevis 的 M9289 EtherNet/IP 网络适配器。
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)
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
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)
#### 1.3.10.2 远程 IO IP 地址设置

这是如何设置 Crevis 的 M9289 EtherNet/IP 网络适配器的 IP 地址。

<br>

{% hint style="info" %}
   - Crevis M9289 远程 IO 的出厂默认 IP 是 192.168.100.99。

   - 如果您不知道远程 IO IP 或需要更改它，请遵循以下步骤。
{% endhint %}

<br>

**1. 使用 LAN 电缆直接连接 PC 和远程 IO。**

![[Figure 1.3.10.2-1 LAN Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

**2. 将远程 IO 适配器的 DIP 开关 9 仅更改为 ON。**

![[Figure 1.3.10.2-2 DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

**3. 执行 Bootpsvr.exe 程序。**
   * 该程序由 Crevis 提供。 （从网站下载并安装 IO Guide Pro。）

![[Figure 1.3.10.2-3 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[Figure 1.3.10.2-4 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
   - 按下“启动 BootP”后，断开并重新施加电源以重启 M9289 模块。
{% endhint %}

![[Figure 1.3.10.2-5 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>

**4. 当适配器设备重启时，设备信息将在 BootpSvr.exe 程序中显示。**

![[Figure 1.3.10.2-6 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

**5. 选择设备并设置 IP。**

![[Figure 1.3.10.2-7 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[Figure 1.3.10.2-8 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

**6. 完成 IP 设置后，将适配器的所有 DIP 开关切换为 OFF 并重启设备。**

{% hint style="info" %}
   - 一定要检查 DIP 开关状态及适配器是否已重启。
{% endhint %}

![[Figure 1.3.10.2-9 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

**7. 在 PC 上使用 ping 测试等验证 IP。**

![[Figure 1.3.10.2-10 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

**8. 如果 IP 地址已成功更改，请继续进行设置。**

{% hint style="info" %}
   - 请根据 "[**1.3.10.1 EtherNet/IP - 标准远程 IO 连接设置**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)" 程序进行设置。
{% endhint %}
[__SOURCE](1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)
## 1.4 CIFX PCI 通信监控

<br>

在按照 "[**1.2 CIFX PCI - 安装和设置工业通信卡**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" 和 "[**1.3 CIFX PCI - 设置工业通信**](../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 的程序设置通信后，您可以在以下屏幕中检查操作。

<br>

**1. 工业通信监控**

<br>

您可以通过触摸 **\[Service > 19: 工业通信监控]** 进入屏幕，并在相关屏幕中检查设置的固件信息、通信状态和通信配置等详细信息。

<br>

{% hint style="info" %}
   - 使用 **\[重启]** 按钮，您可以重启PCI通信卡的工业通信。

   - 请检查插槽、固件和设备的状态。

   - 对于主设备，检查配置和活动从设备的数量是否与配置从设备的数量匹配。
{% endhint %}

<br>

![[Figure 1.4-1 工业通信监控]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_1.png>)

<br>

{% hint style="info" %}
   [状态信息]   
      - 通信：通信链路已建立并且正在交换I/O数据   
      - 运行：通信卡（PCI）正在运行   
      - 准备：通信处于待机状态   
      - 错误：通信错误状态   

      - 通信错误：在通信过程中发生错误代码   
      - 错误计数：积累的通信错误数量   
      - 活动从设备：当前连接并交换I/O数据的从设备数量   
      - 配置从设备：配置用于通信的从设备数量   
      - 诊断从设备：在通信诊断下的从设备数量   
      - 看门狗时间（毫秒）：监控通信程序活动的超时值   
{% endhint %}

<br>

**2. 工业通信节点监控**

<br> 

单击监控屏幕底部的节点状态按钮以监控连接到主协议的设备状态

<br>

![[图 1.4-2 工业通信监控]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_2.png>)

{% hint style="info" %}
   [节点状态信息]   
      - 绿色：节点当前连接并且正在交换I/O数据   
      - 红色：节点已配置但未连接   
{% endhint %}

<br>

{% hint style="info" %}
   - 在DeviceNet主设备的情况下，您可以通过扫描节点信息列表进行监控
{% endhint %}

<br>

![[图 1.4-3 工业通信监控]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_3.png>)
[__SOURCE](1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)
### 1.4.1 错误代码

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>

<br>

<table class="tg">
<thead>
	<tr>
		<th>错误代码</th>
		<th>描述</th>
		<th>操作</th>
	</tr>
</thead>

<tbody>
	<tr>
		<td>0x00000000</td>
		<td>正常</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xC000000C</td>
		<td>控制器和PCI之间的看门狗超时</td>
		<td>请检查控制器和设备的状态。可以通过重新启动通信来重置它们。</td>
	</tr>
    <tr>
		<td>0xC0000123</td>
		<td>无许可证</td>
		<td>请检查您是否拥有主控的许可证。</td>
	</tr>
    <tr>
		<td>0xC0000140</td>
		<td>通信错误</td>
		<td>请检查设备的状态或连接。</td>
	</tr>
    <tr>
		<td>0xC0000141</td>
		<td>连接丢失</td>
		<td>请检查设备的状态或连接。</td>
	</tr>
    <tr>
		<td>0xC0000142</td>
		<td>连接等待超时</td>
		<td>请检查设备的状态或连接。</td>
	</tr>
    <tr>
		<td>0xC0000144</td>
		<td>重复IP地址</td>
		<td>检查连接设备的IP地址并更改重复的地址。</td>
	</tr>
    <tr>
		<td>0xC0000145</td>
		<td>电缆未连接</td>
		<td>请检查通讯电缆的连接状态。</td>
	</tr>
    <tr>
		<td>0xC0000180</td>
		<td>通信总线关闭标志已设置 <br> [可能的原因] <br> - 检测到CAN高/低通信线路短路 <br> - 不稳定的电源电压 <br> - 由于噪声等原因导致的持续网络错误</td>
		<td>检查通信电缆的接触状态或接线，并重置设备。</td>
	</tr>
    <tr>
		<td>0xC0470298</td>
		<td>未提供DeviceNet 24V电源</td>
		<td>请检查DeviceNet 24V电源。</td>
	</tr>
	<tr>
		<td>0xC0620023</td>
		<td>检测到DeviceNet从站总线关闭 <br> [可能的原因] <br>  - 检测到CAN高/低通信线路短路 <br>  - 不稳定的电源电压 <br>  - 由于噪声等原因导致的持续网络错误</td>
		<td>检查通信电缆的接触状态或接线，并重置设备。</td>
	</tr>
    <tr>
		<td>0xC062002C</td>
		<td>未提供DeviceNet 24V电源</td>
		<td>请检查DeviceNet 24V电源。</td>
	</tr>
</tbody>
</table>
[__SOURCE](2-ethernet-ip/README.md)
# 2. EtherNet/IP

本章描述了内置EtherNet/IP主机（扫描仪）和从机（适配器）的特性和配置方法。
<br>

**EtherNet/IP概述**

<br>

EtherNet/IP是由CI（控制网络国际）和ODVA（开放设备网络供应商协会）开发的一种基于以太网的开放工业通信协议。

在工厂环境中，各种设备如传感器、远程I/O、马达驱动器、HMI、PLC和机器人控制器可以与单个EtherNet/IP网络连接，无论厂家如何。

![[Figure 2-1 EtherNet/IP]](<../_assets//2-ethernet-ip/image_1.png>)

<br>

EtherNet/IP根据其通信功能分类如下：

**扫描仪类**

   * 这些产品对应于传统的现场总线主机，可以向EtherNet/IP适配器或扫描仪请求I/O数据连接。

<br>

**适配器类**

  * 这些产品对应于传统的现场总线从机，作为EtherNet/IP扫描仪请求的实时I/O数据的连接目标。

  * 适配器无法在没有扫描仪请求的情况下自主传输或接收实时I/O数据。

<br>

**消息类**

   * 这些产品能够发送和接收来自所有类产品的显式消息，但不支持实时I/O数据传输。

   * 示例包括用于程序上传/下载和网络配置工具的计算机接口卡。

<br>

**缩写**

<br>

|缩写|描述|
|---------------|------------------------------|
|适配器|从EtherNet/IP扫描仪收集输出数据并向其传输输入数据的设备|
|扫描仪|向终端设备（EtherNet/IP适配器）发送输出数据并收集输入数据的设备|
|LAN|局域网|
|RPI|请求数据包间隔|
|PLC|可编程逻辑控制器|
|T2O|目标到发起者（适配器 -> 扫描仪）|
|O2T|发起者到目标（扫描仪 -> 适配器）|
[__SOURCE](2-ethernet-ip/1-network.md)
## 2.1 网络设置

**1. 主模块**

<br>

可以与 EtherNet/IP 适配器连接的 LAN 端口为 LAN1/LAN2/LAN3。

<br>

![figure 2.1-1 Main Module](../_assets/2-ethernet-ip/1-network/hi6com.png)

<br>

**2. 网络设置**

<br>

选择一个 LAN 端口以连接 EtherNet/IP 通信，然后通过 TP 屏幕检查 LAN 端口的设置，如下所示，并根据需要更改设置。

<br>

![figure 2.1-2 Network configuration](../_assets/2-ethernet-ip/1-network/networkConfig.png)

<br>

{% hint style="info" %}
   - LAN1/LAN2/LAN3 每个 IP 地址的子网部分应设置为不同。

   - 更改设置后，请重启机器人控制器。
{% endhint %}

<br>

**3. 连接状态检查**

<br>

可以根据 LAN 端口的 Link/Act LED 状态检查与 EtherNet/IP 扫描仪的物理连接状态。

<br>

使用 LAN 电缆连接 EtherNet/IP 适配器和扫描仪，然后检查 LED 状态。如果左侧的 LED 不亮或不闪烁，则表示电缆或适配器或扫描仪设备存在问题。请检查电缆或设备的连接状态。

<br>

![figure 2.1-3 LAN Port](../_assets/2-ethernet-ip/1-network/lanPort.png)

<br>

**4. 网络配置**

<br>

建议将 EtherNet/IP 网络和工厂网络配置为独立网络。如下面的图所示，如果将 EtherNet/IP 网络和工厂网络配置为一个网络，它们将共享一个传输介质，从而增加网络负载。因此，建议尽可能为 EtherNet/IP 网络使用独立配置的网络。

<br>

![figure 2.1-4 Network](../_assets/2-ethernet-ip/1-network/NG_Network.png)

<br>

![figure 2.1-5 Network](../_assets/2-ethernet-ip/1-network/Good_Network.png)

<br>
[__SOURCE](2-ethernet-ip/2-license.md)
## 2.2 许可证设置

**1. 许可证激活**

<br>

在初始屏幕上，导航到 "系统" > "2: 控制参数" > "10: 选用功能的许可证密钥注册"

<br>

![figure 2.2-1 license](../_assets/2-ethernet-ip/2-license/license.png)

<br>

1. 从许可证列表中选择以太网/IP适配器的 "有效"。
2. 将系统序列号交给许可证管理员
3. 从管理员那里获取许可证密钥，输入并按 "确认" 按钮
4. 许可证密钥 [XXXXXX] ==> 确认
5. 确认当进入以太网/IP适配器菜单时，关于没有许可证的警告信息已消失。<br>

<br>
[__SOURCE](2-ethernet-ip/3-adapter/README.md)
## 2.3 EtherNet/IP 适配器 (从设备)

<br>

本节提供内置 EtherNet/IP 适配器 (从设备) 的概述和说明

<br>
[__SOURCE](2-ethernet-ip/3-adapter/1-specification.md)
### 2.3.1 EtherNet/IP适配器规格 (从站)

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th colspan=2, class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
    <tr>
        <td>连接</td>
        <td>O (主站) -> T (从站)</td>
		<td>T (从站) -> O (主站)</td>
	</tr>
    <tr>
        <td>最大IO大小</td>
        <td>240字节</td>
		<td>240字节</td>
	</tr>
    <tr>
        <td>实例号</td>
        <td>112 (0x70)</td>
		<td>100 (0x64)</td>
	</tr>
    <tr>
        <td>实时传输格式</td>
        <td>32位运行/空闲头部</td>
		<td>无</td>
	</tr>
	<tr>
        <td>连接类型</td>
        <td>点对点</td>
		<td>点对点</td>
	</tr>
	<tr>
        <td>优先级</td>
        <td>计划</td>
		<td>计划</td>
	</tr>
    <tr>
		<td>IO周期时间 (RPI)</td>
		<td colspan=2>最小 5ms</td>
	</tr>
    <tr>
		<td>设备类型</td>
		<td colspan=2>通用离散I/O</td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td colspan=2>10或100 Mbit/s</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td colspan=2>不支持</td>
	</tr>
    <tr>
		<td >IP分配方法</td>
		<td colspan=2>静态IP地址</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>以太网 II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>10或100 BASE-T以太网</td>
	</tr>
    <tr>
		<td>自协商</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>集线器</td>
		<td>允许</td>
	</tr>
    <tr>
		<td>交换机</td>
		<td>允许</td>
	</tr>
</tbody>
</table>
<br>

**连接**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>电缆</td>
		<td>最低Cat5, STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最大100m</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](2-ethernet-ip/3-adapter/2-settings.md)
### 2.3.2 EtherNet/IP 适配器 (从属) 设置

<br>

**1. EtherNet/IP 适配器设置和通过教学挂件监控**

<br>

在初始屏幕上，导航到 "SYSTEM" > "Control Parameter" > "Industrial Communication" > "Ethernet/IP Setting"<br>

<br>

![Config.PNG](../../_assets/2-ethernet-ip/3-adapter/Config.png)<br>

<br>

**[网络]**

- 协议 : 选择是否使用 EtherNet/IP 适配器。
- 端口 : 选择要连接到 EtherNet/IP 扫描仪的 LAN 端口。 (所选 LAN 端口的信息会立即显示在该行。)

<br>

**[I/O 大小]**

- 输入字节计数: 可设置为 0-240。
- 输出字节计数: 可设置为 0-240。

<br>

{% hint style="info" %}
   [状态信息]   
      - 通信: 通信链接已建立并正在交换 I/O 数据   
      - 运行: 通信卡 (PCI) 正在运行   
      - 就绪: 通信处于待机状态   
      - 错误: 通信错误状态   

{% endhint %}
[__SOURCE](2-ethernet-ip/3-adapter/3-connect-scanner/README.md)
### 2.3.3 连接外部扫描仪设备

<br>

本节解释如何将外部 EtherNet/IP 扫描仪连接到 EtherNet/IP 适配器。
[__SOURCE](2-ethernet-ip/3-adapter/3-connect-scanner/1-connect-ls-plc.md)
#### 2.3.3.1 LS ELECTRIC PLC

<br>

本节解释如何将 LS ELECTRIC PLC 与 EtherNet/IP 连接。  
以下是使用的 PLC 和通讯模块。  
(PLC: XGI-CPUS, 通信模块: XGL-EFMTB)

<br>

**1. XG5000 运行**

<br>

![xg5000.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/xg5000.png)

<br>

有关下载 XG5000 程序和详细使用方法，请参考 LS ELECTRIC 网站。

<br>

**2. EDS 文件注册**

<br>

点击菜单 > 工具 > EDS(D) > EDS 文件注册，然后选择 "Hi6_EIP_240402.eds."  
确认如下面图所示的 EDS 文件注册。

<br>

![eds.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/eds.png)

<br>

**3. 设备连接**

<br>

[1] 创建项目。<br>
![newProject_1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_1.png)<br>

[2] 添加通讯模块。<br>
![newProject_2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_2.png)<br>

![newProject_3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_3.png)<br>

![newProject_4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_4.png)<br>

<br>

[3] 设置通讯模块 <br>
双击下图左侧选项卡中的 XGL-EFMT。<br>
![newProject_6.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_6.png)

<br>

- 设置 IP 地址、子网掩码、网关等。  
- 要将 PLC 的两个 LAN 端口用作继电器功能，请选择 "Relay" 复选框。  
- 将 RAPIEnet 设置更改为禁用。

<br>

**4. 在线连接设置**

<br>

[1] 使用 USB 数据线连接 PLC。<br>
![newProject_7.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_7.png)<br>

[2] 按照下图左侧所示的按钮下载所有设置。<br>
![newProject_8.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_8.png)<br>

<br>

**5. 自动扫描**

<br>

[1] 连接到 PLC 后，自动扫描是可能的。<br>
如果当前状态不是在线，请点击菜单 > 在线 > 连接以更改为在线状态。<br>

[2] 右键单击 XGL-EFMT > 添加项目 > 智能扩展<br>
![auto1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto1.png)<br>

[3] 点击下一步。 <br>
![auto2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto2.png)<br>

[4] 点击自动扫描。 <br>
![auto3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto3.png)<br>

![auto4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto4.png)<br>

[5] 检查自动扫描到的设备。  
![auto5.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto5.png)<br>

![auto6.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto6.png)<br>

Hi6 EtherNet/IP 适配器设备出现在下图所示的列表中。 <br>
![auto7.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto7.png)<br>

<br>

**6. 程序变量注册**

<br>

[1] 扫描程序 > NewProgram > 本地变量 (双击)<br>
![variable1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/variable1.png)<br>

[2] 设置要在通信中使用的输入/输出数据。<br>
![variable2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/variable2.png)<br>

<br>

**7. EtherNet/IP 适配器设置**

<br>

[1] 在左侧列表中双击 EB01 (Hi6 EtherNet/IP 适配器)。<br>

[2] 按下 EIP 详细设置按钮。<br>
![AdapterSetting1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting1.png)<br>

[3] 请参考下图选择 EtherNet/IP 适配器的设置值。 <br>
- 连接类型
- T2O RPI 范围，O2T RPI 范围
- T2O 输入，O2T 输出大小
- 传输周期
- 超时
- 本地标签，远程标签 <br>
![AdapterSetting2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting2.png) <br>

[4] 点击在线 > 通讯模块设置和诊断 > 服务启用。<br>
![AdapterSetting3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting3.png)<br>

[5] 勾选 FEnet I/O 服务复选框。<br>
![AdapterSetting4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting4.png)<br>

<br>

**8. 通信设置完成后的 IO 块分配**

<br>

{% hint style="info" %}
   **完成通信设置后，可以通过分配 IO 块来使用输入/输出信号。请参阅 ("[**4. 工业通信 IO 块分配**](../../4-io-block-allocation.md)")。**
{% endhint %}
[__SOURCE](2-ethernet-ip/3-adapter/4-error_code.md)
### 2.3.4 错误代码

|代码|信息|
|------|---|
|W23101|EtherNet/IP 初始化失败|
|W23102|EtherNet/IP 通信超时发生|
|W23103|EIP 适配器 CPF O2T 初始化失败|
|W23104|EIP 适配器 CPF T2O 初始化失败|
|W23105|EIP 适配器 IO MSG O2T 初始化失败|
|W23106|EIP 适配器 IO MSG T2O 初始化失败|
|W23107|EIP 适配器 PIT 初始化失败|
|W23108|EIP 适配器套接字通信初始化失败|
|W23109|EIP 适配器套接字通信 (UDP 0) 初始化失败|
|W23110|EIP 适配器套接字通信 (UDP 1) 初始化失败|
|W23111|EIP 适配器套接字通信 (UDP 2) 初始化失败|
|W23112|EIP 适配器套接字通信 (UDP 3) 初始化失败|
|W23113|EIP 适配器套接字通信 (TCP 0) 初始化失败|
|W23114|EIP 适配器套接字通信 (TCP 1) 初始化失败|
|W23115|EIP 适配器套接字通信 (TCP 2) 初始化失败|
|W23116|EIP 适配器套接字通信 (TCP 3) 初始化失败|
|W23117|EIP 适配器内部通信1 (IO 写入) 问题|
|W23118|EIP 适配器内部通信1 (IO 读取) 问题|
|W23119|EIP 适配器内部通信1 (状态写入) 问题|
|W23120|EIP 适配器内部通信1 (配置读取) 问题|
|W23150|EIP 适配器内部通信2 (IO 读取) 问题|
|W23151|EIP 适配器内部通信2 (IO 写入) 问题|
|W23152|EIP 适配器内部通信2 (状态读取) 问题|
|W23153|EIP 适配器内部通信2 (配置写入) 问题|
[__SOURCE](2-ethernet-ip/4-scanner/README.md)
## 2.4 EtherNet/IP 扫描器 (主)

<br>

本节提供内置 EtherNet/IP 扫描器 (主) 的概述和说明

<br>
[__SOURCE](2-ethernet-ip/4-scanner/1-specification.md)
### 2.4.1 EtherNet/IP Scanner (Master) 规格

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=2, class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td colspan=2>最大可连接从机数量</td>
		<td>20</td>
	</tr>
    <tr>
		<td rowspan=2>IO 大小</td>
        <td>最大 I/O 大小</td>
		<td>最大 1200 字节</td>
	</tr>
    <tr>
        <td>最大 I/O 大小（1 个从机）</td>
		<td>最大 240 字节</td>
	</tr>
    <tr>
		<td colspan=2>IO 连接</td>
		<td>循环</td>
	</tr>
    <tr>
		<td colspan=2>IO 更新时延</td>
		<td>最小 5ms</td>
	</tr>
    <tr>
		<td colspan=2>通信速度</td>
		<td>10 或 100 Mbit/s</td>
	</tr>
    <tr>
		<td colspan=2>快速连接</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td colspan=2>拓扑结构</td>
		<td>树形，线性</td>
	</tr>
    <tr>
		<td colspan=2>IP 分配方法</td>
		<td>静态 IP 地址</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>10 或 100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>自动协商</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>集线器</td>
		<td>允许</td>
	</tr>
    <tr>
		<td>交换机</td>
		<td>允许</td>
	</tr>
</tbody>
</table>
<br>

**连接**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>电缆</td>
		<td>最小 Cat5，STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最大 100m</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](2-ethernet-ip/4-scanner/2-settings.md)
### 2.4.2 EtherNet/IP 扫描仪 (主设备) 设置

<br>

在完成 "[**2.1 网络设置**](../../2-ethernet-ip/1-network.md)" 和 "[**2.2 许可设置**](../../2-ethernet-ip/2-license.md)" 中的程序后，请继续进行以下步骤。

<br>

**1. 触摸菜单以进入设置屏幕。**

<br>

**\[系统 > 2: 控制参数 > 11: 工业通信 > 3: EtherNet/IP 设置]**

<br>

![[figure 2.4.2-1 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_1.png>) 

<br>

![[figure 2.4.2-2 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_2.png>) 

<br>

{% hint style="info" %}
   [协议设置]

      - 关闭 : 禁用 EtherNet/IP   
      - 适配器 : EtherNet/IP 适配器模式   
      - 扫描仪 : EtherNet/IP 扫描仪模式   
      - 适配器 + 扫描仪 : EtherNet/IP 适配器 + 扫描仪模式（使用同一局域网端口）
{% endhint %}

{% hint style="info" %}
   [端口设置]

      - 通用控制器 LAN1 到 LAN3 可用（确保状态为“OK”）
{% endhint %}

<br>

**2. 选择“扫描仪”模式并点击“添加设备”按钮以继续到下一个屏幕。**

<br>

![[figure 2.4.2-3 Scanner Add Device]](<../../_assets/2-ethernet-ip/4-scanner/img_3.png>) 

<br>

**3. 输入设置以匹配目标设备并保存。**

<br>

{% hint style="info" %}
   [设备设置]

      - 设备编号 : 设备连接顺序（I/O 数据分配顺序）   
      - IP 地址 : 设备的 IP 地址   
      - 设备名称 : 设备名称（仅用于识别；不影响通信）   
      - RPI (毫秒) : 请求的数据包间隔 (I/O 数据更新周期)   
      - 连接类型   
            - 独占所有者 (I/O) : 在扫描仪和适配器之间建立双向 I/O 连接   
            - 仅输入 : 仅连接到适配器的输入信号   
            - 仅监听 : 在适配器已经连接到另一台扫描仪时，仅连接到输入信号   

      - 输入 (T > O) : 从设备 > 主设备连接   
      - 输出 (O > T) : 主设备 > 从设备连接   

      - 运行/空闲头 : 选择是否包括 I/O 数据头   
      - 实例编号 : I/O 数据交换的输入/输出组实例编号   
      - I/O 大小 : I/O 数据大小（以字节为单位）   
{% endhint %}

<br>

{% hint style="info" %}
   - 有关连接示例，请参阅以下手册。    
   - "[**2.3.3.1 连接外部适配器设备 - Crevis 远程 IO**](3-connect-adapter/1-crevis.md)"

   - "[**2.3.3.2 连接外部适配器设备 - Wago 远程 IO**](3-connect-adapter/2-wago.md)"

   - "[**2.3.3.3 连接外部适配器设备 - Hilscher CIFX PCI EtherNet/IP 适配器**](3-connect-adapter/3-pci.md)"

   - "[**2.3.3.4 连接外部适配器设备 - Baumer OM-70**](3-connect-adapter/4-baumer.md)"  
{% endhint %}

<br>

![[figure 2.4.2-4 Scanner Add Device]](<../../_assets/2-ethernet-ip/4-scanner/img_4.png>) 

<br>

**4. 点击“确定”按钮以传输通信设置。**

<br>

![[figure 2.4.2-5 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_5.png>) 

<br>

**5. 检查状态以验证通信是否成功建立。**

<br>

![[figure 2.4.2-6 Communication Status]](<../../_assets/2-ethernet-ip/4-scanner/img_6.png>) 

<br>

{% hint style="info" %}
   [通信状态检查]   
      - 许可: 当前许可状态   
      - 运行: 指示 EtherNet/IP 功能的操作状态   
      - 通信: 指示 EtherNet/IP 连接状态   
      - 错误: 指示 EtherNet/IP 错误状态   

   - 设备编号颜色   
      - 绿色: 通信连接 OK   
      - 红色: 通信连接 NG (失败)   
{% endhint %}

<br>

![[figure 2.4.2-7 Communication Status]](<../../_assets/2-ethernet-ip/4-scanner/img_7.png>) 

<br>

**6. 完成通信设置后，分配 I/O 块。**

{% hint style="info" %}
   **完成通信设置后，可以通过分配 I/O 块使用输入/输出信号。请参阅 ("[**4. 工业通信 IO 块分配**](../../5-io-block-allocation.md)")**
{% endhint %}
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/README.md)
### 2.4.3 连接外部适配器设备

<br>

<style type="text/css">
table  {border-collapse:collapse;}
.sm-font-table th, .sm-font-table td {font-size:9px;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**连接外部适配器设备的配置值**

<br>

{% hint style="info" %}
   - 请将IO大小设置为与外部设备上配置的输入/输出大小匹配。   
{% endhint %}

<br>

{% hint style="info" %}
   - 有关详细规格，请参考设备制造商提供的手册    
{% endhint %}

<br>

<table class="tg sm-font-table">
<thead>
	<tr>
    	<th rowspan=2, class='powderblued'>制造商</th>
		<th rowspan=2, class='powderblued'>产品</th>
		<th rowspan=2, class='powderblued'>连接类型</th>
        <th colspan=2, class='powderblued'>T -> O</th>
        <th colspan=2, class='powderblued'>O -> T</th>
        <th colspan=5, class='powderblued'>附加配置</th>
	</tr>
    <tr>
        <th class='powderblued'>实例ID</th>
        <th class='powderblued'>运行空闲头</th>
        <th class='powderblued'>实例ID</th>
        <th class='powderblued'>运行空闲头</th>
		<th class='powderblued'>实例ID</th>
        <th class='powderblued'>总大小</th>
		<th class='powderblued'>数据大小</th>
        <th class='powderblued'>数据类型</th>
		<th class='powderblued'>数据</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Crevis</td>
		<td>M9289</td>
        <td>独占拥有者</td>
		<td>1</td>
		<td>否</td>
        <td>2</td>
		<td>是</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Wago</td>
		<td>750-366</td>
        <td>独占拥有者</td>
		<td>104: 状态 + AI + DI<br>105: 状态 + DI<br>106: 状态 + AI<br>107: AI + DI<br>108: DI<br>109: AI</td>
		<td>否</td>
        <td>101: AO + DO<br>102: DO<br>103: AO</td>
		<td>是</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Hilscher</td>
		<td>CIFX PCI EtherNet/IP适配器</td>
        <td>独占拥有者</td>
		<td>101</td>
		<td>是</td>
        <td>100</td>
		<td>是</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Baumer</td>
		<td>OM-70 EtherNet/IP</td>
        <td>仅输入</td>
		<td>100</td>
		<td>否</td>
        <td>238</td>
		<td>-</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Beckhoff</td>
		<td>EK-9500</td>
        <td>独占拥有者</td>
		<td>129</td>
		<td>否</td>
        <td>130</td>
		<td>是</td>
		<td colspan=5>-</td>
	</tr>
	<tr>
		<td rowspan=6>Rockwell Automation (AB)</td>
		<td rowspan=6>Point I/O 1734-AENTR</td>
        <td rowspan=6>独占拥有者</td>
		<td rowspan=6>101</td>
		<td rowspan=6>否</td>
        <td rowspan=6>100</td>
		<td rowspan=6>是</td>
		<td rowspan=6>102</td>
		<td rowspan=6>10</td>
		<td>4byte</td>
		<td>无符号 int</td>
		<td>1</td>
	</tr>
	<tr>
		<td>2byte</td>
		<td>无符号 int</td>
		<td>IO插槽 + 1</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>无符号 int</td>
		<td>(T -> O) 对齐<br>0: 字节<br>2: 字<br>4: 双字<br>255: 固定</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>无符号 int</td>
		<td>(T -> O) 每个插槽的固定大小</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>无符号 int</td>
		<td>(O -> T) 对齐<br>0: 字节<br>2: 字<br>4: 双字<br>255: 固定</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>无符号 int</td>
		<td>(O -> T) 每个插槽的固定大小</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis.md)
#### 2.4.3.1 连接外部适配器设备 - Crevis Remote IO

<br>

{% hint style="info" %}
   - 您可以使用 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置。 

   - "[**下载 EDS 文件工具 (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 有关示例中使用的远程 I/O 的 IP 设置，请参考以下手册链接。 

   - "[**1.3.10.2 远程 IO IP 设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

**1. 准备适配器设备的手册和 EDS 文件。**

![[figure 2.4.3.1-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_1.png>) 

<br>

![[figure 2.4.3.1-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_2.png>) 

<br>

![[figure 2.4.3.1-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_3.png>) 

<br>

**2. 使用 EZ-EDS 程序打开 EDS 文件并验证设备信息。**

<br>

![[figure 2.4.3.1-4 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_4.png>) 

<br>

{% hint style="info" %}
   - 检查连接管理器中的连接类型   
      - 示例：独占所有者 

   - 检查实时传输格式中标题的存在   
      - 输入 (T > O) : 无标题   
      - 输出 (O > T) : 32 位运行/空闲标题   

   - 单击“创建 / 解码路径”以验证实例 ID   
{% endhint %}

<br>

![[figure 2.4.3.1-5 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_5.png>) 

<br>

{% hint style="info" %}
      - 输入 (T > O) : 1   
      - 输出 (O > T) : 2   
{% endhint %}

<br>

**3. 查看设备手册中的 I/O 大小。**

<br>

{% hint style="info" %}
   - 验证要连接的设备的 I/O 配置。 
{% endhint %}

<br>

![[figure 2.4.3.1-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_6.png>) 

<br>

{% hint style="info" %}
   - 请参阅手册中各个插槽配置，以确定总 I/O 大小。
{% endhint %}

<br>

![[figure 2.4.3.1-7 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_7.png>) 

<br>

![[图 2.4.3.1-8 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_8.png>) 

<br>

**4. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.1-8 EtherNet/IP 设置]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_9.png>)

<br>

{% hint style="info" %}
   - 请参考目标设备的手册以正确输入设置。   
      - 输入 (T > O) : 从属 > 主控   
      - 输出 (O > T) : 主控 > 从属   

   [适配器配置]   
   - Crevis M9289   
      - M7002 : 无   
      - M2768 : 1 字节 (O > T)   
      - M2768 : 1 字节 (O > T)   
      - M12DF : 2 字节 (T > O)   
      - M12DF : 2 字节 (T > O)   
      - M2768 : 1 字节 (O > T)   
      - M2768 : 1 字节 (O > T)   

   [IO 装配信息]   
   [T > O]   
      - 大小：4 字节   
      - 实例：1   
      - 运行/空闲标题：无   

   [O > T]    
      - 大小：4 字节   
      - 实例：2   
      - 运行/空闲标题：32 位   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/2-wago.md)
#### 2.4.3.2 连接外部适配器设备 - Wago Remote IO

<br>

{% hint style="info" %}
   - 您可以使用 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置信息。

   - "[**下载 EDS 文件工具 (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 请查阅 Wago 手册以获取设备的 IP 配置。
{% endhint %}

<br>

**1. 准备适配器设备的手册和 EDS 文件。**

![[figure 2.4.3.2-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_1.png>) 

<br>

**2. 检查设备手册中提供的实例 ID**

<br>

![[figure 2.4.3.2-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_2.png>) 

<br>

{% hint style="info" %}
   - 输入 (T > O)   
      - 104: 状态  + 模拟  + 数字   
      - 105: 状态  + 数字   
      - 106: 状态  + 模拟   
      - 107: 模拟  + 数字   
      - 108: 数字   
      - 109: 模拟   

   - 输出 (O > T)   
      - 101: 模拟 + 数字   
      - 102: 数字   
      - 103: 模拟   
{% endhint %}

<br>

**3. 使用 EZ-EDS 程序打开 EDS 文件并验证设备信息。**

<br>

![[figure 2.4.3.2-3 EDS 信息](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_3.png>) 

<br>

{% hint style="info" %}
   - 在连接管理器中检查连接类型   
      - 示例：独占所有者

   - 检查实时传输格式中头的存在   
      - 输入 (T > O) : 无头   
      - 输出 (O > T) : 32 位运行/空闲头   
{% endhint %}

<br>

**4. 检查设备手册中的 I/O 大小。**

<br>

{% hint style="info" %}
   - 验证要连接的设备的 I/O 配置。 
{% endhint %}

<br>

![[figure 2.4.3.2-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_4.png>) 

<br>

{% hint style="info" %}
   - 请查阅每个槽位的手册以确定总 I/O 大小。
{% endhint %}

<br>

![[figure 2.4.3.2-5 I/O 大小]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_5.png>) 

<br>

![[figure 2.4.3.2-6 I/O 大小]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_6.png>) 

<br>

**5. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.2-7 EtherNet/IP 设置]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_7.png>)

<br>

{% hint style="info" %}
   - 请参考目标设备的手册以正确输入设置。   
      - 输入 (T > O) : 从属 > 主   
      - 输出 (O > T) : 主 > 从   

   [适配器配置]   
   - Wago 750-366   
      - 状态 1byte (T > O) (选择实例 ID 104, 105, 106 时)   
      - 753-436 : 1byte (T > O)   
      - 753-536 : 1byte (O > T)   

   [IO 部件信息]   
   [T > O]   
      - 大小: 2bytes   
      - 实例: 105   
      - 运行/空闲头: 无   

   [O > T]    
      - 大小: 1bytes   
      - 实例: 101   
      - 运行/空闲头: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/3-pci.md)
#### 2.4.3.3 连接外部适配器设备 - Hilscher CIFX PCI EtherNet/IP 适配器

<br>

{% hint style="info" %}
   - 您可以使用 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置信息。

   - "[**下载 EDS 文件工具 (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 请参考 Hilscher 手册获取设备的 IP 配置。
{% endhint %}

<br>

**1. 准备适配器设备的手册和 EDS 文件。**

![[figure 2.4.3.3-1 CIFX PCI]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_1.png>) 

<br>

**2. 使用 EZ-EDS 程序打开 EDS 文件并验证设备信息。**

<br>

![[figure 2.4.3.3-2 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_2.png>) 

<br>

{% hint style="info" %}
   - 检查连接管理器中的连接类型   
      - 示例: 独占所有者

   - 检查实时传输格式中标题的存在   
      - 输入 (T > O) : 32-bit 运行/待机头   
      - 输出 (O > T) : 32-bit 运行/待机头   
{% endhint %}

<br>

![[figure 2.4.3.3-3 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_3.png>) 

<br>

{% hint style="info" %}
   - 检查参数中的实例 ID   
      - 输入 (T > O) : 101   
      - 输出 (O > T) : 100   
{% endhint %}

<br>

**3. 检查设备手册中的 I/O 大小。**

<br>

{% hint style="info" %}
   - 检查当前要连接的设备的 I/O 大小（参考相应的 PCI 设备设置）   
{% endhint %}

<br>

**4. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.3-4 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_4.png>)

<br>

{% hint style="info" %}
   - 请参考目标设备的手册以正确输入设置。   
      - 输入 (T > O) : 从属 > 主   
      - 输出 (O > T) : 主 > 从   

   [IO 装配信息]   
   [T > O]   
      - 大小: 240 字节（在 PCI 设备中配置的值）   
      - 实例: 101   
      - 运行/待机头: 32Bit   

   [O > T]    
      - 大小: 240 字节（在 PCI 设备中配置的值）   
      - 实例: 100   
      - 运行/待机头: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer.md)
#### 2.4.3.4 连接外部适配器设备 - Baumer OM-70

<br>

{% hint style="info" %}
   - 您可以使用 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置信息。

   - "[**下载 EDS 文件工具 (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 请参考 Baumer 手册获取设备的 IP 配置。
{% endhint %}

<br>

**1. 准备适配器设备的手册和 EDS 文件。**

![[figure 2.4.3.4-1 Baumer OM-70]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_1.png>) 

<br>

**2. 验证设备手册中的实例 ID 和 I/O 大小。**

<br>

![[figure 2.4.3.4-2 Baumer OM-70]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_2.png>) 

<br>

{% hint style="info" %}
   [仅输入连接]   

   - 输入 (T > O)   
      - 实例 ID: 100   
      - 大小: 34 字节   

   - 输出 (O > T)   
      - 实例 ID: 238   
      - 大小: 0 字节    
{% endhint %}

<br>

**3. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.4-3 EtherNet/IP 设置]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_3.png>) 

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff.md)
#### 2.4.3.5 连接外部适配器设备 - Beckhoff Remote IO

<br>

{% hint style="info" %}
   - 您可以使用 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置文件信息。

   - "[**下载 EDS 文件工具 (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 请参阅 Beckhoff 手册以获取设备的 IP 配置。
{% endhint %}

<br>

**1. 准备适配器设备的手册和 EDS 文件。**

![[figure 2.4.3.5-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_1.png>) 

<br>

**2. 访问设备的网页以配置 IP 地址。**

<br>

{% hint style="info" %}
   - 在此示例中，初始 IP 地址设置为 192.168.1.2 (DIP 开关 No. 2 是 ON)
{% endhint %}

<br>

![[figure 2.4.3.5-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_2.png>) 

<br>

![[figure 2.4.3.5-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_3.png>) 

<br>

{% hint style="info" %}
   - 在此示例中，IP 地址更改为 192.168.10.95。

   - 输入 IP 地址后，单击检查按钮以保存。
{% endhint %}

<br>

![[figure 2.4.3.5-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_4.png>) 

<br>

{% hint style="info" %}
   - 按照以下方式设置 DIP 开关并重新启动设备：   
      - 1 ~ 8  : ON   
      - 9 ~ 10 : OFF   
{% endhint %}

<br>

![[figure 2.4.3.5-5 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_5.png>) 

<br>

![[figure 2.4.3.5-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_6.png>) 

<br>

**3. 访问设备的网页以验证 EtherNet/IP 配置信息。**

<br>

{% hint style="info" %}
   - 使用新配置的 IP 地址重新访问网页，并验证 IP 地址和 EtherNet/IP 配置详细信息。
{% endhint %}

<br>

![[figure 2.4.3.5-7 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_7.png>) 

<br>

![[figure 2.4.3.5-8 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_8.png>) 

<br>

{% hint style="info" %}
   - 输入 (T > O)   
      - 实例 ID: 129   
      - 字节大小: 6      

   - 输出 (O > T)   
      - 实例 ID: 130   
      - 字节大小: 6   
{% endhint %}

<br>

**4. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.5-9 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_9.png>)

<br>

{% hint style="info" %}
   - 请参阅目标设备的手册以正确输入设置。   
      - 输入 (T > O) : 从属设备 > 主设备    
      - 输出 (O > T) : 主设备 > 从属设备   

   [适配器配置]   
   - Beckhoff EK-9500   
      - EK-1008 : 1byte (T > O)   
      - EK-2008 : 1byte (O > T)   

   [IO 组件信息]   
   [T > O]   
      - 大小: 6bytes   
      - 实例: 129   
      - 运行/空闲头: 不   

   [O > T]    
      - 大小: 6bytes   
      - 实例: 130   
      - 运行/空闲头: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell.md)
#### 2.4.3.6 连接外部适配器设备 - Rockwell Automation (AB) 远程 IO

<br>

{% hint style="info" %}
   - 您可以使用 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置信息。

   - "[**下载 EDS 文件工具 (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 请参考 Rockwell Automation 手册以获取设备的 IP 配置。
{% endhint %}

<br>

**1. 准备适配器设备的手册和 EDS 文件。**

<br>

![[figure 2.4.3.6-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_1.png>) 

<br>

![[figure 2.4.3.6-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_2.png>) 

<br>

**2. 使用 EZ-EDS 程序打开 EDS 文件并验证设备信息。**

<br>

![[figure 2.4.3.6-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_3.png>) 

<br>

![[figure 2.4.3.6-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_4.png>) 

<br>

{% hint style="info" %}
   - 检查连接类型在连接管理器中   
      - 示例：独占所有者

   - 检查实时传输格式中是否存在标题   
      - 输入 (T > O) : 无标题   
      - 输出 (O > T) : 32 位运行/闲置标题   

   - 单击“创建 / 解码路径”以验证实例 ID   
      - 输入 (T > O) : 101   
      - 输出 (O > T) : 100   
      - 配置 : 102   
{% endhint %}

<br>

**3. 检查设备手册中的 I/O 大小。**

<br>

{% hint style="info" %}
   - 验证要连接的设备的 I/O 配置。 
{% endhint %}

<br>

![[figure 2.4.3.6-5 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_5.png>) 

<br>

{% hint style="info" %}
   - 验证要连接的设备的 I/O 配置。 
{% endhint %}

<br>

![[figure 2.4.3.6-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_6.png>) 

<br>

![[figure 2.4.3.6-7 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_7.png>) 

<br>

**4. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.6-8 EtherNet/IP 设置]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_8.png>)

<br>

{% hint style="info" %}
   - 请参考目标设备的手册以正确输入设置。   
      - 输入 (T > O) : 从属 > 主设备    
      - 输出 (O > T) : 主设备 > 从属    

   [适配器配置]   
   - 点 I/O 1734-AENTR    
      - 状态 : 8byte (T > O)    
      - 1734-IB8 : 1byte (T > O)   
      - 1734-OB8E : 1byte (O > T) + 1byte (T > O, 状态)   

   [IO 装配信息]   
   [T > O]   
      - 大小: 10bytes   
      - 实例: 101   
      - 运行/闲置标题: 无   

   [O > T]    
      - 大小: 1byte   
      - 实例: 100   
      - 运行/闲置标题: 32 位   
{% endhint %}

<br>

![[figure 2.4.3.6-9 EtherNet/IP 设置]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_9.png>)

<br>

{% hint style="info" %}
   - 请参考目标设备的手册以正确输入额外设置。   
      - 输入 (T > O) : 从属 > 主设备   
      - 输出 (O > T) : 主设备 > 从属   

   [额外设置]   
      - 配置段 : 开   
      - 实例: 102   
      - 大小: 10bytes    

   [配置段信息]    
      - (4bytes) 1 : 标头    
      - (2bytes) 3 : 连接插槽 + 1   
      - (1byte)  0 : T > O 对齐 (以字节为单位)      
      - (1byte)  1 : T > O 每个插槽的数据大小      
      - (1byte)  0 : O > T 对齐 (以字节为单位)      
      - (1byte)  1 : O > T 每个插槽的数据大小      
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/4-error.md)
### 2.4.4 错误代码

<br>

{% hint style="info" %}
   - 通过使用CIP标准的一般状态代码显示每个设备的通信状态，提供实时诊断功能。
{% endhint %}

<br>

![[figure 2.4.4-1 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_8.png>) 

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**一般状态代码**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>状态值 (十六进制)</th>
		<th class='powderblued'>名称</th>
		<th class='powderblued'>描述</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>-</td>
		<td>通信未配置或已更改</td>
		<td>通信设置尚未应用或正在更改中</td>
	</tr>
	<tr>
		<td>0x00</td>
		<td>成功</td>
		<td>指定的对象已成功执行服务。</td>
	</tr>
	<tr>
		<td>0x00 (在错误情况下)</td>
		<td>无响应</td>
		<td>无通信响应（例如，电缆断开，无效的IP地址等）</td>
	</tr>
	<tr>
		<td>0x01</td>
		<td>连接失败</td>
		<td>连接相关服务失败。这发生在连接路径的任意位置。</td>
	</tr>
	<tr>
		<td>0x02</td>
		<td>资源不可用</td>
		<td>执行请求服务所需的某些资源不可用。</td>
	</tr>
	<tr>
		<td>0x03</td>
		<td>无效的参数值</td>
		<td>请参阅状态代码0x20，通常在这种情况下应用。</td>
	</tr>
	<tr>
		<td>0x04</td>
		<td>路径段错误</td>
		<td>遇到路径段错误。提供的路径信息评估失败。</td>
	</tr>
	<tr>
		<td>0x05</td>
		<td>路径目标未知</td>
		<td>路径引用未知的对象类、实例或结构元素，导致路径处理中止。</td>
	</tr>
	<tr>
		<td>0x06</td>
		<td>部分传输</td>
		<td>只能传输预期数据的一部分。</td>
	</tr>
	<tr>
		<td>0x07</td>
		<td>连接丢失</td>
		<td>消息传递的连接已丢失。</td>
	</tr>
	<tr>
		<td>0x08</td>
		<td>服务不支持</td>
		<td>请求的服务尚未为该对象类或实例实现或未定义</td>
	</tr>
	<tr>
		<td>0x09</td>
		<td>无效的属性值</td>
		<td>检测到无效的属性数据</td>
	</tr>
	<tr>
		<td>0x0A</td>
		<td>属性列表错误</td>
		<td>Get_Attribute_List或Set_Attribute_List响应中的某个属性的状态不等于0。</td>
	</tr>
	<tr>
		<td>0x0B</td>
		<td>已经处于请求状态</td>
		<td>对象已经处于服务所请求的模式或状态</td>
	</tr>
	<tr>
		<td>0x0C</td>
		<td>对象状态冲突</td>
		<td>对象无法在当前模式或状态下执行请求的服务</td>
	</tr>
	<tr>
		<td>0x0D</td>
		<td>对象已存在</td>
		<td>尝试创建已经存在的对象实例。</td>
	</tr>
	<tr>
		<td>0x0E</td>
		<td>属性不可设置</td>
		<td>尝试更改不可修改的属性。</td>
	</tr>
	<tr>
		<td>0x0F</td>
		<td>权限冲突</td>
		<td>权限或特权检查失败</td>
	</tr>
	<tr>
		<td>0x10</td>
		<td>设备状态冲突</td>
		<td>设备的当前模式或状态阻止执行请求的服务。</td>
	</tr>
	<tr>
		<td>0x11</td>
		<td>回复数据太大</td>
		<td>响应缓冲区中要传输的数据所需的空间超过分配的响应缓冲区大小</td>
	</tr>
	<tr>
		<td>0x12</td>
		<td>原始值分段</td>
		<td>服务指定了一个将分段原始数据值的操作，即半个REAL数据类型。</td>
	</tr>
	<tr>
		<td>0x13</td>
		<td>数据不足</td>
		<td>服务未提供执行指定操作所需的所有数据</td>
	</tr>
	<tr>
		<td>0x14</td>
		<td>属性不支持</td>
		<td>请求中指定了不支持的属性</td>
	</tr>
	<tr>
		<td>0x15</td>
		<td>数据过多</td>
		<td>服务提供了超出预期的数据。</td>
	</tr>
	<tr>
		<td>0x16</td>
		<td>对象不存在</td>
		<td>指定的对象在设备中不存在。</td>
	</tr>
	<tr>
		<td>0x17</td>
		<td>服务分段序列错误</td>
		<td>该服务的分段序列当前未对该数据激活</td>
	</tr>
	<tr>
		<td>0x18</td>
		<td>没有存储的属性数据</td>
		<td>在请求服务之前，该对象的属性数据未被保存。</td>
	</tr>
	<tr>
		<td>0x19</td>
		<td>存储操作失败</td>
		<td>由于存储尝试期间的故障，该对象的属性数据无法被保存</td>
	</tr>
	<tr>
		<td>0x1A</td>
		<td>路由失败，请求数据包过大</td>
		<td>服务请求数据包对于传输到目标路径上的网络来说过大。路由设备被迫中止服务</td>
	</tr>
	<tr>
		<td>0x1B</td>
		<td>路由失败，响应数据包过大</td>
		<td>服务响应数据包对于从目标路径上的网络传输来说过大。路由设备被迫中止服务</td>
	</tr>
	<tr>
		<td>0x1C</td>
		<td>缺失属性列表条目数据</td>
		<td>服务未在需要执行请求行为的属性列表中提供某个属性</td>
	</tr>
	<tr>
		<td>0x1D</td>
		<td>无效的属性值列表</td>
		<td>服务返回包含无效属性状态信息的属性列表</td>
	</tr>
	<tr>
		<td>0x1E</td>
		<td>嵌入式服务错误</td>
		<td>嵌入式服务引发了错误</td>
	</tr>
	<tr>
		<td>0x1F</td>
		<td>供应商特定错误</td>
		<td>发生了供应商特定错误。此错误应该仅在其他所有一般错误代码无法正确应用时发生</td>
	</tr>
	<tr>
		<td>0x20</td>
		<td>无效参数</td>
		<td>与请求相关的参数无效。该参数不符合CIP规范的要求和/或在应用对象的规范中定义的要求。</td>
	</tr>
	<tr>
		<td>0x21</td>
		<td>一次性值已写入</td>
		<td>尝试第二次写入一次性介质，或尝试修改已经确立后无法更改的值</td>
	</tr>
	<tr>
		<td>0x22</td>
		<td>收到无效回复</td>
		<td>收到无效回复。可能的原因包括回复服务代码与请求服务代码不匹配，或回复消息短于可预期的最小大小</td>
	</tr>
	<tr>
		<td>0x23</td>
		<td>保留</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0x24</td>
		<td>保留</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0x25</td>
		<td>路径中的密钥故障</td>
		<td>密钥段（即路径中的第一个段）与目标模块不匹配。有关密钥检查失败的部分的更多信息可以从对象特定状态中得出。</td>
	</tr>
	<tr>
		<td>0x26</td>
		<td>路径大小无效</td>
		<td>由于缺乏信息或包含过多的路由数据，无法将路径路由到对象</td>
	</tr>
	<tr>
		<td>0x27</td>
		<td>列表中意外的属性</td>
		<td>尝试设置在当前情况下不可设置的属性</td>
	</tr>
	<tr>
		<td>0x28</td>
		<td>无效的成员ID</td>
		<td>请求中指定的成员ID在指定的类/实例或属性中不可用</td>
	</tr>
	<tr>
		<td>0x29</td>
		<td>成员无法被设置</td>
		<td>发生了对不能修改的成员进行修改的请求</td>
	</tr>
	<tr>
		<td>0x2A</td>
		<td>仅组2服务器一般故障</td>
		<td>此特定于DeviceNet的错误无法在EtherNet/IP中发生</td>
	</tr>
	<tr>
		<td>0x2B - 0xCF</td>
		<td>保留</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xD0 - 0xFF</td>
		<td>供应商特定代码</td>
		<td>发生了特定于对象类的错误</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](3-ethercat-master-io/README.md)
# 3. EtherCAT 主控 IO

<br>

本章解释如何使用 EtherCAT 主控连接我公司选择的多个标准远程 IO 模块。

<br>

**EtherCAT 概述**

EtherCAT 是由 Beckhoff Automation 开发的基于以太网的现场总线系统。

EtherCAT 协议提供非常快速的 IO 数据更新和精确的同步功能。

<br>

**EtherCAT 主控 IO**
   * 对应现有现场总线主控的产品，可以要求 EtherCAT 从设备执行 I/O 数据连接。

<br>

{% hint style="info" %}
   - EtherCAT 主控使用控制器的普通 LAN 端口。

   - 远程 IO 模块使用 Crevis 的 M9386 EtherCAT 网络适配器。
{% endhint %}
[__SOURCE](3-ethercat-master-io/1-Settings-EtherCAT-Master.md)
## 3.1 EtherCAT 主控 IO 设置

<br>

**1. 触摸菜单以进入设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 4: EtherCAT 主控设置]**

<br>

![[图 3.1-1 EtherCAT 主控设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_1.png>) 

<br>

{% hint style="info" %}
   - 在 EtherCAT 主控设置屏幕上检查所选控制器 LAN 端口号。 
{% endhint %}

**2. 连接控制器 LAN 端口和 Remote IO 电缆等进行通信，并检查状态。**

<br>

![[图 3.1-2 硬件连接]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_2.png>) 
![[图 3.1-3 硬件连接]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_3.png>) 

<br>

{% hint style="info" %}
   - 请使用 LAN 电缆连接控制器和 Remote IO。

   - 将 Remote IO 的所有 DIP 开关设置为 OFF。

   - 同时连接 Remote IO 电源和现场电源（24 V DC）。
{% endhint %}

<br>

**3. 在设置菜单中选择 EtherCAT 主控使用为 "ON"。**

<br>

![[图 3.1-4 EtherCAT 主控设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_4.png>)

<br>

{% hint style="info" %}
   - 根据您的使用环境设置通信周期。

   - 支持 1 ms、2 ms 和 5 ms 的通信周期。
{% endhint %}

<br>

**4. 从设置菜单中的从站列表中选择与连接的 Remote IO 模块相同的配置。**

<br>

![[图 3.1-5 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_5.png>)

<br>

{% hint style="info" %}
   - 检查输入和输出字节计数。
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

![[图 3.1-6 EtherCAT 主控设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_6.png>) 

<br>

**5. 在完成设置后重启控制器。**

![[图 3.1-7 EtherCAT 主控设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_7.png>) 

<br>

![[图 3.1-8 EtherCAT 主控设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_8.png>) 

<br>

{% hint style="info" %}
   - 请在完成设置后重启控制器。
{% endhint %}

<br>

**6. 在确认设置值已反映后，检查通信状态。**

![[图 3.1-9 EtherCAT 主控设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_9.png>) 

<br>

{% hint style="info" %}
   - 请检查通信连接状态并查看是否有错误。
{% endhint %}

<br>

![[图 3.1-10 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_10.png>)

<br>

{% hint style="info" %}
   - 请检查 Remote IO 模块上的 LED 确认通信是否正确建立。
{% endhint %}

<br>

{% hint style="info" %}
   **如果在通信过程中出现错误，请参考 ("[**3.2 EtherCAT 主控 IO 错误处理**](../3-ethercat-master-io/2-Error-EtherCAT-Master.md)").**
{% endhint %}

<br>

**7. 在完成通信设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[**4. 工业通信 IO 块分配**](../4-io-block-allocation.md)").**
{% endhint %}
[__SOURCE](3-ethercat-master-io/2-Error-EtherCAT-Master.md)
## 3.2 EtherCAT 主控 IO 错误处理

这是解决在 EtherCAT 主控 IO 设置过程中可能发生的重大错误的方法。

<br>

![[Figure 3.2-1 EtherCAT 主控状态]](<../_assets/3-ethercat-master-io/2-Error/image_1.png>) 

{% hint style="info" %}
   - 请检查 LAN 电缆的连接状态。

   - 检查适配器设备电源是否开启。

   - 请检查设置是否与远程 IO 模块的 IO 组合匹配。
{% endhint %}

<br>
[__SOURCE](4-pnio/README.md)
# 4. PROFINET I/O (Hi7)

<br>

本章解释如何使用 PROFINET I/O 设备 (BD671) 连接机器人控制器的内部输入/输出信号。<br>

<br>

{% hint style="info" %}
PROFINET I/O (BD671) 的功能由 Hi7 机器人控制器支持。<br>
有关 PROFIsafe 手册，请参阅 SafeSpace 2.0 手册 ([SafeSpace 2.0 link](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/korean/3-safety-function/3-safety-function/4-safety-io/4-profisafe))
{% endhint %}
[__SOURCE](4-pnio/1-pnio.md)
## 4.1 PROFINET ?

 **1. PROFINET**
- PROFINET是一个基于以太网的工业自动化通信标准。
- 它支持控制器（PLC、机器人控制器等）与分布式I/O设备（驱动器、传感器、模块等）之间的实时数据交换。

**2. PROFINET规格**
- 数字输入：50、120和240字节（选择一种字节计数类型）
- 数字输出：50、120和240字节（选择一种字节计数类型）
- 安全I/O：8/8字节（激活或禁用）
- 最小通信周期：1毫秒
- 支持的通信速度：10或100 Mbps
- 合规性等级：B
- 网络负载等级：II
- 可选功能：遗留、MRP

**3. PROFINET配置程序**

1) 连接BD671、PROFINET控制器和Hi7 Com
2) GSDML文件注册（TIA portal）
3) PROFINET控制器设置（TIA portal）
4) Hi7设置（TP UI）
5) PROFINET通信验证
6) PROFINET I/O信号分配（FB块设置）

**3.1 连接BD671、F-Host和Hi7 Com**

**3.1.1 LAN电缆连接**
1) 使用LAN电缆连接PROFINET控制器和BD671。
2) 检查链接LED是否在闪烁。
3) 使用LAN电缆连接Hi7 COM的LAN3接口和BD671。
4) 检查链接LED是否在闪烁。

![](../_assets/4-pnio/profisafe_connect.png)

**3.1.2 Hi7 Com连接设置**
1) 按如下菜单导航：系统 -> 控制参数 -> 工业通信 -> EtherCAT主设置
2) 按如下设置。
- EtherCAT主：开启
- 端口：LAN3
3) 从从站列表中选择“OptionBD - PROFINET_IO”，然后按应用按钮。
4) 重启Hi7机器人控制器。
5) 重启后，检查运行、通信、错误LED的状态。

![](../_assets/4-pnio/EC_master_setting1.png)
<br> <br>
![](../_assets/4-pnio/EC_master_setting2.png)


**3.2 GSDML文件注册（TIA portal）**
1) 运行TIA portal。
2) 在菜单中按如下导航：[选项] → [管理通用站描述文件（GSD）]。
3) 点击“...”按钮，设置GSDML文件所在的目录。
4) 从屏幕上显示的列表中选择“GSDML-V2.43-Hyundai-Robotics-HI6-20250418.xml”，然后按[安装]按钮。
5) 检查其是否已作为新设备在硬件目录中注册。 <br>
![](../_assets/4-pnio/profisafe_gsdmal.png)

**3.3 PROFINET控制器设置（TIA portal）**
1) 运行TIA portal并创建一个新项目。
2) 双击设备与网络部分以打开。<br>
![](../_assets/4-pnio/profisafe_device_network.png)

3) 选择支持PROFINET通信的控制器（例如，CPU 1511F-1 PN），并将其拖到网络视图中。
4) 从硬件目录中添加上一步中添加的设备（HRC，PROFINET I/O DAP）并拖到网络视图中。
5) 通过拖动和放置两个设备图形中的LAN端口连接这两个设备。<br>
![](../_assets/4-pnio/profisafe_device_network2.png)

6) 双击“设备与网络”屏幕中的HRC-IO设备。
7) 选择所需插槽。
8) 从右侧目录中拖动所需模块（DI、DO或PROFIsafe I/O）并移动到“设备概述窗口”。<br>
![](../_assets/4-pnio/profisafe_device_network3.png)

9) 双击“设备与网络”屏幕中的HRC-IO设备。
10) 再次单击HRC-IO设备以打开设置屏幕。
11) 导航到下方的常规选项卡。
12) 从左侧菜单中选择以太网地址。
13) 取消勾选“自动生成PROFINET设备名称”。
14) 将“PROFINET设备名称”设置为“hd-hrc-0”，并保存。<br>
![](../_assets/4-pnio/profisafe_device_network4.png)

**3.4 Hi7设置（TP UI）**
1) 将参数设置为以下值，这些值与PNIO控制器中的设置相同。
- PROFINET IO设备名称：hd-hrc-0
- 插槽1：数字输入：240
- 插槽2：数字输出：240
- 插槽3：安全I/O：无
- （无需更改IP地址。）
2) 按“应用”按钮。<br>
![](../_assets/4-pnio/4_1_profinet_config.png)

**3.5 PROFINET通信验证**
**3.5.1 梯形图程序（TIA portal）**
1) 在设备概述选项卡中，创建如下所示的梯形图程序并下载到控制器中。<br>
![](../_assets/4-pnio/5_1_Safety_Ladder.png)
2) 下载后，检查在分配I/O屏幕上是否显示绿色勾选框。<br>
![](../_assets/4-pnio/5_1_Safety_Ladder2.png)

**3.5.2 TP屏幕**
在菜单中，导航到系统 -> 安全系统 -> 监控 -> PROFINET状态。<br>
![](../_assets/4-pnio/5_2_pnio_status.png)
- 检查每个插槽的状态信息。
- 检查计数器是否持续增加。


**3.6 PROFINET I/O信号分配（FB块设置）**
1) 导航到系统 → 控制参数 → 输入/输出信号设置 → FB块分配
2) 根据需要将块设置更改为PROFINET I/O（最多两个）。
 （最大PROFINET I/O大小为240字节，单个FB块大小为120字节。因此，**任何超过两个的设置将被忽略。**）<br>
![](../_assets/4-pnio/6_fb_block.png)

3) 此外，导航到条件设置菜单并检查PLC操作模式是否为OFF。<br>
![](../_assets/4-pnio/6_1_condition.png)
4) 检查TIA portal屏幕和通用I/O屏幕上的输入/输出信号。<br>
![](../_assets/4-pnio/6_3_public_io.png)
[__SOURCE](4-pnio/2-pnio-status.md)
## 5.3 PROFINET 监控

通过选择 **\[System > 8: Safety System > 3: Monitoring > 4: PROFINET Status]** 菜单，您可以按插槽监控 PROFINET 状态。

<p align="center">
<img src="../_assets/4-pnio/PROFINET_monitoring.png"></img>
<em><p align="center">PROFINET 状态监控屏幕</p></em>
</p>

- 大小：指设置的 I/O 大小（单位：字节）。
- 状态：BAD（未使用或通信错误），GOOD（通信正常）
- 计数器：I/O 更新计数（如果持续增加则通信正常）

<p align="center">
<img src="../_assets/4-pnio/profinet_LED.png"></img>
<em><p align="center">BD671(PROFINET) </p></em>
</p>
[__SOURCE](5-io-block-allocation.md)
# 5. 工业通信 IO 读取和写入

这是在完成工业通信设置后，为与控制器进行通信分配 IO 块的方法。

要使用工业通信 IO，必须将 IO 块分配到 fb0 - fb9 区域。

<br>

{% hint style="info" %}
   - 有关 fb 块的 IO 读取/写入方法，请参考以下手册。

      **\[控制器操作手册: 一般输入]**   
      **\[控制器操作手册: 一般输出]**   
{% endhint %}

<br>

**1. 选择 IO 块分配菜单。**
   触摸 **\[系统 > 2: 控制参数 > 2: 输入/输出信号设置 > 6: FB 块分配]** 菜单。

<br>

**2. 为所需 fb 区域指定工业通信类型。**
   指定后，触摸 **\[确定]** 按钮。

![[Figure 5-1]](<_assets/4-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[注意]**: 使用嵌入式 PLC 时，请检查 IO 属性和 DI/DO - X/Y。
{% endhint %}

{% hint style="warning" %}
**\[注意]**: 对于 EtherNet/IP 适配器，最大块大小为 120 字节，最多可以选择 2 个块。任何超过 2 的选择将被忽略。
{% endhint %}
[__SOURCE](6-slave-config-file.md)
# 6. 从属设备描述文件

要配置来自工业通信主站的从属通信，针对每种协议使用从属设备的描述文件。

<br>

可以从我们的网站下载从属设备描述文件。
从 [www.hd-hyundairobotics.com](https://hd-hyundairobotics.com/) -> 工业机器人网站 -> 客户支持 -> 应用软件 下载 "**Hi7 Fieldbus Config**"。

<br>

{% hint style="info" %}
   - EtherNet/IP: EDS 文件

   - PROFINET IO: GSDML (.XML) 文件

   - EtherCAT: ESI (.XML) 文件

   - PROFIBUS-DP: GSD 文件

   - DeviceNet: EDS 文件

   - CC-Link IE Field: CSPP 文件

   - CC-Link IE Basic: CSPP 文件
{% endhint %}

<br>
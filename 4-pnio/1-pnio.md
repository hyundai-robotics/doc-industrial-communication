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
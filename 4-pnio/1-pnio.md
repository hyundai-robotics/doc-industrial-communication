## 4.1 PROFINET ?

 **1. PROFINET**
- PROFINET 是一种基于以太网的工业自动化通信标准。
- 它支持控制器 (PLC、机器人控制器等) 与分布式 I/O 设备 (驱动器、传感器、模块等) 之间的实时数据交换。

**2. PROFINET 规格**
- 数字输入：50, 120 和 240 字节（选择一种字节计数类型）
- 数字输出：50, 120 和 240 字节（选择一种字节计数类型）
- 安全 I/O：8/8 字节（激活或停用）
- 最小通信周期：1 毫秒
- 支持的通信速度：10 或 100 Mbps
- 符合性等级：B
- 网络负载等级：II
- 可选功能：Legacy, MRP

**3. PROFINET 配置程序**

1) BD671、PROFINET 控制器和 Hi7 Com 的连接
2) GSDML 文件注册 (TIA portal)
3) PROFINET 控制器设置 (TIA portal)
4) Hi7 设置 (TP UI)
5) PROFINET 通信验证
6) PROFINET I/O 信号分配 (FB 块设置)

**3.1 BD671、F-Host 和 Hi7 Com 的连接**

**3.1.1 LAN 电缆连接**
1) 使用 LAN 电缆连接 PROFINET 控制器和 BD671。
2) 检查 Link LED 是否在闪烁。
3) 使用 LAN 电缆连接 Hi7 COM 的 LAN3 连接器和 BD671。
4) 检查 Link LED 是否在闪烁。

![](../_assets/4-pnio/profisafe_connect.png)

**3.1.2 Hi7 Com 连接设置**
1) 按如下菜单导航：System -> Control Parameters -> Industrial Communication -> EtherCAT Master Settings
2) 按如下所示进行配置。
- EtherCAT Master : ON
- Port : LAN3
3) 从从站列表中选择 "OptionBD - PROFINET_IO" 并按下 Apply 按钮。
4) 重启 Hi7 机器人控制器。
5) 重启后，检查 Run、Communication、Error LEDs 的状态。

![](../_assets/4-pnio/EC_master_setting1.png)
<br> <br>
![](../_assets/4-pnio/EC_master_setting2.png)


**3.2 GSDML 文件注册 (TIA portal)**
1) 运行 TIA portal。
2) 按右侧菜单中的如下方式导航：[Options] → [Manage general station description file (GSD)]。
3) 点击 "..." 按钮并设置 GSDML 文件所在的目录。
4) 从显示在屏幕上的列表中选择 "GSDML-V2.43-Hyundai-Robotics-HI6-20250418.xml" 并按下 [Install] 按钮。
5) 检查是否已在硬件目录中注册为新设备。 <br>
![](../_assets/4-pnio/profisafe_gsdmal.png)

**3.3 PROFINET 控制器设置 (TIA portal)**
1) 运行 TIA portal 并创建一个新项目。
2) 双击 Device & Network 部分以打开它。<br>
![](../_assets/4-pnio/profisafe_device_network.png)

3) 选择支持 PROFINET 通信的控制器（例如，CPU 1511F-1 PN），并将其拖入网络视图。
4) 从硬件目录中添加上一步中添加的设备 (HRC, PROFINET I/O DAP) 并将其拖入网络视图。
5) 按下图中的方式连接两个设备。<br>
![](../_assets/4-pnio/profisafe_device_network2.png)

6) 双击 "Device & Network" 窗口中的 HRC-IO 设备。
7) 选择所需的插槽。
8) 从右侧目录中拖动所需模块 (DI, DO, 或 PROFIsafe I/O) 并移动到 "Device Overview window"。<br>
![](../_assets/4-pnio/profisafe_device_network3.png)

9) 双击 "Device & Network" 窗口中的 HRC-IO 设备。
10) 再次单击 HRC-IO 设备以打开设置界面。
11) 导航到下面的常规选项卡。
12) 从左侧菜单中选择以太网地址。
13) 取消选中 "自动生成 PROFINET 设备名称"。
14) 将 "PROFINET 设备名称" 设置为 "hd-hrc-0" 并保存。<br>
![](../_assets/4-pnio/profisafe_device_network4.png)

**3.4 Hi7 设置 (TP UI)**
1) 将参数设置为与 PNIO 控制器中设置的值相同的值。
- PROFINET IO 设备名称 : hd-hrc-0
- 插槽 1 : 数字输入 : 240
- 插槽 2 : 数字输出 : 240
- 插槽 3 : 安全 I/O : 不
- (无需更改 IP 地址。)
2) 按下 "Apply" 按钮。<br>
![](../_assets/4-pnio/4_1_profinet_config.png)

**3.5 PROFINET 通信验证**
**3.5.1 梯形图程序 (TIA portal)**
1) 在 Device Overview 选项卡中，创建如下所示的梯形图程序并将其下载到控制器。<br>
![](../_assets/4-pnio/5_1_Safety_Ladder.png)
2) 下载后，检查 Distribution I/O 屏幕上是否显示绿色复选框。<br>
![](../_assets/4-pnio/5_1_Safety_Ladder2.png)

**3.5.2 TP 屏幕**
在菜单中导航到 System -> Safety System -> Monitoring -> PROFINET Status。<br>
![](../_assets/4-pnio/5_2_pnio_status.png)
- 检查每个插槽的状态信息。
- 检查计数器是否持续增加。


**3.6 PROFINET I/O 信号分配 (FB 块设置)**
1) 导航到 System → Control Parameters → Input/Output Signal Settings → FB Block Assignment
2) 根据需要将块设置更改为 PROFINET I/O（最多两个）。
 (最大 PROFINET I/O 大小为 240 字节，单个 FB 块大小为 120 字节。因此，**任何超过两个的设置将被忽略。**）<br>
![](../_assets/4-pnio/6_fb_block.png)

3) 另外，导航到 Condition Settings 菜单，并检查 PLC 操作模式是否为 OFF。<br>
![](../_assets/4-pnio/6_1_condition.png)
4) 在 TIA portal 屏幕和 General I/O 屏幕上检查输入/输出信号。<br>
![](../_assets/4-pnio/6_3_public_io.png)
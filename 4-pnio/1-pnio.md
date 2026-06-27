## 4.1 PROFINET 通信设置

 **1. PROFINET**
- PROFINET 是用于工业自动化的基于以太网的通信标准。
- 它支持控制器（PLC、机器人控制器等）与分布式 I/O 设备（驱动器、传感器、模块等）之间的实时数据交换。

**2. PROFINET 规格**
- 数字输入：50、120 和 240 字节（选择一种字节计数类型）
- 数字输出：50、120 和 240 字节（选择一种字节计数类型）
- 安全 I/O：8/8 字节（激活或停用）
- 最小通信周期：1 毫秒
- 支持的通信速度：10 或 100 Mbps
- 一致性类别：B
- 网络负载类别：II
- 可选功能：遗留、MRP

**3. PROFINET 配置程序**

1) 连接 BD671、PROFINET 控制器和 Hi7 Com
2) GSDML 文件注册（TIA portal）
3) PROFINET 控制器设置（TIA portal）
4) Hi7 设置（TP UI）
5) PROFINET 通信验证
6) PROFINET I/O 信号分配（FB 块设置）

**3.1 连接 BD671、F-Host 和 Hi7 Com**

**3.1.1 LAN 电缆连接**
1) 使用 LAN 电缆连接 PROFINET 控制器和 BD671。
2) 检查 Link LED 是否在闪烁。
3) 使用 LAN 电缆连接 Hi7 COM 的 LAN3 连接器和 BD671。
4) 检查 Link LED 是否在闪烁。

![](../_assets/4-pnio/profisafe_connect.png)

**3.1.2 Hi7 Com 连接设置**
1) 如下所示导航到菜单：系统 -> 控制参数 -> 工业通信 -> EtherCAT 主设置
2) 按如下所示进行配置。
- EtherCAT 主机：开启
- 端口：LAN3
3) 从从设备列表中选择 "OptionBD - PROFINET_IO" 并按下 "应用" 按钮。
4) 重启 Hi7 机器人控制器。
5) 重启后，检查运行、通信、错误 LED 的状态。

![](../_assets/4-pnio/EC_master_setting1.png)
<br> <br>
![](../_assets/4-pnio/EC_master_setting2.png)


**3.2 GSDML 文件注册（TIA portal）**
1) 运行 TIA portal。
2) 在菜单中按如下显示导航：[选项] → [管理通用站描述文件（GSD）]。
3) 点击 "..." 按钮并设置 GSDML 文件所在的目录。
4) 从屏幕上显示的列表中选择 "GSDML-V2.43-Hyundai-Robotics-Hi7-20251127.xml" 并按下 [安装] 按钮。
5) 检查它是否已作为新设备注册在硬件目录中。 <br>
![](../_assets/4-pnio/profisafe_gsdmal.png)

**3.3 PROFINET 控制器设置（TIA portal）**
1) 运行 TIA portal 并创建一个新项目。
2) 双击设备和网络部分打开它。<br>
![](../_assets/4-pnio/profisafe_device_network.png)

3) 选择支持 PROFINET 通信的控制器（例如，CPU 1511F-1 PN）并将其拖到网络视图中。
4) 从硬件目录中添加在上一步中添加的设备（HRC, PROFINET I/O DAP）并将其拖到网络视图中。
5) 通过拖放两个设备图中的 LAN 端口连接这两个设备。<br>
![](../_assets/4-pnio/profisafe_device_network2.png)

6) 双击 "设备和网络" 屏幕中的 HRC-IO 设备。
7) 选择所需的插槽。
8) 从右侧目录中拖动所需模块（DI、DO 或 PROFIsafe I/O）并移动到 "设备概览窗口"。<br>
![](../_assets/4-pnio/profisafe_device_network3.png)

9) 双击 "设备和网络" 屏幕中的 HRC-IO 设备。
10) 再次点击 HRC-IO 设备以打开设置屏幕。
11) 导航到下方的常规选项卡。
12) 从左侧菜单中选择以太网地址。
13) 取消选中 "自动生成 PROFINET 设备名称"。
14) 将 "PROFINET 设备名称" 设置为 "hd-hrc-0" 并保存。<br>
![](../_assets/4-pnio/profisafe_device_network4.png)

**3.4 Hi7 设置（TP UI）**
1) 将参数设置为以下值，这些值与 PNIO 控制器中设置的值相同。
- PROFINET IO 设备名称：hd-hrc-0
- 插槽 1：数字输入：240
- 插槽 2：数字输出：240
- 插槽 3：安全 I/O：无
- （无需更改 IP 地址。）
2) 按下 "应用" 按钮。<br>
![](../_assets/4-pnio/4_1_profinet_config.png)

**3.5 PROFINET 通信验证**
**3.5.1 梯形图程序（TIA portal）**
1) 在设备概览选项卡中，创建如下所示的梯形图程序并下载到控制器。<br>
![](../_assets/4-pnio/5_1_Safety_Ladder.png)
2) 下载后，检查分配 I/O 屏幕上是否显示绿色复选框。<br>
![](../_assets/4-pnio/5_1_Safety_Ladder2.png)

**3.5.2 TP 屏幕**
在菜单中导航到 **\[系统 > 2: 控制参数 > 11: 工业通信 > 5: PROFINET 设置]**<br>
![](../_assets/4-pnio/PROFINET_monitoring.png)
- 检查每个插槽的状态信息。
- 检查计数器是否持续增加。


**3.6 PROFINET I/O 信号分配（FB 块设置）**
1) 导航到系统 → 控制参数 → 输入/输出信号设置 → FB 块分配
2) 根据需要将块设置更改为 PROFINET I/O（最多两个）。
 (最大的 PROFINET I/O 大小为 240 字节，单个 FB 块的大小为 120 字节。因此，**任何超过两个的设置将被忽略。**)<br>
![](../_assets/4-pnio/6_fb_block.png)

3) 另外，导航到条件设置菜单并检查 PLC 操作模式是否为 OFF。<br>
![](../_assets/4-pnio/6_1_condition.png)
4) 检查 TIA portal 屏幕和通用 I/O 屏幕上的输入/输出信号。<br>
![](../_assets/4-pnio/6_3_public_io.png)
## 4.1 PROFINET ?

**1. PROFINET？**
- PROFINET是一种基于以太网的工业自动化通信标准。
- 支持控制器（PLC、机器人控制器等）与分布式I/O设备（驱动器、传感器、模块等）之间的实时数据交换。

**2. PROFINET规格**
- 数字输入：50、120、240 bytes（选择1个）
- 数字输出：50、120、240 bytes（选择1个） 
- 安全输入输出：8/8 bytes（启用或禁用） 
- 最小通信周期：1 msec
- 支持通信速度：10或100 Mbps
- Conformance Class : B
- Netload Class : II
- Optional Feature : Legacy, MRP

**3. PROFINET设置流程**

1) BD671与PROFINET控制器 & Hi7 Com的连接
2) GSDML文件注册（TIA Portal）
3) PROFINET控制器设置（TIA Portal）
4) Hi7设置（TP UI）
5) PROFINET通信确认
6) PROFINET I/O信号分配（FB Block Settings）

**3.1 BD671与F-Host & Hi7 Com的连接**

**3.1.1 网线连接**
1) 用网线连接 PROFINET 控制器与 BD671。
2) 确认 Link LED 是否闪烁。
3) 用网线连接 Hi7 COM 的 LAN3 连接器与 BD671。
4) 确认 Link LED 是否闪烁。

![](../_assets/4-pnio/profisafe_connect.png)

**3.1.2 Hi7 Com的连接设置**
1) 依次进入菜单：系统 -> 控制参数 -> 工业通信-> EtherCAT Master设置
2) 按如下所示进行设置：
- EtherCAT Master : ON
- Port : LAN3
3) 在从站列表中选择“OptionBD – PROFINET_IO”并按下应用按钮。
4) 重启Hi7机器人控制器。
5) 重启后确认Run & Communication & Error LED的点亮状态。

![](../_assets/4-pnio/EC_master_setting1.png)
<br> <br>
![](../_assets/4-pnio/EC_master_setting2.png)


**3.2 GSDML 文件注册（TIA Portal）**
1) 执行 TIA Portal
2) 如右侧所示，依次进入菜单：[Options] → [Manage general station description file (GSD)]。
3) 点击“…”按钮后，设置 GSDML file 所在的目录。
4) 从屏幕显示的列表中，选择“GSDML-V2.43-Hyundai-Robotics-HI6-20250418.xml”并按下【Install】按钮。
5) 确认其是否在硬件目录中注册为新设备。 <br>
![](../_assets/4-pnio/profisafe_gsdmal.png)

**3.3 PROFINET 控制器设置（TIA Portal）**
1) 执行TIA Portal并创建新项目。
2) 双击Device & Network部分来将其打开。<br>
![](../_assets/4-pnio/profisafe_device_network.png)

3) 选择支持PROFINET通信的控制器（例如CPU 1511F-1 PN）并拖放到网络视图。
4) 从硬件目录中添加上一步骤添加的设备（HRC、PROFINET I/O DAP）并拖放到网络视图。
5) 通过鼠标拖放将两个设备图中的LAN端口相互连接。<br>
![](../_assets/4-pnio/profisafe_device_network2.png)

6) 在“Device & Network”界面中双击HRC-IO设备。
7) 选择所需的插槽。
8) 从右侧目录中将所需的模块（DI、DO或PROFIsafe I/O）拖动到“Device Overview window”。<br>
![](../_assets/4-pnio/profisafe_device_network3.png)

9) 在“Device & Network”界面中双击HRC-IO设备。
10) 再次点击HRC-IO设备来打开Setting界面。
11) 移动到下面的General标签。
12) 在左侧菜单中选择Ethernet addresses。
13) 取消勾选“Generate PROFINET device name automatically.”部分。
14) 将“PROFINET device name”设置为“hd-hrc-0”并保存。<br>
![](../_assets/4-pnio/profisafe_device_network4.png)

**3.4 Hi7设置（TP UI）**
1) 使用与PNIO控制器中设置的相同值来设置下列参数。
- PROFINET IO Device Name : hd-hrc-0
- Slot 1 : Digital Input : 240
- Slot 2 : Digital Output : 240
- Slot 3 : Safety I/O : No
- （IP地址无需更改。）
2) 按“应用”按钮。<br>
![](../_assets/4-pnio/4_1_profinet_config.png)

**3.5 PROFINET 通信确认**
**3.5.1 梯形图程序（Tia Portal）**
1) 在 Device Overview 选项卡中，创建如下梯形图程序并下载到控制器。<br>
![](../_assets/4-pnio/5_1_Safety_Ladder.png)
2) 下载后，在 Distribution I/O 界面中确认是否显示绿色复选框。<br>
![](../_assets/4-pnio/5_1_Safety_Ladder2.png)

**3.5.2 TP 界面**
从菜单中移动到：系统 -> 安全系统 -> 监控 -> PROFINET 状态。<br>
![](../_assets/4-pnio/5_2_pnio_status.png)
- 确认各插槽的状态信息
- 确认Counter是否持续递增


**3.6 PROFINET I/O信号分配（FB Block Settings）**
1）依次进入：系统 → 控制参数 → 输入输出信号设置 → FB块分配
2) 将所需数量的块设置更改为PROFINET I/O，数量不得超过2个。
 （最大PROFINET I/O大小为240字节，单个FB块的大小为120字节。因此，**超过2个的设置将被忽略。**）<br>
![](../_assets/4-pnio/6_fb_block.png)

3) 另外，移动到条件设置菜单并确认PLC运行模式是否为OFF。<br>
![](../_assets/4-pnio/6_1_condition.png)
4) 在TIA Portal及通用I/O界面中，确认输入输出信号。<br>
![](../_assets/4-pnio/6_3_public_io.png)

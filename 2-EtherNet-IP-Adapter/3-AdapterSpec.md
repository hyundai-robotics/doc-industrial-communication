## 2.3 EtherNet/IP适配器

**2.3.1 EtherNet/IP适配器规格**
|项目|说明|
|------|---|
|设备类型|General Purpose Discrete I/O (7)|
|Input Assembly Instance|100|
|Output Assembly Instance|112|
|Input Size Range(bytes)|0 - 240|
|Output Size Range(bytes)|0 - 240|
|RPI Range (ms)|5 – 3000|<br>

**2.3.2 通过示教器进行EtherNet/IP适配器的设置及监控**
从主界面移动到：“SYSTEM” > “Control Parameter” > “Industrial Communication” > “Ethernet/IP适配器”<br>
![Config.PNG](../_assets/2-EtherNet-IP-Adapter/Spec/Config.PNG)<br>
*[图2.3.1 设置]*<br>

**[Network]**
-	功能启用：选择是否启用Ethernet/IP适配器
-	以太网端口选择：选择所要与Ethernet/IP Scanner连接的LAN Port（所选LAN Port的信息显示在下一行）<br>

**[I/O Size]**
-	输入字节数：可设置0～240
-	输出字节数：可设置0～240<br>

**[Monitoring]**
- 运行（Run）：表示Ethernet/IP的I/O Data交换状态（On：正在正常通信，Off：未在通信）
- 准备（Ready）：表示Ethernet/IP适配器的初始化状态（On：初始化正常，Off：初始化异常）
- 错误（Error）：显示Ethernet/IP适配器的报警或警告状态（On：报警/警告状态，Off：正常）
- 版本：显示Ethernet/IP适配器S/W版本信息
- 错误代码：发生报警或警告时显示报警/警告代码 

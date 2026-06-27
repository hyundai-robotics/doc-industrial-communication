# 2. EtherNet/IP

本章介绍了内置 EtherNet/IP 主站（扫描器）和从站（适配器）的特性和配置方法。
<br>

**EtherNet/IP 概述**

<br>

EtherNet/IP 是由 CI（ControlNet International）和 ODVA（Open DeviceNet Vendors Association）开发的基于以太网的开放工业通信协议。

在工厂环境中，各种设备如传感器、远程 I/O、马达驱动器、HMI、PLC 和机器人控制器可以连接到单一的 EtherNet/IP 网络，无论制造商如何。

![[Figure 2-1 EtherNet/IP]](<../_assets//2-ethernet-ip/image_1.png>)

<br>

EtherNet/IP 根据其通信功能分为以下几类：

**扫描器类**

   * 这些产品对应于传统的现场总线主机，可以向 EtherNet/IP 适配器或扫描器请求 I/O 数据连接。

<br>

**适配器类**

  * 这些产品对应于传统的现场总线从机，是 EtherNet/IP 扫描器请求的实时 I/O 数据的连接目标。
    
  * 适配器无法在没有扫描器请求的情况下独立传输或接收实时 I/O 数据。

<br>

**消息类**

   * 这些产品能够与所有类的产品之间发送和接收显式消息，但不支持实时 I/O 数据传输。
   
   * 示例包括用于程序上传/下载的计算机接口卡和网络配置工具。

<br>

**缩写**

<br>

|缩写|描述|
|---------------|------------------------------|
|适配器|一个从 EtherNet/IP 扫描器收集输出数据并向其传输输入数据的设备|
|扫描器|一个向终端设备（EtherNet/IP 适配器）发送输出数据并收集输入数据的设备|
|LAN|局域网|
|RPI|请求包间隔|
|PLC|可编程逻辑控制器|
|T2O|目标到源（适配器 -> 扫描器）|
|O2T|源到目标（扫描器 -> 适配器)|
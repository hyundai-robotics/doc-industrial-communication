### 1.3.3 EtherNet/IP

本章描述了EtherNet/IP主控（扫描器）和从控（适配器）的特性及其设置方法。

<br>

**EtherNet/IP概述**

EtherNet/IP是一种基于以太网的开放工业通信协议，由CI（ControlNet International）和ODVA（开放设备网供应商协会）开发。

在工厂中，各种设备如传感器、远程IO、马达驱动器、HMI、PLC和机器人控制器可以在不考虑制造商的情况下连接到一个EtherNet/IP网络。

![[Figure 1.3.3-1 EtherNet/IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/image_1.png>)

<br>

根据通信功能，EtherNet/IP可分为以下几类。

**扫描器类**
   * 对应于现有现场总线主控的产品，可以要求EtherNet/IP适配器或扫描器执行I/O数据连接。

<br>

**适配器类**
  * 对应于现有现场总线从控的产品，是EtherNet/IP扫描器请求的实时I/O数据连接的目标。

  * 适配器无法在没有扫描器的情况下独立发送和接收实时I/O数据。

<br>

**消息类**
   * 能够发送和接收对所有类产品的显式消息，但不支持实时I/O数据的传输和接收。

   * 例如，这些产品可以是用于程序上传/下载的计算机接口卡和网络设置工具等。
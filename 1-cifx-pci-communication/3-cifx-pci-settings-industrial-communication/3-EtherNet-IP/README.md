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
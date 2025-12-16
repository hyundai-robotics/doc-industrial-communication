# 1.3.3 EtherNet/IP

本章说明EtherNet/IP Master（Scanner）和Slave（Adapter）的特性及设置方法。

<br>

##### EtherNet/IP 概要

EthetNet/IP是由CI（ControlNet International）和ODVA（Open DeviceNet Vendors Association）开发的基于以太网的开放式工业通信协议。

在工厂中，传感器、远程IO、电机驱动器、HMI、PLC、机器人控制器等各种设备，无论制造商如何，都可以连接到同一个EtherNet/IP网络。

![[图 1.3.3-1 EtherNet/IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/image_1.png>)


<br>

EtherNet/IP根据通信功能区分如下。

##### Scanner Class
   * 对应于现有现场总线主站（Master）的产品，可以向EtherNet/IP Adapter或Scanner请求I/O数据连接。

<br>

##### Adapter Class
  * 对应于现有现场总线从站（Slave）的产品，是EtherNet/IP Scanner请求的Real-Time I/O数据连接目标（Target）。

  * Adapter不能在没有Scanner的情况下自行收发Real-Time I/O数据。

<br>

##### Messaging Class
   * 本产品支持对所有Class产品进行Explicit消息的收发，但不支持Real-Time I/O数据的收发。

   * 例如，用于程序上传/下载的计算机接口卡、网络设置工具等。
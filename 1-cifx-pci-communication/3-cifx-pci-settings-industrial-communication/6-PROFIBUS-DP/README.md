### 1.3.6 PROFIBUS-DP

本章描述了PROFIBUS-DP主设备和从设备的特性以及如何设置它们。

<br>

**Fieldbus概述**

Fieldbus是一种行业标准，已开放以通过单根电缆连接传感器、按钮、电机驱动器和操作接口等设备到PLC（可编程逻辑控制器）并在工厂中进行操作。

Fieldbus提供智能服务，例如对整个网络状态的中央监控和网络的重新配置。

例如，可以为传感器和开关设置详细信息、操作和模式，而不仅仅是简单的开/关。

使用单根电缆可以减少布线的时间和成本，简化配置，并在维护中提供优势。

此外，与具有非确定性响应特性的通用通信协议不同，Fieldbus保证数据响应速度，以满足时间特性至关重要的工业应用。

![[Figure 1.3.6-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/image_1.png>) 

<br>

一个Fieldbus网络连接一个主设备和多个从设备。
主设备搜索并管理整个网络，并与从设备交换数据。

一般来说，PLC是主设备，而传感器、按钮、控制器等可以配置为从设备。
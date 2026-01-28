### 1.3.9 CC-Link IE Field

本章说明CC-Link IE Field Slave的特性及设置方法。 


<br>

**Fieldbus 概要**

现场总线（Fieldbus）是一种开放的工业标准， 用于在工厂中通过一根电缆将传感器、按钮、电机驱动器、操作界面等设备 与 PLC（Programmable Logic Controller）连接并进行控制。

现场总线提供从中央监控整个网络状态或重新配置等的智能服务。

例如，对于传感器或开关，不仅可实现简单的On/Off，还可以提供详细信息、动作、模式设置等。

使用单根电缆可以节省布线的时间和费用，且配置简单，有利于维护。

另外，与一般通信协议具有非确定性响应（Non-deterministic Response）的特性不同，数据响应速度有保证，满足对时限特性要求严格的工业应用。

![[图 1.3.9-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/image_1.png>) 

<br>

1个现场总线网络连接1个主站（Master）设备和多个从站（Slave）设备。
主站设备搜索／管理整个网络并与从站设备交换数据。

一般来说，PLC是主站设备，其他传感器、按钮、控制器等可以作为从站设备构成。

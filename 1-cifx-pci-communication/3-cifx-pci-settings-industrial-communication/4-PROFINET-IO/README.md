### 1.3.4 PROFINET IO

本章节描述了PROFINET IO主控（控制器）和从设备（设备）的特性以及如何设置它们。

<br>

**PROFINET IO 概述**

PROFINET IO是一种基于以太网的开放工业通信协议，逐步从PROFIBUS-DP和工业以太网演变而来。

![[Figure 1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>)

<br>

它遵循提供者-消费者模型进行数据交换，并可以分为以下三类产品。

**IO 控制器类**
   * 与现有PROFIBUS-DP类1主控对应的产品，这些产品是运行自动化程序如PLC的类型。

   * IO 控制器向设置的IO设备提供输出数据，并从它们那里消费输入数据。

<br>

**IO 设备类**
  * 与现有PROFIBUS-DP从设备对应的产品，通过PROFINET IO与PLC等IO控制器连接。

  * IO设备向IO控制器提供输出数据，提供输入数据，并消费输出数据。

<br>

**IO 监督类**
   * 与现有PROFIBUS-DP类2主控对应的产品，包括用于网络配置和诊断的编程设备、PC、HMI。
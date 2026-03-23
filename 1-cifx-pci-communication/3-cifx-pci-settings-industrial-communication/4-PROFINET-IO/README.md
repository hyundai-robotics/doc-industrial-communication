### 1.3.4 PROFINET IO

本章描述了PROFINET IO主站（控制器）和从站（设备）的特性，以及如何设置它们。

<br>

**PROFINET IO 概述**

PROFINET IO是一种基于以太网的开放工业通信协议，逐步从PROFIBUS-DP和工业以太网演变而来。

![[Figure 1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>) 

<br>

它遵循提供者-消费者模型进行数据交换，可以分为以下三类产品。

**IO 控制器类**
   * 对应现有PROFIBUS-DP类别1主站的产品，是运行自动化程序（例如PLC）的产品类型。

   * IO控制器向设置的IO设备提供输出数据，并从它们处获取输入数据。

<br>

**IO 设备类**
  * 对应现有PROFIBUS-DP从站的产品，通过PROFINET IO与PLC等IO控制器连接。

  * IO设备向IO控制器提供输出数据，提供输入数据，并消耗输出数据。

<br>

**IO 监视器类**
   * 对应现有PROFIBUS-DP类别2主站的产品，包括用于网络配置和诊断的编程设备、PC、HMI等。
### 1.3.4 PROFINET IO

本章描述了PROFINET IO主控（控制器）和从设备（设备）的特性，以及如何进行设置。 

<br>

**PROFINET IO概述**

PROFINET IO是基于以太网的开放工业通信协议，逐步从PROFIBUS-DP和工业以太网演变而来。

![[Figure 1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>) 

<br>

它遵循提供者-消费者模型进行数据交换，可以被分类为以下三类产品。

**IO控制器类**
   * 与现有PROFIBUS-DP类1主控相对应的产品，是运行自动化程序（如PLC）的产品类型。

   * IO控制器向设置的IO设备提供输出数据，并从它们那里消耗输入数据。

<br>

**IO设备类**
  * 与现有PROFIBUS-DP从设备相对应的产品，通过PROFINET IO与如PLC的IO控制器连接。

  * IO设备向IO控制器提供输出数据，提供输入数据，并消耗输出数据。

<br>

**IO监控器类**
   * 与现有PROFIBUS-DP类2主控相对应的产品，包括用于网络配置和诊断的编程设备、PC、HMI。
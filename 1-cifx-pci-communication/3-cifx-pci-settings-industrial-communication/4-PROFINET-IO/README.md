# 1.3.4 PROFINET IO

本章说明PROFINET IO Master（Controller）和Slave（Device）的特性及设置方法。 

<br>

##### PROFINET IO概要

PROFINET IO是从PROFIBUS-DP和工业以太网逐步发展而来的基于以太网的开放式工业通信协议。

![[图1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>) 

<br>

数据交换遵循Provider、Consumer模型，产品可分为以下3种Class。

##### IO Controller Class
   * 对应于现有PROFIBUS-DP Class 1主站（Master）的产品，是运行自动化程序的产品，例如PLC等。

   * IO Controller向为其配置的IO Device提供输出数据，并消费输入数据。

<br>

##### IO Device Class
  * 对应于现有PROFIBUS-DP从站（Slave）的产品，通过PROFINET IO连接到PLC等IO Controller。

  * IO Device向IO Controller提供输出数据，提供输入数据，并消费输出数据。

<br>

##### IO Supervisor Class
   * 对应于现有PROFIBUS-DP中Class 2主站（Master）的产品，包括用于网络配置及诊断的编程设备、PC、HMI等。

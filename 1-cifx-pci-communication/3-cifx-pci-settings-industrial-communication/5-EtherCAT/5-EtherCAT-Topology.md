# 1.3.5.5 EtherCAT电缆接线（Topology）

<br>

EtherCAT与现有工业通信不同，对电缆接线及可使用的Ethernet Port有限制。

##### 1. Ethernet Port

{% hint style="info" %}
\.      连接EtherCAT Master与Slave时，必须使用Port 0号。
{% endhint %}

![[图 1.3.5.5-1 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_1.png>)

{% hint style="info" %}
\.      Master连接1个Slave时
{% endhint %}

![[图 1.3.5.5-2 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_2.png>)

{% hint style="info" %}
\.      Master连接2个以上Slave时

\.      从Slave Port 1号连接到下一个Slave Port 0号。
{% endhint %}

![[图 1.3.5.5-3 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_3.png>)

<br>

##### 2. Redundancy

{% hint style="info" %}
\.      Master使用Redundancy功能时

\.      通过连接最后Slave的Port 1号与Master的Port 1号，形成Ring结构。
{% endhint %}

![[图 1.3.5.5-4 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_4.png>)


<br>

##### 3. 电缆接线错误


"[请参考“**1.4.1 ERROR Code**”。](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)" 참고해 주십시오.

<br>

{% hint style="info" %}
\.      Network Scan无法进行时

\.      请检查连接到Master的端口及电缆。
{% endhint %}

![[图 1.3.5.5-5 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
\.      Topology Error (Configuration Error)

\.      请检查Master与Slave之间的电缆接线。
{% endhint %}

![[图 1.3.5.5-6 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
\.      Topology Error 2（Configuration正常但诊断时出错）

\.      请检查Master与Slave之间的电缆接线。

\.      请检查Slave与Slave之间的电缆接线。
{% endhint %}

![[图 1.3.5.5-7 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_7.png>)

![[图 1.3.5.5-8 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
\.      Mandatory Slave Missing Error

\.      请检查Slave与Slave之间的电缆接线。
{% endhint %}

![[图 1.3.5.5-9 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_9.png>)
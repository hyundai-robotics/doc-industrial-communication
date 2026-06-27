#### 1.3.5.5 EtherCAT 电缆接线（拓扑）

<br>

与现有工业通信不同，EtherCAT在电缆接线和可用以太网端口上有其限制。

**1. 以太网端口**

{% hint style="info" %}
   - 连接EtherCAT主站和从站时，应使用端口0。
{% endhint %}

![[Figure 1.3.5.5-1 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
   - 当一个从站连接到主站时
{% endhint %}

![[Figure 1.3.5.5-2 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
   - 当两个或更多从站连接到主站时

   - 从从站端口1连接到下一个从站端口0。
{% endhint %}

![[Figure 1.3.5.5-3 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_3.png>)

<br>

**2. 冗余**

{% hint style="info" %}
   - 在主站使用冗余功能时

   - 将最后一个从站的端口1和主站的端口1连接以形成环结构。
{% endhint %}

![[Figure 1.3.5.5-4 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_4.png>) 


<br>

**3. 电缆接线错误**


请参考 "[1.4.1 错误代码](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"。

<br>

{% hint style="info" %}
   - 如果网络扫描功能无法正常工作。

   - 请检查连接到主站的端口和电缆。
{% endhint %}

![[Figure 1.3.5.5-5 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
   - 拓扑错误（配置错误）

   - 请检查主站和从站之间的电缆接线。
{% endhint %}

![[Figure 1.3.5.5-6 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
   - 拓扑错误2（配置期间正常，但诊断时有错误）

   - 请检查主站和从站之间的电缆接线。

   - 请检查从站之间的电缆接线。
{% endhint %}

![[Figure 1.3.5.5-7 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_7.png>)

![[Figure 1.3.5.5-8 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
   - 必须从站缺失错误

   - 请检查从站之间的电缆接线。
{% endhint %}

![[Figure 1.3.5.5-9 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_9.png>)
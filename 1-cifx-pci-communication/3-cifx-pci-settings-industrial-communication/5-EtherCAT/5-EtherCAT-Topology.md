#### 1.3.5.5 EtherCAT 电缆连接 (拓扑)

<br>

与现有工业通信不同，EtherCAT 在电缆连接和可用的以太网端口方面有一定的限制。

**1. 以太网端口**

{% hint style="info" %}
   - 在连接 EtherCAT 主站与从站时，应使用端口 0。
{% endhint %}

![[Figure 1.3.5.5-1 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
   - 当一个从站连接到主站时
{% endhint %}

![[Figure 1.3.5.5-2 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
   - 当两个或多个从站连接到主站时

   - 从从站端口 1 连接到下一个从站端口 0。
{% endhint %}

![[Figure 1.3.5.5-3 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_3.png>)

<br>

**2. 冗余**

{% hint style="info" %}
   - 当在主站使用冗余功能时 

   - 将最后一个从站的端口 1 和主站的端口 1 连接以形成环形结构。
{% endhint %}

![[Figure 1.3.5.5-4 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_4.png>) 


<br>

**3. 电缆连接错误**


请参考 "[1.4.1 错误代码](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"。

<br>

{% hint style="info" %}
   - 如果网络扫描功能无法工作。

   - 请检查连接到主站的端口和电缆。
{% endhint %}

![[Figure 1.3.5.5-5 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
   - 拓扑错误 (配置错误)

   - 请检查主站与从站之间的电缆连接。
{% endhint %}

![[Figure 1.3.5.5-6 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
   - 拓扑错误 2 (配置期间正常，但是在诊断时有错误)

   - 请检查主站与从站之间的电缆连接。

   - 请检查从站之间的电缆连接。
{% endhint %}

![[Figure 1.3.5.5-7 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_7.png>)

![[Figure 1.3.5.5-8 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
   - 必须的从站缺失错误

   - 请检查从站之间的电缆连接。
{% endhint %}

![[Figure 1.3.5.5-9 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_9.png>)
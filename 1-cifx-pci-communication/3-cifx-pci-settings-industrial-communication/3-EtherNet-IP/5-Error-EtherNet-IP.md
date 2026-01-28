#### 1.3.3.5 EtherNet/IP错误处理

这是解决EtherNet/IP设置中可能发生的主要错误的方法。

可以利用Sycon.Net的Diagnosis功能来确认错误。

<br>

请参考“[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)”。

<br>

**1. 通信电缆断线错误**

{% hint style="info" %}
   - 请确认 LAN 电缆的连接状态。

   - 请确认 Adapter Device 的电源是否开启。
{% endhint %}

![[图 1.3.3.5-1 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_1.png>) 


<br>

**2. IP Address设置错误**

{% hint style="info" %}
   - 请确认Master - Slave Device的IP Address。

   - 如果Adapter Device中已设置的IP Address与Sycon.net中所输入的值不同，则会发生错误。

{% endhint %}

![[图 1.3.3.5-2 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_2.png>) 

![[图 1.3.3.5-3 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_3.png>) 



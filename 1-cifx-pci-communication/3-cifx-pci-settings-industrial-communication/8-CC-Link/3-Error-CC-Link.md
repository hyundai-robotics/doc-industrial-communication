# 1.3.8.3 CC-Link Slave 错误处理

<br>

请参考“[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)”。

<br>

##### 1. CC-Link 终端电阻

{% hint style="info" %}
\.      连接CC-Link电缆时，必须在终端添加电阻。

\.      如果通信无法连接，请确认终端电阻。

\.      CC-Link终端电阻：110欧
{% endhint %}

{% hint style="info" %}
\.      如下图所示，如果CIFX-50 CC PCI是CC-Link的终端，请添加终端电阻。
{% endhint %}

![[图1.3.8.5-1 CC-Link终端电阻]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/5-Error/image_1.png>) 



##### 2. CC-Link ERROR

{% hint style="info" %}
\.      为了实现通信，需要向 CC-Link 电缆提供 24V 电源。

\.      如果通信无法连接，请检查是否提供 24V 电源。
{% endhint %}

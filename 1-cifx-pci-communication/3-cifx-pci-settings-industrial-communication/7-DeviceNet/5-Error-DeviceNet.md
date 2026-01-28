#### 1.3.7.5 DeviceNet错误处理

<br>

请参考“[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)”。

<br>

**1. DeviceNet终端电阻**

{% hint style="info" %}
\.      连接DeviceNet电缆时必须在终端添加电阻。

\.      如果Network Scan无法进行，请检查终端电阻。

\.      DeviceNet 终端电阻：120欧
{% endhint %}

{% hint style="info" %}
\.      如下图所示，如果CIFX-50 DN PCI是DeviceNet的终端，请添加终端电阻。
{% endhint %}

![[图1.3.7.5-1 DeviceNet终端电阻]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_1.png>) 

{% hint style="info" %}
\.      如下图所示，如果DeviceNet Remote IO是终端，请添加终端电阻或操作DIP Switch。
{% endhint %}

![[图 1.3.7.5-2 DeviceNet终端电阻]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_2.png>) 

<br>

**2. 通信速度**

{% hint style="info" %}
\.      如果DeviceNet Master与Slave之间的通信速度不同，可能无法进行Network Scan。

\.      如果Network Scan无法进行，请检查通信速度。
{% endhint %}

![[图 1.3.7.5-3 DeviceNet Baudrate]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_3.png>) 

<br>

**3. DeviceNet ERROR**

{% hint style="info" %}
\.      如果 DeviceNet 电缆未提供 24V 电源，则会出现如下 ERROR。

\.      请检查是否提供 24V 电源。
{% endhint %}

![[图 1.3.7.5-4 DeviceNet Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_4.png>) 
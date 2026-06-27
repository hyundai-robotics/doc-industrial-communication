#### 1.3.7.5 DeviceNet 错误处理

<br>

请参阅 "[1.4.1 错误代码](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)"。

<br>

**1. DeviceNet 终端电阻**

{% hint style="info" %}
   - 在连接 DeviceNet 电缆时，应在终端处添加一个电阻。

   - 如果网络扫描功能无法正常工作，请检查终端电阻。

   - DeviceNet 终端电阻：120 欧姆
{% endhint %}

{% hint style="info" %}
   - 如下图所示，如果 CIFX-50 DN PCI 位于 DeviceNet 终端，请添加终端电阻。
{% endhint %}

![[Figure 1.3.7.5-1 DeviceNet 终端电阻]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_1.png>) 

{% hint style="info" %}
   - 如下图所示，如果 DeviceNet 远程 IO 位于终端，请添加终端电阻或操作 DIP 开关。
{% endhint %}

![[Figure 1.3.7.5-2 DeviceNet 终端电阻]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_2.png>) 

<br>

**2. 通信速度**

{% hint style="info" %}
   - 如果 DeviceNet 主站和从站之间的通信速度不同，网络扫描功能可能无法正常工作。

   - 如果网络扫描功能无法正常工作，请检查通信速度。
{% endhint %}

![[Figure 1.3.7.5-3 DeviceNet 波特率]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_3.png>) 

<br>

**3. DeviceNet 错误**

{% hint style="info" %}
   - 如果未向 DeviceNet 电缆提供 24V 电源，将出现以下错误。

   - 请检查 24V 电源供应。
{% endhint %}

![[Figure 1.3.7.5-4 DeviceNet 错误]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_4.png>)
## 1.3.7.5 DeviceNet Error Handling

<br>

Please refer to "[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

<br>

**1. DeviceNet termination resistor**

{% hint style="info" %}
\.      A resistor should be added at the termination when connecting the DeviceNet cable.

\.      If the Network Scan function does not work, please check the termination resistor.

\.      DeviceNet termination resistor: 120 ohms
{% endhint %}

{% hint style="info" %}
\.      As shown in the figure below, if the CIFX-50 DN PCI is at the DeviceNet termination, please add a termination resistor.
{% endhint %}

![[Figure 1.3.7.5-1 DeviceNet Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_1.png>) 

{% hint style="info" %}
\.      As shown in the figure below, if the DeviceNet Remote IO is at the termination, please add a termination resistor or operate the DIP switch.
{% endhint %}

![[Figure 1.3.7.5-2 DeviceNet Termination Resistor]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_2.png>) 

<br>

**2. Communication Speed**

{% hint style="info" %}
\.      If the communication speed differs between the DeviceNet master and slave, the Network Scan function may not work.

\.      If the Network Scan function does not work, please check the communication speed.
{% endhint %}

![[Figure 1.3.7.5-3 DeviceNet Baudrate]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_3.png>) 

<br>

**3. DeviceNet ERROR**

{% hint style="info" %}
\.      If a 24V power is not supplied to the DeviceNet cable, the following error will appear.

\.      Please check the 24V power supply.
{% endhint %}

![[Figure 1.3.7.5-4 DeviceNet Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_4.png>) 
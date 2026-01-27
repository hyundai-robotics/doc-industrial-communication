## 1.3.7.5 DeviceNet-Fehlerbehandlung

<br>

Bitte beachten Sie „[**1.4.1 FEHLERCODE**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)“.

<br>

**1. DeviceNet-Abschlusswiderstand**

{% hint style="info" %}
\.      Beim Anschluss des DeviceNet-Kabels muss am Abschluss ein Widerstand angebracht werden.

\.      Wenn der Netzwerkscan nicht funktioniert, überprüfen Sie bitte den Abschlusswiderstand.

\.      DeviceNet-Abschlusswiderstand: 120 Ohm
{% endhint %}

{% hint style="info" %}
\.      Wie in der Abbildung unten gezeigt, setzen Sie bitte einen Abschlusswiderstand, wenn sich CIFX-50 DN PCI am DeviceNet-Abschluss befindet.
{% endhint %}

![[Abbildung 1.3.7.5-1 DeviceNet-Abschlusswiderstand]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_1.png>) 

{% hint style="info" %}
\.      Wie in der Abbildung unten gezeigt, fügen Sie bitte einen Abschlusswiderstand hinzu oder betätigen Sie den DIP-Schalter, wenn sich DeviceNet-Remote-E/A am Abschluss befindet.
{% endhint %}

![[Abbildung 1.3.7.5-2 DeviceNet-Abschlusswiderstand]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_2.png>) 

<br>

**2. Kommunikationsgeschwindigkeit**

{% hint style="info" %}
\.      Wenn die Kommunikationsgeschwindigkeit zwischen DeviceNet-Master und Slave abweicht, funktioniert der Netzwerkscan möglicherweise nicht.

\.      Wenn der Netzwerkscan nicht funktioniert, überprüfen Sie bitte die Kommunikationsgeschwindigkeit.
{% endhint %}

![[Abbildung 1.3.7.5-3 DeviceNet Baudrate]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_3.png>) 

<br>

**3. DeviceNet ERROR**

{% hint style="info" %}
\.      Wenn das DeviceNet-Kabel nicht mit 24 V versorgt wird, wird der folgende Fehler (ERROR) angezeigt.

\.      Bitte überprüfen Sie die 24-V-Stromversorgung.
{% endhint %}

![[Abbildung 1.3.7.5-4 DeviceNet Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_4.png>) 
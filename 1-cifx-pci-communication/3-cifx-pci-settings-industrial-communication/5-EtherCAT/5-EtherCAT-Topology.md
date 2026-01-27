## 1.3.5.5 EtherCAT-Kabelverdrahtung (Topologie)

<br>

Im Gegensatz zu bestehenden industriellen Kommunikationssystemen gibt es bei EtherCAT Einschränkungen hinsichtlich der Kabelverdrahtung und der verwendbaren Ethernet-Ports.

**1. Ethernet-Port**

{% hint style="info" %}
\.      Beim Anschluss von EtherCAT-Master und -Slave muss Port 0 verwendet werden.
{% endhint %}

![[Abbildung 1.3.5.5-1 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
\.      Wenn 1 Slave an den Master angeschlossen ist
{% endhint %}

![[Abbildung 1.3.5.5-2 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
\.      Wenn 2 oder mehr Slaves an den Master angeschlossen sind

\.      Verbinden Sie den Slave-Port 1 mit dem nächsten Slave-Port 0.
{% endhint %}

![[Abbildung 1.3.5.5-3 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_3.png>) 

<br>

**2. Redundancy **

{% hint style="info" %}
\.      Bei Verwendung der Redundanzfunktion im Master 

\.      Verbinden Sie Port 1 des letzten Slaves und Port 1 des Masters, um eine Ringstruktur zu bilden.
{% endhint %}

![[Abbildung 1.3.5.5-4 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_4.png>) 


<br>

**3. Kabelverdrahtung ERROR**


Bitte beachten Sie „[**1.4.1 FEHLERCODE**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)“.

<br>

{% hint style="info" %}
\.      Wenn der Netzwerkscan nicht funktioniert

\.      Bitte überprüfen Sie den Port und das Kabel, die mit dem Master verbunden sind.
{% endhint %}

![[Abbildung 1.3.5.5-5 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
\.      Topology Error (Configuration Error)

\.      Bitte überprüfen Sie die Kabelverbindung zwischen Master und Slave.
{% endhint %}

![[Abbildung 1.3.5.5-6 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
\.      Topologiefehler 2 (konfiguriert normal, aber Fehler bei der Diagnose)

\.      Bitte überprüfen Sie die Kabelverbindung zwischen Master und Slave.

\.      Bitte überprüfen Sie die Kabelverbindung zwischen Slave und Slave.
{% endhint %}

![[Abbildung 1.3.5.5-7 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_7.png>)

![[Abbildung 1.3.5.5-8 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
\.      Mandatory Slave Missing Error

\.      Bitte überprüfen Sie die Kabelverbindung zwischen Slave und Slave.
{% endhint %}

![[Abbildung 1.3.5.5-9 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_9.png>)
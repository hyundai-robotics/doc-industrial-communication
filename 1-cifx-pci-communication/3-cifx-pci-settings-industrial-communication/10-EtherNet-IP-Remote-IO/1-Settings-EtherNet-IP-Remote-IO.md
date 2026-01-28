#### 1.3.10.1 EtherNet/IP – Standard-Einstellungen für die Remote-E/A-Verbindung

Befolgen Sie bitte die Schritte unter „[**1.3.1 CIFX-PCI-Slot-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)“ und fahren Sie dann mit der folgenden Methode fort.

<br>

**1. Wählen Sie EtherNet/IP Master in den Firmware-Einstellungen für die industrielle Kommunikation aus und starten Sie die Robotersteuerung neu.**

![[Abbildung 1.3.10.1-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>)

<br>

**2. Überprüfen Sie den Bereitschaftsstatus des ausgewählten Protokolls in der Überwachung der industriellen Kommunikation.**

![[Abbildung 1.3.10.1-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

**3. Schließen Sie die PCI- und Remote-E/A-Kabel usw. für die Kommunikation an und überprüfen Sie den Status.**

![[Abbildung 1.3.10.1-3 Hardware-Anschluss]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[Abbildung 1.3.10.1-4 Hardware-Anschluss]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

<br>

{% hint style="info" %}
\.      Verbinden Sie den PCI und den Remote-E/A mit einem LAN-Kabel.

\.      Stellen Sie alle DIP-Schalter des Remote-E/A auf AUS.

\.      Schließen Sie sowohl die Remote-E/A-Stromversorgung als auch die Feldstromversorgung an. (24 V DC)
{% endhint %}

<br>

{% hint style="info" %}
\.      Die werkseitige Standard-IP des Crevis M9289 Remote-E/A lautet 192.168.100.99.

\.      Die Remote-E/A-IP muss für die Kommunikationsverbindung auf 192.168.100.99 eingestellt werden.

\.      „[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)“
{% endhint %}

<br>

**4. Berühren Sie das Menü, um den Bildschirm mit den Slave-Einstellungen aufzurufen.**

**\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 2: PCI-Slave-Slot-Einstellungen > EtherNet/IP-Remote-E/A-Einstellung]**

![[Abbildung 1.3.10.1-5 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>) 

![[Abbildung 1.3.10.1-6 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>) 

<br>

{% hint style="info" %}
\.      Die IP wird als fester Wert festgelegt.

\.      Überprüfen Sie die Anzahl der Eingangs- und Ausgangs-Bytes.

\.      Die ausgewählten Eingangs- und Ausgangszahlen müssen kleiner oder gleich der Anzahl der E/As auf den in den Remote-E/A-Slots installierten Karten sein.
{% endhint %}

<br>

{% hint style="info" %}
\.      Input Module  
\.      M12DF: Digital 16 Punkte  
\.      M3534: Analog 4 Punkte  
{% endhint %}

{% hint style="info" %}
\.      Ausgabemodul  
\.      M225F: Digital 16 Punkte  
\.      M226F: Digital 16 Punkte  
\.      M2768: Digital 8 Punkte   
\.      M4534: Analog 4 Punkte  
{% endhint %}

{% hint style="info" %}
\.      Special Module  
\.      M5112 : Conveyer I/F 
{% endhint %}

<br>

**5. Starten Sie die Steuerung nach Abschluss der Einstellungen neu.**

![[Abbildung 1.3.10.1-7 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>) 

![[Abbildung 1.3.10.1-8 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
\.      Bitte starten Sie die Steuerung nach Abschluss der Einstellungen neu.
{% endhint %}

<br>

**6. Nachdem Sie sich vergewissert haben, dass die Einstellungen übernommen wurden, überprüfen Sie den Kommunikationsstatus.**

![[Abbildung 1.3.10.1-9 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>)

Informationen zum Überprüfen des Status der industriellen Kommunikation auf dem TP finden Sie unter („[**1.4 Überwachung der CIFX-PCI-Kommunikation**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)“).

![[Abbildung 1.3.10.1-10 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>)

{% hint style="info" %}
\.      Wenn keine Kommunikation hergestellt werden kann, überprüfen Sie bitte die IP-Adresse des Remote-E/A.

\.      Bitte befolgen Sie die folgenden Schritte. (Falls nicht 192.168.100.99)

\.      „[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)“
{% endhint %}

![[Abbildung 1.3.10.1-11 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>) 

![[Abbildung 1.3.10.1-12 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>) 

<br>

**7. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.**

{% hint style="info" %}
\.      **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../../../4-io-block-allocation.md)“).**
{% endhint %}
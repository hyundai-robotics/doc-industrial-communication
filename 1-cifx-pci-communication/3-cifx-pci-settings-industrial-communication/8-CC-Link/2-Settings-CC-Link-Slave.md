## 1.3.8.2 CC-Link-Slave-Einstellungen

Befolgen Sie bitte die Schritte unter „[**1.3.1 CIFX-PCI-Slot-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)“ und fahren Sie dann mit der folgenden Methode fort.

<br>

{% hint style="info" %}
\.      Informationen zum Anschluss des CC-Link-Steckers finden Sie im Folgenden.

\.      („[**1.2.2 Stecker**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)“)
{% endhint %}

<br>

**1. Bitte wählen Sie über TP in den Firmware-Einstellungen für die industrielle Kommunikation „CC-Link Slave“ aus und starten Sie die Robotersteuerung neu.**

![[Abbildung 1.3.8.4-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

**2. Überprüfen Sie den aktuellen Status der Kommunikationsprotokollbereitschaft in der Überwachung der industriellen Kommunikation.**

![[Abbildung 1.3.8.4-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Achtung]**: Wenn eine von Sycon.net festgelegte Konfigurationsdatei auf diesen PCI-Slot heruntergeladen wird, werden die TP-Einstellungen ignoriert.
{% endhint %}

<br>

**3. Berühren Sie das Menü, um den Bildschirm mit den Slave-Einstellungen aufzurufen.**
**\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 2: PCI-Slave-Slot-Einstellungen >  CC-Link Slave]**

![[Abbildung 1.3.8.4-3 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>) 

![[Abbildung 1.3.8.4-4 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

**4. Beschreibung der einzelnen Elemente**

{% hint style="info" %}
\.      [Stationsadresse]

\.      CC-Link identifiziert Slaves über die Stationsadresse. (1–64)
{% endhint %}

{% hint style="info" %}
\.      [Kommunikationsgeschwindigkeit (Baudrate)]

\.      Sie können zwischen 156, 625, 2500, 5000 und 10000 Kbit/s wählen.
{% endhint %}

{% hint style="info" %}
\.      [CC-Link Version]

\.      Version 1: E/A-Station verfügbar, Erweiterungszyklus nicht verfügbar

\.      Version 2: E/A-Station nicht verfügbar, Erweiterungszyklus verfügbar
{% endhint %}

{% hint style="info" %}
\.      [Anzahl belegter Stationen]

\.      E/A-Station: Belegt 1

\.      Remote-Gerät: 1 bis 4 wählbar 

\.      Die Größe des zugewiesenen E/A-Byte-Bereichs variiert je nach Anzahl der belegten Stationen.
{% endhint %}

{% hint style="info" %}
\.      [Extension Cycle]

\.      Verfügbar in Version 2

\.      Remote-Gerät: Einzeln (1x), doppelt (2x), vierfach (4x), achtfach (8x) wählbar 

\.      Die Größe des zugewiesenen E/A-Byte-Bereichs variiert je nach Erweiterungszyklus.
{% endhint %}

<br>

{% hint style="info" %}
\.      **Informationen zum E/A-Byte-Bereich finden Sie unter dem folgenden Link.**

\.      **(„[**1.3.8.1 CC-Link-Slave-Spezifikationen**](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md)“)**
{% endhint %}

<br>

**5. Überprüfen Sie nach Abschluss der Einstellungen den Kommunikationsstatus gemäß dem folgenden Verfahren.**

Informationen zum Überprüfen des Status der industriellen Kommunikation auf dem TP finden Sie unter („[**1.4 Überwachung der CIFX-PCI-Kommunikation**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)“).

<br>

**6. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.**

{% hint style="info" %}
\.      **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../../../4-io-block-allocation.md)“).**
{% endhint %}
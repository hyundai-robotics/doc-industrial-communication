#### 1.3.4.4 PROFINET IO-Geräteeinstellungen

Befolgen Sie bitte die Schritte unter „[**1.3.1 CIFX-PCI-Slot-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)“ und fahren Sie dann mit der folgenden Methode fort.

<br>

{% hint style="info" %}
   **[PROFINET IO-Geräte-GSDML-Datei herunterladen]**

   - Bitte beachten Sie „[**5. Beschreibungsdatei für Slave-Geräte**](../../../5-slave-config-file.md)“.
{% endhint %}

<br>

**1. Wählen Sie mithilfe von TP in den Firmware-Einstellungen für die industrielle Kommunikation „PROFINET IO Slave“ aus und starten Sie die Robotersteuerung neu.**

![[Abbildung 1.3.4.4-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_1.png>) 

<br>

**2. Überprüfen Sie den aktuellen Status der Kommunikationsprotokollbereitschaft in der Überwachung der industriellen Kommunikation.**

![[Abbildung 1.3.4.4-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Achtung]**: Wenn eine von Sycon.net festgelegte Konfigurationsdatei auf diesen PCI-Slot heruntergeladen wird, werden die TP-Einstellungen ignoriert.
{% endhint %}

<br>

**3. Berühren Sie das Menü, um den Bildschirm mit den Slave-Einstellungen aufzurufen.**
**\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 2: PCI-Slave-Slot-Einstellungen >  PROFINET IO Slave]**

![[Abbildung 1.3.4.4-3 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[Abbildung 1.3.4.4-4 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

**4. Beschreibung der einzelnen Elemente**

{% hint style="info" %}
   [Station Name]

   - PROFINET IO identifiziert Slaves über die Stationsadresse.

   - Benennungsregel
      - Gerätenamen, die über PROFINET IO verbunden sind, dürfen nicht doppelt vorkommen.  
      - Namen können bis zu 240 Zeichen lang sein.  
      - Die Sonderzeichen „.“ und „-“ dürfen verwendet werden.  
      - Englische Kleinbuchstaben und Zahlen dürfen verwendet werden.  
      - Namen müssen mit englischen Kleinbuchstaben oder Zahlen beginnen und enden.  
{% endhint %}

{% hint style="info" %}
   [Eingangsbytes]

   - Eingangsbytes: Legen Sie die Datengröße für die Eingabe von Master -> Slave fest.
{% endhint %}

{% hint style="info" %}
   [Ausgangsbytes]

   - Ausgangsbytes: Legen Sie die Datengröße für die Ausgabe von Slave -> Master fest.
{% endhint %}

<br>

{% hint style="info" %}
   [**Bei der Einstellung von Slot im Master**]

   - Master Input (32byte)  <--  Slave Output (32bytes)

   - Master Output (256bytes = 64bytes * 4)  -->  Slave Input (256bytes)

   - 4, 8, 16, 32, 64 Bytes -> Geben Sie den Slot für jedes Byte an
   - 128, 256 Bytes -> Geben Sie mehrere 64-Byte-Slots an (2, 4)

   - Der Eingangsslot befindet sich vor dem Ausgangsslot.
{% endhint %}

<br>

![[Abbildung 1.3.4.4-5 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_5.png>) 


<br>

**5. Überprüfen Sie nach Abschluss der Einstellungen den Kommunikationsstatus gemäß dem folgenden Verfahren.**

Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („[**1.4 Überwachung der CIFX-PCI-Kommunikation**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)“).

![[Abbildung 1.3.4.4-6 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_6.png>) 

<br>

**6. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.**

{% hint style="info" %}
   **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../../../4-io-block-allocation.md)“).**
{% endhint %}
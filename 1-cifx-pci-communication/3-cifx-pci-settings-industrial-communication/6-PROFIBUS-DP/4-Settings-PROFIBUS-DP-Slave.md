#### 1.3.6.4 PROFIBUS-DP-Slave-Einstellungen

Befolgen Sie bitte die Schritte unter „[**1.3.1 CIFX-PCI-Slot-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)“ und fahren Sie dann mit der folgenden Methode fort.

<br>

{% hint style="info" %}
   **[PROFIBUS-DP-Slave-GSD-Datei herunterladen]**

   - Bitte beachten Sie „[**5. Beschreibungsdatei für Slave-Geräte**](../../../5-slave-config-file.md)“.
{% endhint %}

<br>

**1. Wählen Sie mithilfe von TP in den Firmware-Einstellungen für die industrielle Kommunikation „PROFIBUS-DP Slave“ aus und starten Sie die Robotersteuerung neu.**

![[Abbildung 1.3.6.4-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

**2. Überprüfen Sie den aktuellen Status der Kommunikationsprotokollbereitschaft in der Überwachung der industriellen Kommunikation.**

![[Abbildung 1.3.6.4-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Achtung]**: Wenn eine von Sycon.net festgelegte Konfigurationsdatei auf diesen PCI-Slot heruntergeladen wird, werden die TP-Einstellungen ignoriert.
{% endhint %}

<br>

**3. Berühren Sie das Menü, um den Bildschirm mit den Slave-Einstellungen aufzurufen.**
**\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 2: PCI-Slave-Slot-Einstellungen > PROFIBUS-DP Slave]**

![[Abbildung 1.3.6.4-3 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[Abbildung 1.3.6.4-4 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

<br>

**4. Beschreibung der einzelnen Elemente**

{% hint style="info" %}
   [Station Address]

   - PROFIBUS-DP identifiziert Slaves über die Stationsadresse.
{% endhint %}

{% hint style="info" %}
   [Eingangsbytes]

   - Eingangsbytes: Legen Sie die Datengröße für die Eingabe von Master -> Slave fest.
{% endhint %}

{% hint style="info" %}
   [Ausgangsbytes]

   - Ausgangsbytes: Legen Sie die Datengröße für die Ausgabe von Slave -> Master fest.
{% endhint %}

{% hint style="info" %}
   [**Bei der Einstellung des Moduls im Master**]

   - Die Module müssen im Master so festgelegt werden, dass sie mit der eingestellten Byteanzahl übereinstimmen.

   - Reihenfolge: Master-Eingang (64–1) -> Master-Ausgang (64–1)

   - Bsp.) Master Input 109 Bytes  <---  Slave Output 109 Bytes   
         - Input 109 Bytes : 64Byte + 32Byte + 8Byte + 4Byte + 1 Byte

   - Bsp.) Master Output 120 Bytes  --->  Slave Input 120 Bytes   
         - Output 120 Bytes : 64Byte + 32Byte + 16Byte + 8Byte


   - Bsp.) Master Input 12 Bytes  <---  Slave Output 12 Bytes   
         - Eingang 12 Bytes : 8 Byte + 4 Byte

   - Bsp.) Master-Ausgang 200 Bytes  --->  Slave-Eingang 200 Bytes   
         - Ausgang 200 Bytes : 64 Byte + 64 Byte + 64 Byte + 8 Byte

   - Das Eingangsmodul befindet sich vor dem Ausgangsmodul.
{% endhint %}

![[Abbildung 1.3.6.4-5 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>)


<br>

**5. Überprüfen Sie nach Abschluss der Einstellungen den Kommunikationsstatus gemäß dem folgenden Verfahren.**

Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („[**1.4 Überwachung der CIFX-PCI-Kommunikation**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)“).

![[Abbildung 1.3.6.4-6 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>)

<br>

**6. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.**

{% hint style="info" %}
   **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../../../4-io-block-allocation.md)“).**
{% endhint %}
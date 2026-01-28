#### 1.3.9.2 CC-Link IE Field Slave-Einstellungen

Befolgen Sie bitte die Schritte unter „[**1.3.1 CIFX-PCI-Slot-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)“ und fahren Sie dann mit der folgenden Methode fort.


<br>

**1. Wählen Sie über TP in den Einstellungen der industriellen Kommunikationsfirmware „CC-Link IE Field Slave“ aus und starten Sie die Robotersteuerung neu.**

![[Abbildung 1.3.9.2-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_1.png>)

<br>

**2. Überprüfen Sie den aktuellen Status der Kommunikationsprotokollbereitschaft in der Überwachung der industriellen Kommunikation.**

![[Abbildung 1.3.9.4-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Achtung]**: Wenn eine von Sycon.net festgelegte Konfigurationsdatei auf diesen PCI-Slot heruntergeladen wird, werden die TP-Einstellungen ignoriert.
{% endhint %}

<br>

**3. Berühren Sie das Menü, um den Bildschirm mit den Slave-Einstellungen aufzurufen.**
**\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 2: PCI-Slave-Slot-Einstellungen >  CC-Link IE Field Slave]**

![[Abbildung 1.3.9.4-3 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>) 

![[Abbildung 1.3.9.4-4 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>) 

<br>

**4. Beschreibung der einzelnen Elemente**

{% hint style="info" %}
   [Network Number]

   - CC-Link IE Field-Netzwerknummer (1–239)
{% endhint %}

{% hint style="info" %}
   [Station Address]

   - Geräte-ID innerhalb des verbundenen Netzwerks (1–120)
{% endhint %}

{% hint style="info" %}
   [IO Type]

   - Der E/A-Typ wird durch die Einstellungen des Master-Geräts bestimmt   
      - Gemischt: Eingang und Ausgang verwenden unterschiedliche Indizes (unterschiedliche Adressen)   
      - Eingang: Nur Eingang   
      - Ausgang: Nur Ausgang   
      - FrontBackMixture: Eingang und Ausgang verwenden denselben Index (dieselbe Adresse)   
{% endhint %}

{% hint style="info" %}
   [Gerätetyp]

   - Die maximal einstellbare E/A-Größe hängt vom Gerätetyp ab.

   - Intelligent Device Station   
      - RY, RX (max): 256 bytes   
      - RWw, RWr (max.): 1024 Wörter

   - Remote-Gerätestation   
      - RY, RX (max.): 16 Byte   
      - RWw, RWr (max.): 64 Wörter
{% endhint %}

{% hint style="info" %}
   [IO Size]

   - Master -> Slave   
      - RWw (word data)   
      - RY (bit data)   

   - Slave -> Master   
      - RWr (Wortdaten)   
      - RX (Bitdaten)  
{% endhint %}

<br>

**5. Überprüfen Sie nach Abschluss der Einstellungen den Kommunikationsstatus gemäß dem folgenden Verfahren.**

Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („[**1.4 Überwachung der CIFX-PCI-Kommunikation**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)“).

<br>

**6. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.**

{% hint style="info" %}
   **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../../../4-io-block-allocation.md)“).**
{% endhint %}

<br>

![[Abbildung 1.3.9.4-5 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>) 
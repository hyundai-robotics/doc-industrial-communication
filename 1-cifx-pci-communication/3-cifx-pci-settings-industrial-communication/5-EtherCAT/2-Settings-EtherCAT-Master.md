#### 1.3.5.2 EtherCAT-Master-Einstellungen

Bitte befolgen Sie die Anweisungen unter „[**1.3.1 CIFX-PCI-Steckplatz-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)“ und „[**1.3.2 SYCON.NET-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)“ und fahren Sie dann mit der folgenden Methode fort.

<br>

{% hint style="info" %}
   - Wenn Sie SYCON.net verwenden und die Erläuterungen im Handbuch nicht ausreichen, ziehen Sie bitte die Funktion „[**1.3.2 SYCON.NET-Hilfe**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)“ zu Rate.
{% endhint %}

<br>

**1. Wählen Sie in den Firmware-Einstellungen für die industrielle Kommunikation „EtherCAT-Master“ aus und starten Sie die Robotersteuerung neu.**

![[Abbildung 1.3.5.2-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_1.png>) 

<br>

**2. Überprüfen Sie den Bereitschaftsstatus des ausgewählten Protokolls in der Überwachung der industriellen Kommunikation.**

![[Abbildung 1.3.5.2-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_2.png>) 

<br>

**3. Wählen Sie mithilfe von Sycon.net das EtherCAT-Master-PCI-Gerät aus.**

![[Abbildung 1.3.5.2-3 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_3.png>)
![[Abbildung 1.3.5.2-4 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_4.png>) 

<br>

**4. Scannen Sie das PCI-Gerät und wenden Sie EtherCAT-Master an.**

![[Abbildung 1.3.5.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_5.png>) 

<br>

**5. Laden Sie die Einstellungen herunter.**

![[Abbildung 1.3.5.2-6 EtherCAT Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_6.png>) 

<br>

**6. Bereiten Sie die Slave-Module für die Verbindung mit dem EtherCAT-Master vor.**
   * In diesem Beispiel verwenden wir Crevis M9386 EtherCAT-Slave.
   * Bitte versorgen Sie das Modul mit Systemstrom und Feldstrom, um es zu aktivieren.

![[Abbildung 1.3.5.2-7 Crevis M9386]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_7.png>) 

<br>

**7. Station-Adresse des Slave-Geräts**

{% hint style="info" %}
   - Die Station-Adresse des EtherCAT-Slave-Geräts wird im Master festgelegt.
{% endhint %}

<br>

**8. Registrieren Sie die XML-Datei des Slave-Geräts.**

{% hint style="info" %}
   - Für die Verwendung von Geräten, die nicht in Sycon.net registriert sind, ist eine XML-Datei erforderlich.

   - Die XML-Datei für das Gerät M9386 kann von der Crevis-Website heruntergeladen werden.
{% endhint %}

![[Abbildung 1.3.5.2-8 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_8.png>)

{% hint style="info" %}
   - Registrieren Sie die heruntergeladene XML-Datei in Sycon.net.

   - Bitte überprüfen Sie bei der Registrierung von XML-Dateien das industrielle Kommunikationsprotokoll (EtherCAT).
{% endhint %}

![[Abbildung 1.3.5.2-9 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_9.png>)

<br>

![[Abbildung 1.3.5.5-10 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_10.png>)

<br>

![[Abbildung 1.3.5.2-11 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_11.png>)

<br>

![[Abbildung 1.3.5.2-12 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_12.png>)


<br>

**9. Network Scan**

{% hint style="warning" %}
   **EtherCAT hat die verwendbaren Kabelverkabelungen und Anschlüsse festgelegt.**

   **Für eine reibungslose Kommunikationsverbindung überprüfen Sie bitte („[**1.3.5.5 EtherCAT-Kabelverdrahtung**](../5-EtherCAT/5-EtherCAT-Topology.md)“).**
{% endhint %}

{% hint style="info" %}
   - EtherCAT Master unterstützt die Netzwerkscan-Funktion.
{% endhint %}

{% hint style="info" %}
   - Klicken Sie mit der rechten Maustaste auf das EtherCAT Master-Gerät und wählen Sie „Netzwerkscan“.
{% endhint %}

![[Abbildung 1.3.5.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_13.png>)

{% hint style="warning" %}
   - Wenn die XML-Datei nicht registriert ist, werden die Slave-Informationen bei der Durchführung eines Netzwerkscans angezeigt, jedoch ist eine Registrierung nicht möglich.
{% endhint %}

{% hint style="info" %}
   - Wenn die XML-Datei ordnungsgemäß registriert ist, können Slave-Geräte über den Netzwerkscan hinzugefügt werden.
{% endhint %}

![[Abbildung 1.3.5.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_14.png>)

<br>

**10. Konfiguration des Slave-Geräts**

{% hint style="info" %}
   - Klicken Sie auf „Trennen“ des Master-Geräts für die Konfiguration des Slave-Geräts.
{% endhint %}

![[Abbildung 1.3.5.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - Doppelklicken Sie auf das Slave-Gerät.
{% endhint %}

![[Abbildung 1.3.5.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_16.png>)

{% hint style="info" %}
   - Fügen Sie an M9386 angeschlossene Slots für die EtherCAT-Slave-Einstellungen hinzu.

   - Slot 1 : M7001  
   - Slot 2 : M12DF  
   - Slot 3 : M225F  
{% endhint %}

![[Abbildung 1.3.5.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_17.png>)

![[Abbildung 1.3.5.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_18.png>)


<br>

**11. Konfiguration des Master-Geräts**

{% hint style="info" %}
   - Doppelklicken Sie auf das Master-Gerät.
{% endhint %}

![[Abbildung 1.3.5.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - Synchronisierung: Wählen Sie „Freerun / DC (Distributed Clocks)“ („Verteilte Uhren“)

   - Ob Redundanz verwendet werden soll (kann nicht zusammen mit „Distributed Clocks“ verwendet werden)

   - Buszykluszeit: Mindestens 250 us unterstützt (1 ms oder mehr empfohlen)
{% endhint %}

<br>

{% hint style="info" %}
   - Sie können die Stationsadresse für jeden Slave festlegen.
{% endhint %}

![[Abbildung 1.3.5.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - Überprüfen Sie die zugewiesenen E/A und die Startadresse für jeden Slave-Slots in der Adresstabelle.
{% endhint %}

![[Abbildung 1.3.5.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_21.png>)


{% hint style="info" %}
   - Fahren Sie nach Abschluss der Einstellungen mit dem Herunterladen fort.
{% endhint %}

![[Abbildung 1.3.5.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_22.png>)

<br>

**12. Überprüfen Sie den Kommunikationsstatus**

{% hint style="info" %}
   - Überprüfen Sie den Kommunikationsstatus in Sycon.net und TP.

   - Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („[**1.4 Überwachen der CIFX-PCI-Kommunikation**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)“).
{% endhint %}

{% hint style="info" %}
   - Doppelklicken Sie auf das angeschlossene Master-Gerät, um den Kommunikationsstatus zu überprüfen.
{% endhint %}

![[Abbildung 1.3.5.2-23 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_23.png>)

![[Abbildung 1.3.5.2-24 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - Mit der Diagnosefunktion von Sycon.net können Sie den Kommunikationsstatus und den Status der E/A-Ein- und Ausgänge überwachen.
{% endhint %}

![[Abbildung 1.3.5.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_25.png>)

<br>

**13. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.**

{% hint style="info" %}
   **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../../../4-io-block-allocation.md)“).**
{% endhint %}
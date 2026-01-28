#### 1.3.7.2 DeviceNet-Master-Einstellungen

Bitte befolgen Sie die Anweisungen unter „[**1.3.1 CIFX-PCI-Steckplatz-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)“ und „[**1.3.2 SYCON.NET-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)“ und fahren Sie dann mit der folgenden Methode fort.

<br>

{% hint style="info" %}
\.      Wenn Sie SYCON.net verwenden und die Erläuterungen im Handbuch nicht ausreichen, ziehen Sie bitte die Funktion „[**1.3.2 SYCON.NET-Hilfe**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)“ zu Rate.
{% endhint %}

<br>

{% hint style="info" %}
\.      Informationen zum Anschluss des DeviceNet-Steckers finden Sie im Folgenden.

\.      („[**1.2.2 Stecker**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)“)
{% endhint %}

<br>

**1. Wählen Sie DeviceNet Master in den Firmware-Einstellungen für die industrielle Kommunikation aus und starten Sie die Robotersteuerung neu.**

![[Abbildung 1.3.7.2-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_1.png>) 

<br>

**2. Überprüfen Sie den Bereitschaftsstatus des ausgewählten Protokolls in der Überwachung der industriellen Kommunikation.**

![[Abbildung 1.3.7.2-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_2.png>) 

<br>

**3. Wählen Sie mit Sycon.net das DeviceNet-Master-PCI-Gerät aus.**

![[Abbildung 1.3.7.2-3 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_3.png>)
![[Abbildung 1.3.7.2-4 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_4.png>) 

<br>

**4. Scannen Sie das PCI-Gerät und wenden Sie „DeviceNet-Master“ an.**

![[Abbildung 1.3.7.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_5.png>) 

<br>

**5. Stellen Sie die Kommunikationsgeschwindigkeit ein.**

{% hint style="warning" %}
\.      Wenn die Kommunikationsgeschwindigkeit von Master und Slave unterschiedlich ist, funktioniert der Netzwerkscan nicht ordnungsgemäß.
{% endhint %}

![[Abbildung 1.3.7.2-6 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_6.png>) 

<br>

**6. Laden Sie die Einstellungen herunter.**

![[Abbildung 1.3.7.2-7 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_7.png>) 

<br>

**7. Bereiten Sie die Slave-Module für die Verbindung mit dem DeviceNet-Master vor.**
   * In diesem Beispiel verwenden wir Crevis NA-9211 DeviceNet-Slave.
   * Bitte versorgen Sie das Modul mit Systemstrom und Feldstrom, um es zu aktivieren.

![[Abbildung 1.3.7.2-8 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_8.png>) 

<br>

**8. Einstellungen des Slave-Geräts**

{% hint style="info" %}
\.      Stellen Sie die MAC-ID, die Kommunikationsgeschwindigkeit und den Abschlusswiderstand des DeviceNet-Slave-Geräts ein.
{% endhint %}

![[Abbildung 1.3.7.2-9 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_9.png>) 

![[Abbildung 1.3.7.2-10 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_10.png>)

{% hint style="info" %}
\.      [Beispiel-Einstellungen]

\.      Abschlusswiderstand: Verwendung mit im Kabel installiertem Abschlusswiderstand (Abschluss-DIP-Schalter AUS)

\.      MAC-ID (Stationsnummer): Auf 4 einstellen (nur DIP-Schalter 3 EIN)

\.      Kommunikationsgeschwindigkeit (Baudrate): Auf „Auto“ einstellen (DIP-Schalter 7 und 8 EIN)
{% endhint %}

<br>

**9. Registrieren Sie die EDS-Datei des Slave-Geräts.**

{% hint style="info" %}
\.      Für die Verwendung von Geräten, die nicht in Sycon.net registriert sind, ist eine EDS-Datei erforderlich.

\.      Die EDS-Datei für das Gerät NA-9211 kann von der Crevis-Website heruntergeladen werden.
{% endhint %}

![[Abbildung 1.3.7.2-11 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_11.png>)

{% hint style="info" %}
\.      Registrieren Sie alle heruntergeladenen EDS-Dateien in Sycon.net.

\.      Bitte überprüfen Sie bei der Registrierung von EDS-Dateien das industrielle Kommunikationsprotokoll (DeviceNet).
{% endhint %}

![[Abbildung 1.3.7.2-12 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_12.png>)

<br>

![[Abbildung 1.3.7.5-13 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_13.png>)



<br>

**10. Netzwerkscan**

{% hint style="warning" %}
\.      **Überprüfen Sie bei der Durchführung eines Netzwerkscans unbedingt die folgenden Punkte.**

\.      **(1) Ob das Kabel angeschlossen ist.**  
\.      **(2) Ob ein Abschlusswiderstand angeschlossen oder ein Abschluss-DIP-Schalter verwendet werden soll.**  
\.      **(3) Ob die Kommunikationsgeschwindigkeit zwischen Master und Slave festgelegt ist**  

\.      **Für eine reibungslose Kommunikationsverbindung überprüfen Sie bitte („[**1.3.7.5 DeviceNet-Fehlerbehandlung**](../7-DeviceNet/5-Error-DeviceNet.md)“).**
{% endhint %}

{% hint style="info" %}
\.      DeviceNet Master unterstützt die Netzwerkscan-Funktion.
{% endhint %}

{% hint style="info" %}
\.      Klicken Sie mit der rechten Maustaste auf das DeviceNet Master-Gerät und wählen Sie „Netzwerkscan“.
{% endhint %}

![[Abbildung 1.3.7.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      Wenn die EDS-Datei nicht registriert ist, werden die Slave-Informationen bei der Durchführung eines Netzwerkscans angezeigt, jedoch ist eine Registrierung nicht möglich.
{% endhint %}

{% hint style="info" %}
\.      Wenn die EDS-Datei ordnungsgemäß registriert ist, können Slave-Geräte über den Netzwerkscan hinzugefügt werden.
{% endhint %}

![[Abbildung 1.3.7.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_15.png>)

![[Abbildung 1.3.7.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_16.png>)

<br>

**11. Konfiguration des Slave-Geräts**

{% hint style="info" %}
\.      Klicken Sie auf „Trennen“ des Master-Geräts für die Konfiguration des Slave-Geräts.
{% endhint %}

![[Abbildung 1.3.7.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
\.      Doppelklicken Sie auf das Slave-Gerät.
{% endhint %}

![[Abbildung 1.3.7.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_18.png>)


<br>

{% hint style="info" %}
\.      Legen Sie den Verbindungstyp des Slave-Geräts fest.

\.      Wählen Sie die Nachrichtenübertragungsmethode für die DeviceNet-Kommunikationsverbindung aus.

\.      **Wenn UCMM nicht aktiviert ist, wird UCMM-Gruppe 2 als Standardwert festgelegt.**   

\.      UCMM GROUP 1 : IO Message   
\.      UCMM-GRUPPE 2: Meldung zur Master-Slave-Verbindung während der Netzwerkinitialisierung (Standardeinstellung)   
\.      UCMM-GRUPPE 3: Explizite Nachricht   

\.      Für bestimmte Geräte kann UCMM-Gruppe 3 verwendet werden. Bitte überprüfen Sie daher die Produktspezifikationen, bevor Sie fortfahren.
{% endhint %}

![[Abbildung 1.3.7.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_19.png>)

<br>

{% hint style="info" %}
\.      Crevis NA-9211 fährt ohne Überprüfung von UCMM fort. (Verwendet den Standardwert von Gruppe 2)
{% endhint %}

![[Abbildung 1.3.7.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_20.png>)

<br>


{% hint style="info" %}
\.      Überprüfen Sie die DeviceNet-Slave-Einstellungen.

\.      Ausgang: ST-2318 (1 Byte)  
\.      Eingang: ST-1218 (1 Byte)  
{% endhint %}

<br>

{% hint style="info" %}
\.      Erforderliche Einstellungen je nach Kommunikationsmethode (Abfrage, Zustandsänderung, zyklisch, Bit-Strobe)  
{% endhint %}

<br>

![[Abbildung 1.3.7.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_21.png>)

<br>

{% hint style="info" %}
\.      [Production Inhibit Time]

\.      Legen Sie den Zyklus für die E/A-Datengenerierung des Slave-Geräts (ms) fest.  
\.  
\.      Beispiel) 10 ms: E/A-Daten werden alle 10 ms generiert.  
\.      Beispiel) 0 ms: Der Slave generiert E/A-Daten so schnell wie möglich.  

\.      Je kürzer der Zyklus, desto größer kann die Belastung des Slave-Geräts sein. (Die Spezifikationen müssen für jeden Slave überprüft werden.) 
{% endhint %}

<br>

{% hint style="info" %}
\.      [Expected Packet Rate]

\.      Legen Sie die Zeit für die Aktualisierung der E/A-Daten zwischen Master und Slave fest  
{% endhint %}

<br>

![[Abbildung 1.3.7.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_22.png>)



<br>

**12. Konfiguration des Master-Geräts**

{% hint style="info" %}
\.      Doppelklicken Sie auf das Master-Gerät.
{% endhint %}

![[Abbildung 1.3.7.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      Legen Sie die DeviceNet-Kommunikationsgeschwindigkeit fest. (An die Kommunikationsgeschwindigkeit des Slaves anpassen)
{% endhint %}

![[Abbildung 1.3.7.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.      Überprüfen Sie die zugewiesenen E/A und die Startadresse für jeden Slave-Slots in der Adresstabelle.
{% endhint %}

![[Abbildung 1.3.7.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      Legen Sie fest, ob die Quick-Connect-Funktion verwendet werden soll.
{% endhint %}

![[Abbildung 1.3.7.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_26.png>)


{% hint style="info" %}
\.      Fahren Sie nach Abschluss der Einstellungen mit dem Herunterladen fort.
{% endhint %}

![[Abbildung 1.3.7.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_27.png>)

<br>

**13. Überprüfen Sie den Kommunikationsstatus**

{% hint style="info" %}
\.        Überprüfen Sie den Kommunikationsstatus in Sycon.net und TP.

\.        Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („[**1.4 Überwachen der CIFX-PCI-Kommunikation**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)“).
{% endhint %}

{% hint style="info" %}
\.      Doppelklicken Sie auf das angeschlossene Master-Gerät, um den Kommunikationsstatus zu überprüfen.
{% endhint %}

![[Abbildung 1.3.7.2-28 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_28.png>)

![[Abbildung 1.3.7.2-29 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.        Mit der Diagnosefunktion von Sycon.net können Sie den Kommunikationsstatus und den Status der E/A-Ein- und Ausgänge überwachen.
{% endhint %}

![[Abbildung 1.3.7.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_30.png>)

<br>

**14. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.**

{% hint style="info" %}
\.      **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../../../4-io-block-allocation.md)“).**
{% endhint %}
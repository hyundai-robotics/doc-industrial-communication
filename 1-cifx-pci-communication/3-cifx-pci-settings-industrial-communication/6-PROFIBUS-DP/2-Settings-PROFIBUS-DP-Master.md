# 1.3.6.2 PROFIBUS-DP-Master-Einstellungen


Bitte befolgen Sie die Anweisungen unter „[**1.3.1 CIFX-PCI-Steckplatz-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)“ und „[**1.3.2 SYCON.NET-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)“ und fahren Sie dann mit der folgenden Methode fort.

<br>

{% hint style="info" %}
\.      Wenn Sie SYCON.net verwenden und die Erläuterungen im Handbuch nicht ausreichen, ziehen Sie bitte die Funktion „[**1.3.2 SYCON.NET-Hilfe**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)“ zu Rate.
{% endhint %}

<br>

##### 1. Wählen Sie in den Einstellungen der industriellen Kommunikationsfirmware „PROFIBUS-DP Master“ aus und starten Sie die Robotersteuerung neu.

![[Abbildung 1.3.6.2-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

##### 2. Überprüfen Sie den Bereitschaftsstatus des ausgewählten Protokolls in der Überwachung der industriellen Kommunikation.

![[Abbildung 1.3.6.2-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_2.png>) 

<br>

##### 3. Wählen Sie mit Sycon.net das PROFIBUS-DP-Master-PCI-Gerät aus.

![[Abbildung 1.3.6.2-3 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[Abbildung 1.3.6.2-4 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

##### 4. Scannen Sie das PCI-Gerät und wenden Sie „PROFIBUS-DP Master“ an.

![[Abbildung 1.3.6.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>


##### 5. Laden Sie die Einstellungen herunter.

![[Abbildung 1.3.6.2-6 PROFIBUS-DP Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

##### 6. Bereiten Sie die Slave-Module für die Verbindung mit dem PROFIBUS-DP-Master vor.
   * In diesem Beispiel verwenden wir Crevis GN-9222 PROFIBUS-DP Slave.
   * Bitte versorgen Sie das Modul mit Systemstrom und Feldstrom, um es zu aktivieren.

![[Abbildung 1.3.6.2-7 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_7.png>) 


<br>

##### 7. Einstellungen des Slave-Geräts

{% hint style="info" %}
\.      Legen Sie die Knotennummer und den Abschluss des PROFIBUS-DP-Slave-Geräts fest.
{% endhint %}

![[Abbildung 1.3.6.2-8 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_8.png>) 


{% hint style="info" %}
\.      Abschluss: Legen Sie den Abschluss mithilfe des DIP-Schalters fest (Beispiel: Abschlussverarbeitung aktiviert).

\.      Knoten-ID (Stationsnummer): Legen Sie diese mithilfe des DIP-Schalters fest (Beispiel: Knoten 3).
{% endhint %}

<br>

##### 8. Registrieren Sie die GSD-Datei des Slave-Geräts.

{% hint style="info" %}
\.      Für die Verwendung von Geräten, die nicht in Sycon.net registriert sind, ist eine GSD-Datei erforderlich.

\.      Die GSD-Datei für das Gerät GN-9222 kann von der Crevis-Website heruntergeladen werden.
{% endhint %}

![[Abbildung 1.3.6.2-9 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      Registrieren Sie die heruntergeladene GSD-Datei in Sycon.net.

\.      Überprüfen Sie bei der Registrierung von GSD-Dateien das industrielle Kommunikationsprotokoll (PROFIBUS-DP).
{% endhint %}

![[Abbildung 1.3.6.2-10 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_10.png>)

<br>

![[Abbildung 1.3.6.5-11 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_11.png>)

![[Abbildung 1.3.6.5-12 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_12.png>)



<br>

##### 9. Network Scan

{% hint style="warning" %}
\.      **Überprüfen Sie bei der Durchführung eines Netzwerkscans unbedingt die folgenden Punkte.**

\.      **(1) Ob das Kabel angeschlossen ist.**  
\.      **(2) Ob der Abschluss-DIP-Schalter verwendet wird.**  
{% endhint %}

{% hint style="info" %}
\.      Der PROFIBUS-DP-Master unterstützt die Netzwerkscan-Funktion.
{% endhint %}

{% hint style="info" %}
\.      Klicken Sie mit der rechten Maustaste auf das PROFIBUS-DP-Master-Gerät und wählen Sie „Netzwerkscan“.
{% endhint %}

![[Abbildung 1.3.6.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      Wenn die GSD-Datei nicht registriert ist, werden die Slave-Informationen bei der Durchführung eines Netzwerkscans angezeigt, jedoch ist eine Registrierung nicht möglich.
{% endhint %}

{% hint style="info" %}
\.      Wenn die GSD-Datei ordnungsgemäß registriert ist, können Slave-Geräte über den Netzwerkscan hinzugefügt werden.
{% endhint %}

![[Abbildung 1.3.6.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

##### 10. Konfiguration des Slave-Geräts

{% hint style="info" %}
\.      Klicken Sie auf „Trennen“ des Master-Geräts für die Konfiguration des Slave-Geräts.
{% endhint %}

![[Abbildung 1.3.6.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Doppelklicken Sie auf das Slave-Gerät.
{% endhint %}

![[Abbildung 1.3.6.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      Überprüfen Sie die PROFIBUS-DP-Slave-Einstellungen.

\.      Steckplatz 1 : GN-9222  
\.      Steckplatz 2 : GT-12DF (Eingang 2 Byte)  
\.      Steckplatz 3 : GT-227F (Ausgang 2 Byte)  
\.      Steckplatz 4 : GT-3154 (Eingang 8 Byte)  
\.      Steckplatz 5 : GT-4254 (Ausgang 8 Byte)  
{% endhint %}

![[Abbildung 1.3.6.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_17.png>)

<br>

![[Abbildung 1.3.6.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_18.png>)


<br>

##### 11. Konfiguration des Master-Geräts

{% hint style="info" %}
\.      Doppelklicken Sie auf das Master-Gerät.
{% endhint %}

![[Abbildung 1.3.6.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_19.png>)


{% hint style="info" %}
\.      Legen Sie die PROFIBUS-DP-Kommunikationsgeschwindigkeit fest.

\.      9,6 – 12000 Kbit/s 
{% endhint %}

![[Abbildung 1.3.6.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Bitte überprüfen Sie, ob die Slot-Informationen des Slave-Geräts im Master-Gerät korrekt sind.
{% endhint %}

![[Abbildung 1.3.6.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
\.      Überprüfen Sie die zugewiesenen E/A und die Startadresse für jeden Slave-Slots in der Adresstabelle.
{% endhint %}

![[Abbildung 1.3.6.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
\.      Überprüfen Sie, ob sich jedes Gerät in der Stationstabelle im aktiven Status befindet.
{% endhint %}

![[Abbildung 1.3.6.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      Fahren Sie nach Abschluss der Einstellungen mit dem Herunterladen fort.
{% endhint %}

![[Abbildung 1.3.6.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

##### 12. Überprüfen Sie den Kommunikationsstatus

{% hint style="info" %}
\.        Überprüfen Sie den Kommunikationsstatus in Sycon.net und TP.

\.        Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („[**1.4 Überwachen der CIFX-PCI-Kommunikation**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)“).
{% endhint %}

{% hint style="info" %}
\.      Doppelklicken Sie auf das angeschlossene Master-Gerät, um den Kommunikationsstatus zu überprüfen.
{% endhint %}

![[Abbildung 1.3.6.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[Abbildung 1.3.6.2-26 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Mit der Diagnosefunktion von Sycon.net können Sie den Kommunikationsstatus und den Status der E/A-Ein- und Ausgänge überwachen.
{% endhint %}

![[Abbildung 1.3.6.2-27 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_27.png>)

<br>

##### 13. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.

{% hint style="info" %}
\.      **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../../../4-io-block-allocation.md)“).**
{% endhint %}

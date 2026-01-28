#### 1.3.4.2 PROFINET IO-Controller-Einstellungen

Bitte befolgen Sie die Anweisungen unter „[**1.3.1 CIFX-PCI-Steckplatz-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)“ und „[**1.3.2 SYCON.NET-Einstellungen**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)“ und fahren Sie dann mit der folgenden Methode fort.

<br>

{% hint style="info" %}
   - Wenn Sie SYCON.net verwenden und die Erläuterungen im Handbuch nicht ausreichen, ziehen Sie bitte die Funktion „[**1.3.2 SYCON.NET-Hilfe**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)“ zu Rate.
{% endhint %}

<br>

**1. Wählen Sie in den Firmware-Einstellungen für die industrielle Kommunikation „PROFINET IO Master“ aus und starten Sie die Robotersteuerung neu.**

![[Abbildung 1.3.4.2-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

**2. Überprüfen Sie den Bereitschaftsstatus des ausgewählten Protokolls in der Überwachung der industriellen Kommunikation.**

![[Abbildung 1.3.4.2-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

**3. Wählen Sie mit Sycon.net das PCI-Gerät „PROFINET IO-Controller“ aus.**

![[Abbildung 1.3.4.2-3 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_3.png>)
![[Abbildung 1.3.4.2-4 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

**4. Scannen Sie das PCI-Gerät und wenden Sie den PROFINET IO-Controller an.**

![[Abbildung 1.3.4.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

**5. Laden Sie die Einstellungen herunter.**

![[Abbildung 1.3.4.2-6 PROFINET IO Controller Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

**6. Bereiten Sie die Gerätemodule (Slave) für die Verbindung mit dem PROFINET IO-Controller vor.**
   * In diesem Beispiel verwenden wir das PROFINET IO-Gerät Crevis M9287.
   * Bitte versorgen Sie das Modul mit Systemstrom und Feldstrom, um es zu aktivieren.

![[Abbildung 1.3.4.2-7 Crevis M9287]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
   - So legen Sie den Namen des PROFINET IO-Geräts mit dem DIP-Schalter fest

   - M9287-XX: Mit DIP-Schalter eingestellte Nummer

   - In diesem Beispiel wurde der Name mit DIP-Schalter 1 auf M9287-01 eingestellt.
{% endhint %}

<br>

**7. (Beispiel für DIP-Schalter) Legen Sie den Namen des Slave-Geräts mit dem DIP-Schalter fest.**
   * Schalten Sie nur den DIP-Schalter 1 auf EIN.


![[Abbildung 1.3.4.2-8 Crevis M9287 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
   - Bitte starten Sie das Gerät nach der Einstellung der DIP-Schalter neu.
{% endhint %}

<br>

**8. Registrieren Sie die GSDML-Datei des Slave-Geräts.**

{% hint style="info" %}
   - Für die Verwendung von Geräten, die nicht in Sycon.net registriert sind, ist eine GSDML-Datei erforderlich.

   - Die GSDML-Datei für das Gerät M9287 kann von der Crevis-Website heruntergeladen werden.
{% endhint %}

![[Abbildung 1.3.4.2-9 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
   - Registrieren Sie die heruntergeladene GSDML-Datei in Sycon.net.

   - Überprüfen Sie bei der Registrierung von GSDML-Dateien bitte das industrielle Kommunikationsprotokoll (PROFINET IO).
{% endhint %}

![[Abbildung 1.3.4.2-10 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_10.png>)![[Abbildung 1.3.4.2-11 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_11.png>)
![[Abbildung 1.3.4.2-12 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_12.png>)

![[Abbildung 1.3.4.2-13 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_13.png>)


<br>

**9. Netzwerkscan**

{% hint style="info" %}
   - Der PROFINET IO-Controller unterstützt die Netzwerkscan-Funktion.
{% endhint %}

{% hint style="info" %}
   - Klicken Sie mit der rechten Maustaste auf das Gerät „PROFINET IO Master“ und wählen Sie „Netzwerkscan“.
{% endhint %}

![[Abbildung 1.3.4.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
   - Wenn die GSDML-Datei nicht registriert ist, werden die Slave-Informationen bei der Durchführung eines Netzwerkscans angezeigt, jedoch ist eine Registrierung nicht möglich.
{% endhint %}

![[Abbildung 1.3.4.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - Wenn die GSDML-Datei ordnungsgemäß registriert ist, können Slave-Geräte über den Netzwerkscan hinzugefügt werden.
{% endhint %}

![[Abbildung 1.3.4.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_16.png>)

![[Abbildung 1.3.4.2-17 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_17.png>)

![[Abbildung 1.3.4.2-18 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

**10. Konfiguration des Slave-Geräts (Gerät)**

{% hint style="info" %}
   - Klicken Sie auf „Trennen“ des Master-Geräts für die Konfiguration des Slave-Geräts.
{% endhint %}

![[Abbildung 1.3.4.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - Doppelklicken Sie auf das Slave-Gerät.
{% endhint %}

![[Abbildung 1.3.4.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - Fügen Sie die mit M9287 verbundenen Slots für die PROFINET IO Slave (Gerät)-Einstellungen hinzu.

   - Slot 1 : M7001  
   - Slot 2 : M12DF  
   - Slot 3 : M225F  
{% endhint %}

![[Abbildung 1.3.4.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_21.png>)

![[Abbildung 1.3.4.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

**11. Konfiguration des Master-Geräts (Steuerung)**

{% hint style="info" %}
   - Doppelklicken Sie auf das Master-Gerät.
{% endhint %}

![[Abbildung 1.3.4.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - Legen Sie die IP-Adressen des Master-Geräts und des Slave-Geräts fest.

   - Die Slave-IP-Adresse des PROFINET IO-Geräts wird im Master festgelegt.

   - Bitte stellen Sie sicher, dass die IP-Adressen im gleichen Band liegen und sich zwischen Master und Slave nicht überschneiden.
{% endhint %}

![[Abbildung 1.3.4.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_24.png>)

![[Abbildung 1.3.4.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - Bitte überprüfen Sie, ob die Slot-Informationen des Slave-Geräts im Master-Gerät korrekt sind.
{% endhint %}

![[Abbildung 1.3.4.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - Überprüfen Sie die zugewiesenen E/A und die Startadresse für jeden Slave-Slots in der Adresstabelle.
{% endhint %}

![[Abbildung 1.3.4.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - Legen Sie die E/A-Kommunikationsgeschwindigkeit für PROFINET IO fest.
{% endhint %}

![[Abbildung 1.3.4.2-28 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - Fahren Sie nach Abschluss der Einstellungen mit dem Herunterladen fort.
{% endhint %}

![[Abbildung 1.3.4.2-29 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

**12. Überprüfen Sie den Kommunikationsstatus**

{% hint style="info" %}
   - Überprüfen Sie den Kommunikationsstatus in Sycon.net und TP.

   - Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („[**1.4 Überwachen der CIFX-PCI-Kommunikation**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)“).
{% endhint %}

{% hint style="info" %}
   - Doppelklicken Sie auf das angeschlossene Master-Gerät, um den Kommunikationsstatus zu überprüfen.
{% endhint %}

![[Abbildung 1.3.4.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_30.png>)

![[Abbildung 1.3.4.2-31 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
   - Mit der Diagnosefunktion von Sycon.net können Sie den Kommunikationsstatus und den Status der E/A-Ein- und Ausgänge überwachen.
{% endhint %}

![[Abbildung 1.3.4.2-32 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_32.png>)

<br>

**13. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.**

{% hint style="info" %}
   **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../../../4-io-block-allocation.md)“).**
{% endhint %}
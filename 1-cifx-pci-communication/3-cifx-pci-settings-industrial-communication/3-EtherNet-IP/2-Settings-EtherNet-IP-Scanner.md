# 1.3.3.2 EtherNet/IP-Scanner-Einstellungen

“[Bitte befolgen Sie die Anweisungen unter „**1.3.1 CIFX-PCI-Steckplatz-Einstellungen**” und „**1.3.2 SYCON.NET-Einstellungen**” und fahren Sie dann mit der folgenden Methode fort.](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 및 "[Bitte befolgen Sie die Anweisungen unter „**1.3.1 CIFX-PCI-Steckplatz-Einstellungen**” und „**1.3.2 SYCON.NET-Einstellungen**” und fahren Sie dann mit der folgenden Methode fort.](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      SYCON.net 이용 중 매뉴얼에 설명이 부족한 부분은  ""[\.      Wenn Sie SYCON.net verwenden und die Erläuterungen im Handbuch nicht ausreichen, ziehen Sie bitte die Funktion „**1.3.2 SYCON.NET-Hilfe**” zu Rate.](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" 기능을 참고해 주십시오.
{% endhint %}

<br>

##### 1. Wählen Sie EtherNet/IP Master in den Firmware-Einstellungen für die industrielle Kommunikation aus und starten Sie die Robotersteuerung neu.

![[Abbildung 1.3.3.2-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_1.png>)

<br>

##### 2. Überprüfen Sie den Bereitschaftsstatus des ausgewählten Protokolls in der Überwachung der industriellen Kommunikation.

![[Abbildung 1.3.3.2-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_2.png>)

<br>

##### 3. Wählen Sie mit Sycon.net das EtherNet/IP-Scanner-PCI-Gerät aus.

![[Abbildung 1.3.3.2-3 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_3.png>)
![[Abbildung 1.3.3.2-4 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_4.png>)

<br>

##### 4. Scannen Sie das PCI-Gerät und wenden Sie den EtherNet/IP-Scanner an.

![[Abbildung 1.3.3.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_5.png>)

<br>

##### 5. Laden Sie die Einstellungen herunter.

![[Abbildung 1.3.3.2-6 EtherNet/IP Scanner Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_6.png>)

<br>

##### 6. Bereiten Sie die Adaptermodule (Slave) für den Anschluss an den EtherNet/IP-Scanner vor.
   * In diesem Beispiel verwenden wir den Crevis M9289 EtherNet/IP-Adapter.
   * Bitte versorgen Sie das Modul mit Systemstrom und Feldstrom, um es zu aktivieren.

![[Abbildung 1.3.3.2-7 Crevis M9289]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_7.png>)

<br>

##### 7. Legen Sie die IP-Adresse des Adapters (Slave) für die EtherNet/IP-Kommunikationsverbindung fest.

{% hint style="info" %}
\.      Einstellung der IP-Adresse über DIP-Schalter
{% endhint %}

![[Abbildung 1.3.3.2-8 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      Einstellung der IP-Adresse über BootpSvr.exe
{% endhint %}

<br>

##### 8. (Bootp-Beispiel) Legen Sie die IP-Adresse des Slave-Geräts über Bootp fest.
   * Schalten Sie nur den DIP-Schalter 9 auf EIN.

![[Abbildung 1.3.3.2-9 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_9.png>)

   * Verbinden Sie den PC mit dem LAN-Anschluss des M9289-Adapters.

![[Abbildung 1.3.3.2-10 Crevis M9289 LAN Port]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

##### 9. Führen Sie BootpSvr.exe auf dem PC aus.
   * Dieses Programm wird von Crevis bereitgestellt. (Laden Sie IO Guide Pro von der Website herunter und installieren Sie es.)

![[Abbildung 1.3.3.2-11 Crevis IO Guide Pro]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_11.png>)

![[Abbildung 1.3.3.2-12 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
\.      Drücken Sie „Start BootP“, trennen Sie das M9289-Modul vom Stromnetz und schließen Sie es wieder an, um es neu zu starten.
{% endhint %}

![[Abbildung 1.3.3.2-13 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

##### 10. Wenn das Adaptergerät neu gestartet wird, werden die Geräteinformationen im Programm BootpSvr.exe angezeigt.

![[Abbildung 1.3.3.2-14 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

##### 11. Wählen Sie das Gerät aus und stellen Sie die IP ein.

![[Abbildung 1.3.3.2-15 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_15.png>)![[Abbildung 1.3.3.2-16 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

##### 12. Nachdem die IP-Einstellung abgeschlossen ist, schalten Sie alle DIP-Schalter des Adapters auf AUS und starten Sie das Gerät neu.

{% hint style="info" %}
\.      Überprüfen Sie unbedingt den Status der DIP-Schalter und ob der Adapter neu gestartet wurde.
{% endhint %}

![[Abbildung 1.3.3.2-17 Crevis DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

##### 13. Registrieren Sie die EDS-Datei des Slave-Geräts.

{% hint style="info" %}
\.      Für die Verwendung von Geräten, die nicht in Sycon.net registriert sind, ist eine EDS-Datei erforderlich.

\.      Die EDS-Datei für den M9289-Adapter kann von der Crevis-Website heruntergeladen werden.
{% endhint %}

![[Abbildung 1.3.3.2-18 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
\.      Registrieren Sie die heruntergeladene EDS-Datei in Sycon.net.

\.      Bitte überprüfen Sie bei der Registrierung von EDS-Dateien das industrielle Kommunikationsprotokoll (EtherNet/IP).
{% endhint %}

![[Abbildung 1.3.3.2-19 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_19.png>)![[Abbildung 1.3.3.2-20 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_20.png>)
![[Abbildung 1.3.3.2-21 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_21.png>)

![[Abbildung 1.3.3.2-22 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

##### 14. Network Scan

{% hint style="info" %}
\.      Der EtherNet/IP-Scanner unterstützt keine Netzwerkscan-Funktion.
{% endhint %}

<br>

##### 15. Konfiguration des Slave-Geräts (Adapter)

{% hint style="info" %}
\.      Ziehen Sie das registrierte Gerät und platzieren Sie es auf der EtherNet/IP-Master-Busleitung.
{% endhint %}

![[Abbildung 1.3.3.2-23 Sycon.net Bus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      Doppelklicken Sie auf das Gerät (Adapter), um mit den Einstellungen fortzufahren.

\.      Legen Sie die Anzahl der Eingangs-/Ausgangs-Bytes fest, die für das in diesem Gerät installierte E/A-Gerät geeignet ist.

\.      In diesem Beispiel wurden die folgenden Einstellungen vorgenommen.
{% endhint %}

<br>

![[Abbildung 1.3.3.2-24 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.        O -> T : Originator(Master) -> Target (Slave)

\.        Output : EtherNet/IP Scanner  -> M9289

\.        [Output Module]
\.         1. M225F (2Bytes)
\.         **\.         => 2Bytes**
{% endhint %}

<br>

![[Abbildung 1.3.3.2-25 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.        T -> O : Target (Slave) -> Originator(Master)

\.        Input : M9289 -> EtherNet/IP Scanner

\.        [Input Module]
\.         1. M7001  (1Byte)
\.         2. M12DF  (2Bytes)
\.         **\.         => 3Bytes**


\.         1.M7002 (0Byte)
\.         2.M12DF (2Bytes)
\.         **\.         => 2Bytes**
{% endhint %}

<br>

##### 16. Konfiguration des Master-Geräts (Scanner)
    

{% hint style="info" %}
\.      Klicken Sie mit der rechten Maustaste auf das Master-Gerät und wählen Sie „Trennen“.
{% endhint %}

![[Abbildung 1.3.3.2-26 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.      Doppelklicken Sie auf das Master-Gerät.

\.      Legen Sie die IP-Adresse des Master-Geräts fest.
{% endhint %}

![[Abbildung 1.3.3.2-27 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.      Legen Sie die IP-Adresse des Slave-Geräts fest.
{% endhint %}

![[Abbildung 1.3.3.2-28 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.      Legen Sie die Scan-Zeit des Slave-Geräts fest.

\.      Bitte passen Sie diesen Wert an, um die geeignete Kommunikationsgeschwindigkeit festzulegen.
{% endhint %}

![[Abbildung 1.3.3.2-29 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.      Überprüfen Sie die Einstellungen des Slave-Geräts in der Adressentabelle.

\.      Überprüfen Sie die Anzahl der Eingangs-/Ausgangs-E/A-Bytes und die Startadresse.
{% endhint %}

![[Abbildung 1.3.3.2-30 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
\.        [Quick Connect]

\.      EtherNet/IP unterstützt die Quick-Connect-Funktion.
{% endhint %}

{% hint style="info" %}
\.      Die folgenden Bedingungen müssen erfüllt sein, um die Quick-Connect-Funktion nutzen zu können.

\.      (1) Produkte, die Master-, Slave-Quick-Connect unterstützen, sind erforderlich.
\.      (2) Quick Connect kann nicht verwendet werden, wenn Auto-Negotiation genutzt wird
\.      (3) Quick Connect kann nicht verwendet werden, wenn Auto-MDI-X genutzt wird
\.      (4) 100 Mbit/s, Vollduplex erforderlich
{% endhint %}

{% hint style="info" %}
\.      Fahren Sie nach Abschluss der Einstellungen mit dem Herunterladen fort.
{% endhint %}

![[Abbildung 1.3.3.2-31 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

##### 17. Überprüfen Sie den Kommunikationsstatus

{% hint style="info" %}
\.      Überprüfen Sie den Kommunikationsstatus in Sycon.net und TP.

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[\.      Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („1.4 Überwachen der CIFX-PCI-Kommunikation“).](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      Doppelklicken Sie auf das angeschlossene Master-Gerät, um den Kommunikationsstatus zu überprüfen.
{% endhint %}

![[Abbildung 1.3.3.2-32 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_32.png>)

![[Abbildung 1.3.3.2-33 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
\.      Mit der Diagnosefunktion von Sycon.net können Sie den Kommunikationsstatus und den Status der E/A-Ein- und Ausgänge überwachen.
{% endhint %}

![[Abbildung 1.3.3.2-34 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_34.png>)

<br>

##### 18. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[\.      **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**“).**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
# 1.3.2 SYCON.NET-Einstellungen

Hi6 제어기는 “**Sycon.net**” 프로그램을 이용하여 산업용 통신 설정을 진행합니다. 설정 방법은 다음과 같습니다. (“[Die Hi6-Steuerung führt die industriellen Kommunikationseinstellungen mit dem Programm „**Sycon.net**” durch. Die Einstellung erfolgt wie folgt. (Bitte installieren Sie das Programm gemäß „**1.1 Installation von Sycon.net**”.)](../../1-cifx-pci-install-program/1-sycon-net.md)”을 참고하여 설치해주시기 바랍니다.)

<br>

##### 1. Referenzmaterialien zu den Kommunikationseinstellungen.
*„Sycon.net v1.0500\DVD\_2018-12-1\_1\_0500\Documentation\4. Training Material\EN”** Materialien können als Referenz herangezogen werden.
   * Referenzmaterialien

1\) EtherNetIP Scanner - Configuration and Testing TM 02 EN.pdf

2\) PROFIBUS DP Master – Configuration and Testing TM 02 EN.pdf

3\) PROFINET IO Controller - Configuration and Testing TM 02 EN.pdf

<br>

##### 2. Verbinden Sie den PC, auf dem Sycon.net installiert ist, mit dem allgemeinen LAN-Port der Robotersteuerung. (Nicht mit dem PCI-LAN-Port)
*\[System > 2: Steuerungsparameter > 9: Netzwerk]** Tippen Sie auf das Menü, um die IP-Adresse des allgemeinen LAN-Ports zu überprüfen. Bitte überprüfen Sie den Verbindungsstatus durch einen Ping-Test usw.

![[Abbildung 1.3.2-1 Netzwerk-IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_1.png>)
![[Abbildung 1.3.2-2 Netzwerk-IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_2.png>)

{% hint style="info" %}
\.      Die IP-Adresse kann entsprechend den Benutzereinstellungen geändert werden.
{% endhint %}

<br>

##### 3. Führen Sie Sycon.net aus.

![[Abbildung 1.3.2-3 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_3.png>)

<br>

##### 4. Klicken Sie im Geräte-Katalog auf der rechten Seite des Bildschirms auf das Element, das dem konfigurierten Kommunikationsprotokoll entspricht, und legen Sie es per Drag & Drop auf der Busleitung in der Mitte ab.

![[Abbildung 1.3.2-4 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_4.png>)
![[Abbildung 1.3.2-5 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_5.png>)

<br>

##### 5. Doppelklicken Sie auf das importierte Element, um die Einstellungen zu konfigurieren.

{% hint style="info" %}
\.      „Doppelklicken“ Sie auf das importierte CIFX PCI (Abbildung).

\.      Settings -> Driver

\.      Wählen Sie den netX-Treiber aus.
{% endhint %}

![[Abbildung 1.3.2-6 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_6.png>)

{% hint style="info" %}
\.     Setting -> Driver -> netX Driver -> TCP Connection

\.      IP-Adresse: Bitte geben Sie die allgemeine LAN-Port-IP-Adresse der angeschlossenen Steuerung ein.
{% endhint %}

![[Abbildung 1.3.2-7 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_7.png>)

{% hint style="info" %}
\.      Gerätezuweisung -> Klicken Sie auf „Scannen“.

\.      Wählen Sie die Kommunikation aus (überprüfen Sie das Kanalprotokoll), klicken Sie dann auf „Übernehmen“ und „OK“.
{% endhint %}

{% hint style="warning" %}
*\[Achtung]**: Bitte überprüfen Sie unbedingt das Kanalprotokoll und die Slotnummer.
{% endhint %}

{% hint style="warning" %}
*\[Achtung]**: Wenn der Scan nicht funktioniert, überprüfen Sie den Kabelverbindungsstatus mit der Steuerung und den Firmware-Einstellungen.
{% endhint %}

![[Abbildung 1.3.2-8 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_8.png>)


{% hint style="info" %}
\.      Klicken Sie mit der rechten Maustaste auf die CIFX PCI-Abbildung -> DOWNLOAD
{% endhint %}

![[Abbildung 1.3.2-9 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_9.png>)
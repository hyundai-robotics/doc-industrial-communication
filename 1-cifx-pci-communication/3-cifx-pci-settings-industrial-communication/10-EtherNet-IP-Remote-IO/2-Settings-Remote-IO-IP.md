## 1.3.10.2 Festlegen der Remote-E/A-IP-Adresse

So stellen Sie die IP-Adresse des Crevis M9289 EtherNet/IP-Netzwerkadapters ein.

<br>

{% hint style="info" %}
\.      Die werkseitige Standard-IP des Crevis M9289 Remote-E/A lautet 192.168.100.99.

\.      Wenn Sie die IP-Adresse des Remote-E/A nicht kennen oder ändern müssen, führen Sie bitte die folgenden Schritte aus.
{% endhint %}

<br>

**1. Verbinden Sie den PC und den Remote-E/A direkt über ein LAN-Kabel.**

![[Abbildung 1.3.10.2-1 LAN-Verbindung]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

**2. Schalten Sie nur den DIP-Schalter 9 des Remote-E/A-Adapters auf EIN.**

![[Abbildung 1.3.10.2-2 DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

**3. Führen Sie das Programm „Bootpsvr.exe“ aus.**
   * Dieses Programm wird von Crevis bereitgestellt. (Laden Sie IO Guide Pro von der Website herunter und installieren Sie es.)

![[Abbildung 1.3.10.2-3 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[Abbildung 1.3.10.2-4 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
\.      Drücken Sie „Start BootP“, trennen Sie das M9289-Modul vom Stromnetz und schließen Sie es wieder an, um es neu zu starten.
{% endhint %}

![[Abbildung 1.3.10.2-5 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>


**4. Wenn das Adaptergerät neu gestartet wird, werden die Geräteinformationen im Programm BootpSvr.exe angezeigt.**

![[Abbildung 1.3.10.2-6 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

**5. Wählen Sie das Gerät aus und stellen Sie die IP ein.**

![[Abbildung 1.3.10.2-7 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[Abbildung 1.3.10.2-8 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

**6. Nachdem die IP-Einstellung abgeschlossen ist, schalten Sie alle DIP-Schalter des Adapters auf AUS und starten Sie das Gerät neu.**

{% hint style="info" %}
\.      Überprüfen Sie unbedingt den Status der DIP-Schalter und ob der Adapter neu gestartet wurde.
{% endhint %}

![[Abbildung 1.3.10.2-9 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

**7. Überprüfen Sie die IP-Adresse mithilfe eines Ping-Tests usw. auf dem PC.**

![[Abbildung 1.3.10.2-10 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

**8. Wenn die IP-Adresse erfolgreich geändert wurde, fahren Sie mit den Einstellungen fort.**

{% hint style="info" %}
\.      Bitte fahren Sie mit den Einstellungen gemäß dem Verfahren „[**1.3.10.1 EtherNet/IP – Standard-Einstellungen für die Remote-E/A-Verbindung**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)“ fort.
{% endhint %}

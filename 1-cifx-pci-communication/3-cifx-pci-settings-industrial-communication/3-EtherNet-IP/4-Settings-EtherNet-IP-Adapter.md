# 1.3.3.4 EtherNet/IP-Adaptereinstellungen

“[Befolgen Sie bitte die Schritte unter „**1.3.1 CIFX-PCI-Slot-Einstellungen**“ und fahren Sie dann mit der folgenden Methode fort.](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      **\.      [EtherNet/IP-Adapter-EDS-Datei herunterladen]**

\.      “[\.      Bitte beachten Sie „**5. Beschreibungsdatei für Slave-Geräte**”.](../../../5-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

<br>

##### 1. Wählen Sie mithilfe von TP in den Firmware-Einstellungen für die industrielle Kommunikation „EtherNet/IP Slave“ aus und starten Sie die Robotersteuerung neu.

![[Abbildung 1.3.3.4-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_1.png>)

<br>

##### 2. Überprüfen Sie den aktuellen Status der Kommunikationsprotokollbereitschaft in der Überwachung der industriellen Kommunikation.

![[Abbildung 1.3.3.4-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_2.png>)

<br>

{% hint style="warning" %}
*\[Achtung]**: Wenn eine von Sycon.net festgelegte Konfigurationsdatei auf diesen PCI-Slot heruntergeladen wird, werden die TP-Einstellungen ignoriert.
{% endhint %}

<br>

##### 3. Berühren Sie das Menü, um den Bildschirm mit den Slave-Einstellungen aufzurufen.
*\\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 2: PCI-Slave-Slot-Einstellungen >  EtherNet/IP Slave]**

![[Abbildung 1.3.3.4-3 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_3.png>)

![[Abbildung 1.3.3.4-4 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_4.png>)

<br>

##### 4. Beschreibung der einzelnen Elemente

{% hint style="info" %}
\.      [IP-Einstellung]

\.      Feste IP: Der Anwender legt die IP-Adresse, die Subnetzmaske und die Gateway-Informationen fest.

\.      DHCP: Die IP-Adresse wird vom DHCP-Server zugewiesen.
{% endhint %}

{% hint style="info" %}
\.      [Aktion bei Busfehler]

\.      Löschen: Initialisieren Sie bei einem Kommunikationsfehler alle Eingänge auf 0.

\.      Beibehalten: Behalten Sie bei einem Kommunikationsfehler den letzten gültigen Eingangswert bei.
{% endhint %}

{% hint style="info" %}
\.      [Zulässige Fehlerzeit]

\.      Wenn der Kommunikationsfehler länger als die angegebene zulässige Zeit andauert, werden ein Feldbus-Fehlersignal und ein Alarm ausgegeben.
{% endhint %}

{% hint style="info" %}
\.      [Eingangsbytes]

\.      Eingangsbytes: Legen Sie die Datengröße für die Eingabe von Master -> Slave fest.

\.      O -> T : Originator(Master) -> Target (Slave)
{% endhint %}

{% hint style="info" %}
\.      [Ausgangsbytes]

\.      Ausgangsbytes: Legen Sie die Datengröße für die Ausgabe von Slave -> Master fest.

\.      T -> O : Target (Slave) -> Originator(Master)
{% endhint %}

{% hint style="info" %}
\.      [Run / Idle Header]

\.      Der CIFX-50 RE EtherNet/IP-Adapter, der für die Steuerung verwendet wird, nutzt beim Austausch von E/A mit dem Scanner einen 32-Bit-Run-/Idle-Header. (Standard)

\.      Bitte stellen Sie die Verwendung des 32-Bit-Run/Idle-Headers für Ein- und Ausgabe entsprechend den Scanner-Spezifikationen ein.
{% endhint %}

<br>

{% hint style="info" %}
\.        [Quick Connect]

\.      EtherNet/IP unterstützt die Quick-Connect-Funktion.

\.      Wenn die Quick-Connect-Funktion erforderlich ist, stellen Sie den EtherNet/IP-Adapter bitte mit Sycon.net ein.

\.      (1) Produkte, die Master-, Slave-Quick-Connect unterstützen, sind erforderlich.
\.      (2) Quick Connect kann nicht verwendet werden, wenn Auto-Negotiation genutzt wird
\.      (3) Quick Connect kann nicht verwendet werden, wenn Auto-MDI-X genutzt wird
\.      (4) 100 Mbit/s, Vollduplex erforderlich
{% endhint %}

<br>

##### 5. Überprüfen Sie nach Abschluss der Einstellungen den Kommunikationsstatus gemäß dem folgenden Verfahren.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („1.4 Überwachung der CIFX-PCI-Kommunikation“).](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[Abbildung 1.3.3.4-5 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_5.png>)

<br>

##### 6. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[\.      **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**“).**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
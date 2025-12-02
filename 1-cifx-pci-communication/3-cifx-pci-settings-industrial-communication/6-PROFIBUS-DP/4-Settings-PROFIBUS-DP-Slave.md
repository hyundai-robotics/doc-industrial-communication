# 1.3.6.4 PROFIBUS-DP-Slave-Einstellungen

“[Befolgen Sie bitte die Schritte unter „**1.3.1 CIFX-PCI-Slot-Einstellungen**“ und fahren Sie dann mit der folgenden Methode fort.](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      **\.      [PROFIBUS-DP-Slave-GSD-Datei herunterladen]**

\.      “[\.      Bitte beachten Sie „**5. Beschreibungsdatei für Slave-Geräte**”.](../../../5-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

<br>

##### 1. Wählen Sie mithilfe von TP in den Firmware-Einstellungen für die industrielle Kommunikation „PROFIBUS-DP Slave“ aus und starten Sie die Robotersteuerung neu.

![[Abbildung 1.3.6.4-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>)

<br>

##### 2. Überprüfen Sie den aktuellen Status der Kommunikationsprotokollbereitschaft in der Überwachung der industriellen Kommunikation.

![[Abbildung 1.3.6.4-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>)

<br>

{% hint style="warning" %}
*\[Achtung]**: Wenn eine von Sycon.net festgelegte Konfigurationsdatei auf diesen PCI-Slot heruntergeladen wird, werden die TP-Einstellungen ignoriert.
{% endhint %}

<br>

##### 3. Berühren Sie das Menü, um den Bildschirm mit den Slave-Einstellungen aufzurufen.
*\\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 2: PCI-Slave-Slot-Einstellungen >  PROFIBUS-DP Slave]**

![[Abbildung 1.3.6.4-3 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>)

![[Abbildung 1.3.6.4-4 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>)

<br>

##### 4. Beschreibung der einzelnen Elemente

{% hint style="info" %}
\.      [Station Address]

\.      PROFIBUS-DP identifiziert Slaves über die Stationsadresse.
{% endhint %}

{% hint style="info" %}
\.      [Eingangsbytes]

\.      Eingangsbytes: Legen Sie die Datengröße für die Eingabe von Master -> Slave fest.
{% endhint %}

{% hint style="info" %}
\.      [Ausgangsbytes]

\.      Ausgangsbytes: Legen Sie die Datengröße für die Ausgabe von Slave -> Master fest.
{% endhint %}

{% hint style="info" %}
\.      [**\.      [Bei der Einstellung des Moduls im Master]**]

\.      Die Module müssen im Master so festgelegt werden, dass sie mit der eingestellten Byteanzahl übereinstimmen.

\.      Reihenfolge: Master-Eingang (64 ~ 1) -> Master-Ausgang (64 ~ 1)

\.      EX) Master Input 109 bytes  <---  Slave Output 109 bytes
\.          Input 109 Bytes : 64Byte + 32Byte + 8Byte + 4Byte + 1 Byte

\.      EX) Master Output 120 bytes  --->  Slave Input 120 bytes
\.          Output 120 Bytes : 64Byte + 32Byte + 16Byte + 8Byte


\.      EX) Master Input 12 bytes  <---  Slave Output 12 bytes
\.          Input 12 Bytes : 8Byte + 4Byte

\.      EX) Master Output 200 bytes  --->  Slave Input 200 bytes
\.          Output 200 Bytes : 64Byte + 64Byte + 64Byte + 8Byte

\.      Das Eingangsmodul befindet sich vor dem Ausgangsmodul.
{% endhint %}

![[Abbildung 1.3.6.4-5 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>)


<br>

##### 5. Überprüfen Sie nach Abschluss der Einstellungen den Kommunikationsstatus gemäß dem folgenden Verfahren.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („1.4 Überwachung der CIFX-PCI-Kommunikation“).](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[Abbildung 1.3.6.4-6 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>)

<br>

##### 6. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[\.      **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**“).**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
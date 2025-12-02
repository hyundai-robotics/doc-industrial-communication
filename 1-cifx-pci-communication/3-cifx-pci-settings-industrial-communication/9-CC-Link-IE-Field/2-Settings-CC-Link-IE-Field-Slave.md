# 1.3.9.2 CC-Link IE Field Slave-Einstellungen

“[Befolgen Sie bitte die Schritte unter „**1.3.1 CIFX-PCI-Slot-Einstellungen**“ und fahren Sie dann mit der folgenden Methode fort.](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.


<br>

##### 1. Wählen Sie über TP in den Einstellungen der industriellen Kommunikationsfirmware „CC-Link IE Field Slave“ aus und starten Sie die Robotersteuerung neu.

![[Abbildung 1.3.9.2-1 Firmware-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_1.png>)

<br>

##### 2. Überprüfen Sie den aktuellen Status der Kommunikationsprotokollbereitschaft in der Überwachung der industriellen Kommunikation.

![[Abbildung 1.3.9.4-2 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>)

<br>

{% hint style="warning" %}
*\[Achtung]**: Wenn eine von Sycon.net festgelegte Konfigurationsdatei auf diesen PCI-Slot heruntergeladen wird, werden die TP-Einstellungen ignoriert.
{% endhint %}

<br>

##### 3. Berühren Sie das Menü, um den Bildschirm mit den Slave-Einstellungen aufzurufen.
*\\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 2: PCI-Slave-Slot-Einstellungen >  CC-Link IE Field Slave]**

![[Abbildung 1.3.9.4-3 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>)

![[Abbildung 1.3.9.4-4 Slave-Einstellungen]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>)

<br>

##### 4. Beschreibung der einzelnen Elemente

{% hint style="info" %}
\.      [Network Number]

\.      CC-Link IE Field-Netzwerknummer (1~239)
{% endhint %}

{% hint style="info" %}
\.      [Station Address]

\.      Geräte-ID innerhalb des verbundenen Netzwerks (1 ~ 120)
{% endhint %}

{% hint style="info" %}
\.      [IO Type]

\.      Der E/A-Typ wird durch die Einstellungen des Master-Geräts bestimmt
\.      - Gemischt: Eingang und Ausgang verwenden unterschiedliche Indizes (unterschiedliche Adressen)
\.      - Eingang: Nur Eingang
\.      - Ausgang: Nur Ausgang
\.      - FrontBackMixture: Eingang und Ausgang verwenden denselben Index (dieselbe Adresse)
{% endhint %}

{% hint style="info" %}
\.      [Device Type]

\.      Die maximal einstellbare E/A-Größe hängt vom Gerätetyp ab.

\.      Intelligent Device Station
\.      - RY, RX (max): 256 bytes
\.      - RWw, RWr (max): 1024 words

\.      Remote Device Station
\.      - RY, RX (max): 16 bytes
\.      - RWw, RWr (max): 64 words
{% endhint %}

{% hint style="info" %}
\.      [IO Size]

\.      Master -> Slave
\.      - RWw (word data)
\.      - RY (bit data)

\.      Slave -> Master
\.      - RWr (word data)
\.      - RX (bit data)
{% endhint %}

<br>

##### 5. Überprüfen Sie nach Abschluss der Einstellungen den Kommunikationsstatus gemäß dem folgenden Verfahren.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[Informationen zum Überprüfen des Status der industriellen Kommunikation auf TP finden Sie unter („1.4 Überwachung der CIFX-PCI-Kommunikation“).](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

<br>

##### 6. Weisen Sie nach Abschluss der Kommunikationseinstellungen einen E/A-Block zu.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[\.      **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**“).**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}

<br>

![[Abbildung 1.3.9.4-5 Überwachung der industriellen Kommunikation]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>)
# 1.3.1 CIFX-PCI-Slot-Einstellungen.

Konfigurieren Sie die Kommunikationsmethode für den CIFX-PCI-Slot. Um die Einstellungen zu übernehmen, trennen Sie bitte die Stromversorgung der Steuerung und schalten Sie sie dann wieder ein.

<br>

“[Beziehen Sie sich auf „**1.2.1 PCI-Industriekommunikationskarte**” und fahren Sie mit der folgenden Methode fort.](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" 참고하여 아래 방법을 진행해 주십시오.

<br>

##### 1. Berühren Sie das Menü, um den Bildschirm für die Slot-Einstellungen aufzurufen.
*\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 1: PCI-Slot-Einstellungen > Kanal 1]**


<br>

##### 2. Wählen Sie anhand des folgenden Bildschirms den Slot, die Kommunikationsmethode (Master/Slave) und das Protokoll aus.
   * Die Slotnummer ist die Nummer des Drehschalters der PCI-Kommunikationskarte.
   * 통신 설정 변경을 원하지 않을 경우 **Wenn Sie die Kommunikationseinstellungen nicht ändern möchten, tippen Sie auf die Schaltfläche \[OK], um den Bildschirm zu schließen.** 버튼을 터치하여 종료합니다.

{% hint style="warning" %}
* *\[주의]***\[Achtung]: Durch Berühren der Schaltfläche \[Initialisieren] oder \[Übernehmen]** werden die Slot-Informationen auf der aktuellen Registerkarte initialisiert. Bitte beachten Sie, dass auch die Konfigurationsdatei initialisiert wird.**\[초기화]***\[Achtung]: Durch Berühren der Schaltfläche \[Initialisieren] oder \[Übernehmen]** werden die Slot-Informationen auf der aktuellen Registerkarte initialisiert. Bitte beachten Sie, dass auch die Konfigurationsdatei initialisiert wird.**\[적용]** 버튼을 터치하면 현재 탭의 슬롯 정보가 초기화 됩니다. Config 파일도 같이 초기화 되니 유의하시기 바랍니다.
{% endhint %}

![[Abbildung 1.3.1-1 PCI-Slot-Einstellungen]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[Abbildung 1.3.1-2 PCI-Slot-Einstellungen(master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[Abbildung 1.3.1-3 PCI-Slot-Einstellungen(Slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

##### 3. Schließen Sie die Slot-Einstellungen ab.
*\[Übernehmen]** Tippen Sie auf das Menü

![[Abbildung 1.3.1-4 PCI-Slot-Einstellungen]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
*\[Achtung]**

<1>. **<1>. Wenn Sie die Einstellungen durch Berühren der Schaltfläche \[Übernehmen] anwenden, werden alle auf diesen Slot angewendeten CONFIG-Dateien gelöscht und geändert. Es wird empfohlen, bei einer Änderung der Kommunikation eine separate Sicherungskopie der vorhandenen Einstellungen zu erstellen.** 버튼을 터치하여 설정 시 해당 슬롯에 적용 되어있는 CONFIG 파일이 모두 삭제된 후 변경됩니다. 통신을 변경 하실 경우 기존 설정을 별도로 보관하는 것을 권장합니다.

<2>. **<2>. Wenn Sie die Schaltfläche \[OK] berühren, ohne auf die Schaltfläche \[Übernehmen] zu tippen, wird die ausgewählte Kommunikation nicht angewendet.** 버튼을 터치하지 않고 **<2>. Wenn Sie die Schaltfläche \[OK] berühren, ohne auf die Schaltfläche \[Übernehmen] zu tippen, wird die ausgewählte Kommunikation nicht angewendet.**버튼을 터치할 경우 선택한 통신이 적용되지 않습니다.
{% endhint %}

<br>

##### 4. Wiederholen Sie die Schritte 2. \~ 3. für jeden Slot.

<br>

##### 5. Starten Sie die Steuerung neu, um die konfigurierte Kommunikation anzuwenden.
*\[Service > 19: Überwachung der industriellen Kommunikation]** Tippen Sie auf das Menü, um zu überprüfen, ob die konfigurierte Kommunikation angewendet wurde.

![[Abbildung 1.3.1-5 Bildschirm „Einstellungen für industrielle Kommunikation“]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
*\[Achtung]**: Die Einstellungen werden angewendet, wenn die Steuerung nach den Sloteinstellungen neu gestartet wird.
{% endhint %}

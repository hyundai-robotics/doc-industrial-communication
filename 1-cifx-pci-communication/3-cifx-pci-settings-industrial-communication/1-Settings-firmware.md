# 1.3.1 CIFX-PCI-Slot-Einstellungen.

Konfigurieren Sie die Kommunikationsmethode für den CIFX-PCI-Slot. Um die Einstellungen zu übernehmen, trennen Sie bitte die Stromversorgung der Steuerung und schalten Sie sie dann wieder ein.

<br>

Beziehen Sie sich auf „[**1.2.1 PCI-Industriekommunikationskarte**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)“ und fahren Sie mit der folgenden Methode fort.

<br>

##### 1. Berühren Sie das Menü, um den Bildschirm für die Slot-Einstellungen aufzurufen.
**\[System > 2: Steuerungsparameter > 11: Industrielle Kommunikation > 1: PCI-Slot-Einstellungen > Kanal 1]** 


<br>

##### 2. Wählen Sie anhand des folgenden Bildschirms den Slot, die Kommunikationsmethode (Master/Slave) und das Protokoll aus.
   * Die Slotnummer ist die Nummer des Drehschalters der PCI-Kommunikationskarte.
   * Wenn Sie die Kommunikationseinstellungen nicht ändern möchten, tippen Sie auf die Schaltfläche **\[OK]**, um den Bildschirm zu schließen.

{% hint style="warning" %}
**\[Achtung]**: Durch Berühren der Schaltfläche **\[Initialisieren]** oder **\[Übernehmen]** werden die Slot-Informationen auf der aktuellen Registerkarte initialisiert. Bitte beachten Sie, dass auch die Konfigurationsdatei initialisiert wird.
{% endhint %}

![[Abbildung 1.3.1-1 PCI-Slot-Einstellungen]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[Abbildung 1.3.1-2 PCI-Slot-Einstellungen(master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[Abbildung 1.3.1-3 PCI-Slot-Einstellungen(Slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

##### 3. Schließen Sie die Slot-Einstellungen ab.
**\[Übernehmen]** Tippen Sie auf das Menü

![[Abbildung 1.3.1-4 PCI-Slot-Einstellungen]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[Achtung]**

<1>. Wenn Sie die Einstellungen durch Berühren der Schaltfläche **\[Übernehmen]** anwenden, werden alle auf diesen Slot angewendeten CONFIG-Dateien gelöscht und geändert. Es wird empfohlen, bei einer Änderung der Kommunikation eine separate Sicherungskopie der vorhandenen Einstellungen zu erstellen.

<2>. Wenn Sie die Schaltfläche **\[OK]** berühren, ohne auf die Schaltfläche **\[Übernehmen]** zu tippen, wird die ausgewählte Kommunikation nicht angewendet.
{% endhint %}

<br>

##### 4. Wiederholen Sie die Schritte 2. \~ 3. für jeden Slot.

<br>

##### 5. Starten Sie die Steuerung neu, um die konfigurierte Kommunikation anzuwenden.
**\[Service > 19: Überwachung der industriellen Kommunikation]** Tippen Sie auf das Menü, um zu überprüfen, ob die konfigurierte Kommunikation angewendet wurde.

![[Abbildung 1.3.1-5 Bildschirm „Einstellungen für industrielle Kommunikation“]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[Achtung]**: Die Einstellungen werden angewendet, wenn die Steuerung nach den Sloteinstellungen neu gestartet wird.
{% endhint %}

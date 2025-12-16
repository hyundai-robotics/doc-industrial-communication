# 1.3.8.1 CC-Link Slave-Spezifikationen

<br>

##### Protokollmerkmale

| **Kategorie** | **Spezifikationen** (Version 1.11) | **Spezifikationen** (Version 2.0) |
| :---                       | :---                       | :---                        |
| Maximale Eingangsbyte-Größe        | 48 Bytes                   | 368 Bytes                   |
| Maximale Ausgangsbyte-Größe        | 48 Bytes                   | 368 Bytes                   |
| E/A-Stations-Eingang | 4 Byte (RY) | Nicht unterstützt |
| E/A-Stations-Ausgang       | 4 Byte (RX)                | Nicht unterstützt           |
| Station                    | 1–4                        | 1–4                         |
| Extension Cycle            | Nicht unterstützt                      | 1, 2, 4, 8                  |
| Remote Deivce Input        | 16 Bytes(RY), 32 Byte(RWw) | 112 Bytes(RY), 256 Byte(RWw)|
| Remote Deivce Output       | 16 Bytes(RX), 32 Byte(RWr) | 112 Bytes(RY), 256 Byte(RWr)|
| Kommunikationsgeschwindigkeit | 156 bis 10000 Kbit/s | 156 bis 10000 Kbit/s |



<br>

##### Netzwerkmerkmale

| **Kategorie**                       | **Spezifikationen**                   |
| :---                           | :---                      |
| Data Transport Layer           |                           |
| Hub                            | Nicht zutreffend                  |
| Switch                         | Nicht zutreffend                  |


<br>

##### CC-Link-E/A-Zuordnung

<br>

{% hint style="info" %}
\.        CC-Link Version 1
{% endhint %}

<br>

![[Abbildung 1.3.8.1-1 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Erweiterungszyklus: Einzeln
{% endhint %}

<br>

![[Abbildung 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Double
{% endhint %}

<br>

![[Abbildung 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Erweiterungszyklus: Vierfach
{% endhint %}

<br>

![[Abbildung 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Erweiterungszyklus: Achtfach
{% endhint %}

<br>

![[Abbildung 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_5.png>)

<br>
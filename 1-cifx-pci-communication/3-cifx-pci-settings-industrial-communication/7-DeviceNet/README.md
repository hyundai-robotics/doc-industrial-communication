## 1.3.7 DeviceNet

In diesem Kapitel werden die Eigenschaften und Einstellungsmethoden von DeviceNet-Master und -Slave beschrieben. 

<br>

**Feldbus – Übersicht**

Feldbus ist ein Industriestandard, der für die Verbindung von Geräten wie Sensoren, Tastern, Motortreibern und Bedienoberflächen mit SPSen (speicherprogrammierbaren Steuerungen) über ein einziges Kabel und deren Betrieb in der Fabrik geöffnet wurde.

Feldbus bietet intelligente Dienste wie die zentrale Überwachung oder Neukonfiguration des gesamten Netzwerkstatus.

Beispielsweise sind für Sensoren oder Schalter detaillierte Informationen, Bedienungen, Moduseinstellungen usw. möglich, nicht nur einfaches Ein-/Ausschalten.

Die Verwendung eines einzigen Kabels reduziert den Zeit- und Kostenaufwand für die Verkabelung, vereinfacht die Konfiguration und ist vorteilhaft für die Wartung.

Im Gegensatz zu Protokollen mit nicht deterministischen Antwortcharakteristiken der allgemeinen Kommunikation ist außerdem die Datenantwortgeschwindigkeit garantiert, um industrielle Anwendungen zu erfüllen, bei denen kritische Zeitcharakteristiken wichtig sind.

![[Abbildung 1.3.7-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/image_1.png>)

<br>

Ein Feldbus-Netzwerk verbindet ein Master-Gerät und mehrere Slave-Geräte.
Master-Geräte suchen/verwalten das gesamte Netzwerk und tauschen Daten mit Slave-Geräten aus.

Im Allgemeinen sind SPSen Master-Geräte, und Sensoren, Tasten, Steuerungen usw. können als Slave-Geräte konfiguriert werden.
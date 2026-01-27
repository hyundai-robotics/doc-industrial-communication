## 1.3.9 CC-Link IE Field

In diesem Kapitel werden die Eigenschaften und Einstellungsmethoden von CC-Link IE Field-Slave beschrieben. 


<br>

**Feldbus – Übersicht**

Feldbus (Fieldbus) ist ein offener Industriestandard, der dazu dient, Geräte wie Sensoren, Taster, Motortreiber und Bedienoberflächen in der Fabrik über ein einziges Kabel mit einer SPS (Programmable Logic Controller) zu verbinden und zu betreiben.

Feldbus bietet intelligente Dienste wie die zentrale Überwachung oder Neukonfiguration des gesamten Netzwerkstatus.

Beispielsweise sind für Sensoren oder Schalter detaillierte Informationen, Bedienungen, Moduseinstellungen usw. möglich, nicht nur einfaches Ein-/Ausschalten.

Die Verwendung eines einzigen Kabels reduziert den Zeit- und Kostenaufwand für die Verkabelung, vereinfacht die Konfiguration und ist vorteilhaft für die Wartung.

Im Gegensatz zu Protokollen mit nicht deterministischen Antwortcharakteristiken der allgemeinen Kommunikation ist außerdem die Datenantwortgeschwindigkeit garantiert, um industrielle Anwendungen zu erfüllen, bei denen kritische Zeitcharakteristiken wichtig sind.

![[Abbildung 1.3.9-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/image_1.png>) 

<br>

Ein Feldbus-Netzwerk verbindet ein Master-Gerät und mehrere Slave-Geräte.
Master-Geräte suchen/verwalten das gesamte Netzwerk und tauschen Daten mit Slave-Geräten aus.

Im Allgemeinen sind SPSen Master-Geräte, und Sensoren, Tasten, Steuerungen usw. können als Slave-Geräte konfiguriert werden.

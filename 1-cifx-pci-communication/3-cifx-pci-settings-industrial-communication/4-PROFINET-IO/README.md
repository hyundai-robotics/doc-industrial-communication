# 1.3.4 PROFINET IO

In diesem Kapitel werden die Eigenschaften und Einstellungsmethoden von PROFINET IO-Master (Controller) und Slave (Gerät) beschrieben. 

<br>

##### PROFINET IO – Übersicht

PROFINET IO ist ein offenes industrielles Kommunikationsprotokoll auf Ethernet-Basis, das sich aus PROFIBUS-DP und Industrial Ethernet weiterentwickelt hat.

![[Abbildung 1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>) 

<br>

Es folgt dem Provider-Consumer-Modell für den Datenaustausch, und die Produkte lassen sich in die folgenden drei Klassen einteilen.

##### IO Controller Class
   * Produkte, die den bestehenden PROFIBUS-DP-Mastern der Klasse 1 entsprechen, wie z. B. SPSen, die Automatisierungsprogramme ausführen.

   * E/A-Steuerungen liefern Ausgangsdaten an die für sie konfigurierten E/A-Geräte und verbrauchen deren Eingangsdaten.

<br>

##### E/A-Geräteklasse
  * Produkte, die den bestehenden PROFIBUS-DP-Slaves entsprechen und über PROFINET IO mit E/A-Steuerungen wie SPSen verbunden sind.

  * E/A-Geräte liefern Ausgangsdaten an E/A-Steuerungen, stellen Eingangsdaten bereit und verbrauchen Ausgangsdaten.

<br>

##### IO Supervisor Class
   * Produkte, die bestehenden PROFIBUS-DP-Klasse-2-Mastern entsprechen, wie z. B. Programmiergeräte, PCs, HMI für Netzwerkkonfigurations- und Diagnosezwecke.

# 1.3.3 EtherNet/IP

In diesem Kapitel werden die Eigenschaften und Einstellungsmethoden von EtherNet/IP Master (Scanner) und Slave (Adapter) beschrieben.

<br>

##### EtherNet/IP – Übersicht

EtherNet/IP ist ein offenes industrielles Kommunikationsprotokoll auf Ethernet-Basis, das von CI (ControlNet International) und ODVA (Open DeviceNet Vendors Association) entwickelt wurde.

In der Fabrik können verschiedene Geräte wie Sensoren, Remote-E/A, Motortreiber, HMI, SPS und Robotersteuerungen unabhängig vom Hersteller an ein EtherNet/IP-Netzwerk angeschlossen werden.

![[Abbildung 1.3.3-1 EtherNet/IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/image_1.png>)
 

<br>

EtherNet/IP wird entsprechend seiner Kommunikationsfunktion wie folgt klassifiziert.

##### Scanner Class
   * Produkte, die bestehenden Feldbus-Mastern entsprechen und E/A-Datenverbindungen zu EtherNet/IP-Adaptern oder -Scannern anfordern können.

<br>

##### Adapter Class
  * Produkte, die bestehenden Feldbus-Slaves entsprechen und die Ziele von Echtzeit-E/A-Datenverbindungen sind, die von EtherNet/IP-Scannern angefordert werden.
    
  * Adapter können ohne den Scanner keine Echtzeit-E/A-Daten selbst senden und empfangen.

<br>

##### Messaging Class
   * Produkte, die explizite Nachrichten für alle Klassenprodukte senden und empfangen können, jedoch keine Echtzeit-E/A-Datenübertragung und -empfang unterstützen.
   
   * Beispiele hierfür sind Computerschnittstellenkarten für das Hoch- und Herunterladen von Programmen, Netzwerkkonfigurationstools usw.
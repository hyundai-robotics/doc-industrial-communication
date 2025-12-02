
## 1. PROFINET ?
- PROFINET ist ein Ethernet-basierter Kommunikationsstandard für die industrielle Automatisierung.
- Er unterstützt den Echtzeit-Datenaustausch zwischen Steuerungen (SPS, Robotersteuerungen usw.) und dezentralen E/A-Geräten (Antriebe, Sensoren, Module usw.).

## 2. PROFINET-Spezifikationen
- Digitale Eingänge: 50, 120, 240 Bytes (bitte eine Option auswählen)
- Digitale Ausgänge: 50, 120, 240 Bytes (bitte eine Option auswählen)
- Sicherheits-E/A: 8/8 Byte (aktiviert oder deaktiviert)
- Mindestkommunikationszyklus: 1 ms
- Unterstützte Kommunikationsgeschwindigkeit: 10 oder 100 MBit/s
- Conformance Class : B
- Netload Class : II
- Optional Feature : Legacy, MRP

## 3. PROFINET-Konfigurationsverfahren

1) Anschluss von BD671, PROFINET-Controller und Hi7 Com
2) Registrierung der GSDML-Datei (TIA Portal)
3) PROFINET-Controller-Einstellungen (TIA Portal)
4) Hi7-Einstellungen (TP UI)
5) Überprüfung der PROFINET-Kommunikation
6) Zuweisung der PROFINET-E/A-Signale (FB-Block-Einstellungen)

### 3.1 Anschluss von BD671, F-Host und Hi7 Com

#### 3.1.1 LAN-Kabelverbindung
1) Verbinden Sie den PROFINET-Controller und BD671 mit einem LAN-Kabel.
2) Überprüfen Sie, ob die Link-LED blinkt.
3) Verbinden Sie den LAN3-Anschluss von Hi7 COM und BD671 mit einem LAN-Kabel.
4) Überprüfen Sie, ob die Link-LED blinkt.

![](../_assets/4-pnio/profisafe_connect.png)

#### 3.1.2 Hi7 Com-Verbindungseinstellungen
1) Navigieren Sie wie folgt zum Menü: System -> Steuerungsparameter -> Industrielle Kommunikation -> EtherCAT-Master-Einstellungen
2) Konfigurieren Sie wie unten gezeigt
- EtherCAT Master : ON
- Port : LAN3
3) Wählen Sie „OptionBD – PROFINET_IO” aus der Slave-Liste aus und drücken Sie die Schaltfläche „Übernehmen”.
4) Starten Sie die Hi7-Robotersteuerung neu.
5) Überprüfen Sie nach dem Neustart den Status der LEDs „Run“, „Communication“ und „Error“.

![](../_assets/4-pnio/EC_master_setting1.png)
<br> <br>
![](../_assets/4-pnio/EC_master_setting2.png)


### 3.2 Registrierung der GSDML-Datei (TIA-Portal)
1) Starten Sie das TIA Portal.
2) Navigieren Sie wie rechts im Menü gezeigt zu [Optionen] → [Allgemeine Stationsbeschreibungsdatei (GSD) verwalten].
3) Klicken Sie auf die Schaltfläche „…“ und legen Sie das Verzeichnis fest, in dem sich die GSDML-Datei befindet.
4) Wählen Sie „GSDML-V2.43-Hyundai-Robotics-HI6-20250418.xml” aus der auf dem Bildschirm angezeigten Liste aus und klicken Sie auf die Schaltfläche [Installieren].
5) Überprüfen Sie, ob die Datei als neues Gerät im Hardwarekatalog registriert wurde. <br>
![](../_assets/4-pnio/profisafe_gsdmal.png)

### 3.3 PROFINET-Controller-Einstellungen (TIA-Portal)
1) Starten Sie TIA Portal und erstellen Sie ein neues Projekt.
2) Doppelklicken Sie auf den Abschnitt „Geräte & Netzwerk“, um ihn zu öffnen.<br>
![](../_assets/4-pnio/profisafe_device_network.png)

3) Wählen Sie eine Steuerung aus, die die PROFINET-Kommunikation unterstützt (z. B. CPU 1511F-1 PN), und ziehen Sie sie in die Netzwerkansicht.
4) Fügen Sie das im vorherigen Schritt hinzugefügte Gerät (HRC, PROFINET I/O DAP) aus dem Hardwarekatalog hinzu und ziehen Sie es in die Netzwerkansicht.
5) Verbinden Sie die beiden Geräte, indem Sie die LAN-Ports in den Geräteabbildungen per Drag & Drop verschieben.<br>
![](../_assets/4-pnio/profisafe_device_network2.png)

6) Doppelklicken Sie im Bildschirm „Geräte & Netzwerk“ auf das HRC-IO-Gerät.
7) Wählen Sie den gewünschten Slot aus.
8) Ziehen Sie das gewünschte Modul (DI, DO oder PROFIsafe-E/A) aus dem rechten Katalog und verschieben Sie es in das Fenster „Geräteübersicht“.<br>
![](../_assets/4-pnio/profisafe_device_network3.png)

9) Doppelklicken Sie im Bildschirm „Geräte & Netzwerk“ auf das HRC-IO-Gerät.
10) Klicken Sie erneut auf das HRC-IO-Gerät, um den Bildschirm „Einstellungen“ zu öffnen.
11) Navigieren Sie zur Registerkarte „Allgemein“ unten.
12) Wählen Sie im linken Menü „Ethernet-Adressen“ aus.
13) Deaktivieren Sie „PROFINET-Gerätenamen automatisch generieren“.
14) Setzen Sie „PROFINET-Gerätename“ auf „hd-hrc-0“ und speichern Sie die Einstellung.<br>
![](../_assets/4-pnio/profisafe_device_network4.png)

### 3.4 Hi7-Einstellungen (TP-Benutzeroberfläche)
1) Legen Sie die Parameter mit denselben Werten fest, die im PNIO-Controller konfiguriert sind.
- PROFINET IO Device Name : hd-hrc-0
- Slot 1 : Digital Input : 240
- Slot 2 : Digital Output : 240
- Slot 3 : Safety I/O : No
- (Die IP-Adresse muss nicht geändert werden.)
2) Klicken Sie auf die Schaltfläche „Übernehmen“.<br>
![](../_assets/4-pnio/4_1_profinet_config.png)

### 3.5 Überprüfung der PROFINET-Kommunikation
### 3.5.1 Ladder-Programm (TIA-Portal)
1) Erstellen Sie auf der Registerkarte „Geräteübersicht“ ein Ladder-Programm wie unten gezeigt und laden Sie es auf die Steuerung herunter.<br>
![](../_assets/4-pnio/5_1_Safety_Ladder.png)
2) Überprüfen Sie nach dem Herunterladen, ob auf dem Bildschirm „Verteilungs-E/A“ ein grünes Häkchen angezeigt wird.<br>
![](../_assets/4-pnio/5_1_Safety_Ladder2.png)

### 3.5.2 TP-Bildschirm
Navigieren Sie im Menü zu „System“ -> „Sicherheitssystem“ -> „Überwachung“ -> „PROFINET-Status“.<br>
![](../_assets/4-pnio/5_2_pnio_status.png)
- Überprüfen Sie die Statusinformationen für jeden Slot.
- Überprüfen Sie, ob der Zähler kontinuierlich ansteigt.


### 3.6 Zuweisung der PROFINET-E/A-Signale (FB-Block-Einstellungen)
1) Navigieren Sie zu System → Steuerungsparameter → Ein-/Ausgangssignal-Einstellungen → FB-Block-Zuweisung.
2) Ändern Sie die Blockeinstellungen nach Bedarf auf PROFINET-E/A (maximal 2).
(최대 PROFINET I/O 사이즈는 240바이트이고 개별 FB 블럭의 사이즈는 120바이트 입니다. 따라서 **(Die maximale PROFINET-E/A-Größe beträgt 240 Byte und die Größe des einzelnen FB-Blocks beträgt 120 Byte. Daher werden Einstellungen, die 2 überschreiten, ignoriert.)<br>**)<br>
![](../_assets/4-pnio/6_fb_block.png)

3) Navigieren Sie zusätzlich zum Menü „Bedingungseinstellungen“ und überprüfen Sie, ob der SPS-Betriebsmodus auf AUS steht.<br>
![](../_assets/4-pnio/6_1_condition.png)
4) Überprüfen Sie die Ein-/Ausgangssignale im TIA-Portal und auf dem Bildschirm „Allgemeine E/A“<br>
![](../_assets/4-pnio/6_3_public_io.png)

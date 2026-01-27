## 2.6.1 Verbindung mit der LS ELECTRIC-SPS

In diesem Abschnitt wird erläutert, wie Sie die LS ELECTRIC-SPS mit Hi6 EtherNet/IP verbinden.  
Die unten verwendete SPS und das Kommunikationsmodul sind wie folgt.  
(SPS: XGI-CPUS, Kommunikationsmodul: XGL-EFMTB)

**2.6.1.1 Ausführen von XG5000**
![xg5000.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/xg5000.png) <br>
*[Abbildung 2.6.1.1 Ausführen von XG5000]*<br>
Das XG5000-Programm und detaillierte Anweisungen zur Verwendung können Sie von der LS ELECTRIC-Website herunterladen.

**2.6.1.2 Registrieren der EDS-Datei**
Wählen Sie „Menü > Extras > EDS(D) > EDS-Datei registrieren“. Wählen Sie „Hi6_EIP_240402.eds“ aus.<br>
Bestätigen Sie die Registrierung der EDS-Datei wie in der Abbildung unten gezeigt<br>
![eds.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/eds.png)<br>
*[Abbildung 2.6.1.2 EDS-Datei registrieren]*<br>


**2.6.1.3 Geräteverbindung**
[1] Projekt erstellen<br>
![newProject_1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_1.png)<br>
*[Abbildung 2.6.1.3 Neues Projekt erstellen]*<br>

[2] Kommunikationsmodul hinzufügen<br>
![newProject_2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_2.png)<br>
*[Abbildung 2.6.1.4 Kommunikationsmodul 1 hinzufügen]*<br>

![newProject_3.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_3.png)<br>
*[Abbildung 2.6.1.5 Kommunikationsmodul 2 hinzufügen]*<br>

![newProject_4.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_4.png)<br>
*[Abbildung 2.6.1.6 Kommunikationsmodul 3 hinzufügen]*<br>

[3] Einstellungen für das Kommunikationsmodul <br>
Doppelklicken Sie auf XGL-EFMT, das in der Abbildung unten auf der linken Registerkarte angezeigt wird.<br>
![newProject_6.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_6.png)<br>
*[Abbildung 2.6.1.7 Einstellungen für das Kommunikationsmodul]*<br>
- Konfigurieren Sie die IP-Adresse, die Subnetzmaske, das Gateway usw.  
- Um die beiden LAN-Ports der SPS als Relaisfunktion zu verwenden, aktivieren Sie das Kontrollkästchen „Relais“.  
- Ändern Sie die RAPIEnet-Einstellung auf „Deaktivieren“.

**2.6.1.4 Online-Verbindungseinstellungen**
[1] Verbinden Sie die SPS mit einem USB-Kabel.<br>
![newProject_7.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_7.png)<br>
*[Abbildung 2.6.1.8 Online-Verbindungseinstellungen 1]*<br>

[2] Drücken Sie die Schaltfläche links in der Abbildung unten, um die gesamte Konfiguration herunterzuladen.<br>
![newProject_8.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_8.png)<br>
*[Abbildung 2.6.1.9 Online-Verbindungseinstellungen 2]*<br>

**2.6.1.5 Automatischer Scan**
[1] Der automatische Scan ist möglich, wenn eine Verbindung zur SPS besteht.<br>
Wenn Sie derzeit nicht online sind, klicken Sie auf „Menü“ > „Online“ > „Verbinden“, um in den Online-Status zu wechseln.<br>

[2] Klicken Sie mit der rechten Maustaste auf XGL-EFMT > Element hinzufügen > Klicken Sie auf „Smart Expansion“<br>
![auto1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto1.png)<br>
*[Abbildung 2.6.1.10 Automatischer Scan 1]*<br>

[3] Klicken Sie auf „Weiter“  <br>
![auto2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto2.png)<br>
*[Abbildung 2.6.1.11 Automatischer Scan 2]*<br>

[4] Klicken Sie auf „Automatischer Scan“.<br>
![auto3.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto3.png)<br>
*[Abbildung 2.6.1.12 Automatischer Scan 3]*<br>

![auto4.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto4.png)<br>
*[Abbildung 2.6.1.13 Automatischer Scan4]*<br>

[5] Überprüfen Sie die automatisch gescannten Geräte.  
![auto5.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto5.png)<br>
*[Abbildung 2.6.1.14 Automatischer Scan5]*<br>

![auto6.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto6.png)<br>
*[Abbildung 2.6.1.15 Automatischer Scan6]*<br>

Das Hi6 EtherNet/IP-Adaptergerät wird in der Liste angezeigt, wie in der Abbildung unten dargestellt. <br>
![auto7.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto7.png)<br>
*[Abbildung 2.6.1.16 Automatischer Scan7]*<br>

**2.6.1.6 Registrierung von Programmvariablen**
[1] Programm scannen > Neues Programm > Lokale Variablen (Doppelklick)<br>
![variable1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/variable1.png)<br>
*[Abbildung 2.6.1.17 Variablenregistrierung 1]*<br>

[2] Konfigurieren Sie die Eingangs-/Ausgangsdaten, die für die Kommunikation verwendet werden sollen.<br>
![variable2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/variable2.png)<br>
*[Abbildung 2.6.1.18 Variablenregistrierung 2]*<br>

**2.6.1.7 EtherNet/IP-Adaptereinstellungen**
[1] Doppelklicken Sie in der linken Liste auf EB01 (Hi6 EtherNet/IP-Adapter).<br>

[2] Klicken Sie auf die Schaltfläche „EIP-Detaileinstellungen“.<br>
![AdapterSetting1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting1.png)<br>
*[Abbildung 2.6.1.19 EtherNet/IP-Adapter-Einstellungen 1]*<br>

[3] Wählen Sie anhand der folgenden Abbildung die Einstellungen für den EtherNet/IP-Adapter aus. <br>
- Verbindungstyp
- T2O RPI Range, O2T RPI Range
- T2O Input, O2T Output size
- Übertragungszyklus
- Zeitüberschreitung
- Lokales Tag, Remote-Tag <br>
![AdapterSetting2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting2.png) <br>
*[Abbildung 2.6.1.20 EtherNet/IP-Adapter-Einstellungen 2]*<br>

[4] Online > Einstellungen und Diagnose des Kommunikationsmoduls > Klicken Sie auf „Service aktivieren“<br>
![AdapterSetting3.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting3.png)<br>
*[Abbildung 2.6.1.21 EtherNet/IP-Adapter-Einstellungen 3]*<br>

[5] Aktivieren Sie das Kontrollkästchen „FEnet I/O Service“<br>
![AdapterSetting4.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting4.png)<br>
*[Abbildung 2.6.1.22 EtherNet/IP-Adapter-Einstellungen 4]*<br>

<br>

**2.6.1.8 E/A-Block nach Abschluss der Kommunikationseinstellungen zuweisen**

{% hint style="info" %}
\.      **Nach Abschluss der Kommunikationseinstellungen können Sie Eingangs-/Ausgangssignale verwenden, indem Sie E/A-Blöcke zuweisen. Bitte beachten Sie („[**4. Zuweisung von E/A-Blöcken für die industrielle Kommunikation**](../../4-io-block-allocation.md)“).**
{% endhint %}
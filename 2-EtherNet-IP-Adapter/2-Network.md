## 2.2 EtherNet/IP-Adapter-Netzwerkeinstellungen

**2.2.1 Hi6 Com**
Die LAN-Ports, die mit dem EtherNet/IP-Adapter verbunden werden können, sind LAN1/LAN2/LAN3.<br>

![hi6com.png](../_assets/2-EtherNet-IP-Adapter/Network/hi6com.png)<br>
*[Abbildung 2.2.1 Hi6 Com]*<br>

**2.2.2 Netzwerkeinstellungen**
Nachdem Sie den LAN-Port für die EtherNet/IP-Kommunikation ausgewählt haben, überprüfen Sie die Einstellungen dieses LAN-Ports über den TP-Bildschirm wie unten gezeigt und ändern Sie die Einstellungen nach Bedarf.<br>

![networkConfig.png](../_assets/2-EtherNet-IP-Adapter/Network/networkConfig.png)<br>
*[Abbildung 2.2.2 Netzwerkeinstellungen]*<br>

{% hint style="info" %}
\.      Die IP-Adressen von LAN1/LAN2/LAN3 müssen jeweils unterschiedliche Subnetz-Teile aufweisen.

\.      Starten Sie nach dem Ändern der Einstellungen die Robotersteuerung neu.
{% endhint %}

**2.2.3 Überprüfung des Verbindungsstatus**
Der physische Verbindungsstatus mit dem EtherNet/IP-Scanner kann anhand des Link/Act-LED-Status des LAN-Ports überprüft werden.<br>

![lanPort.png](../_assets/2-EtherNet-IP-Adapter/Network/lanPort.png)<br>
*[Abbildung 2.2.3 LAN-Port]*<br>

Überprüfen Sie nach dem Anschließen des EtherNet/IP-Adapters und des Scanners mit einem LAN-Kabel den LED-Status. Wenn die LED auf der linken Seite nicht leuchtet oder blinkt, liegt ein Problem mit dem Kabel, dem Adapter oder dem Scanner vor. Bitte überprüfen Sie den Verbindungsstatus des Kabels oder Geräts.<br>

**2.2.4 Netzwerkkonfiguration**
Es wird empfohlen, das EtherNet/IP-Netzwerk und das Fabriknetzwerk als separate Netzwerke zu konfigurieren. Wie in der folgenden Abbildung dargestellt, teilen sich EtherNet/IP-Netzwerk und Fabriknetzwerk bei einer Konfiguration als ein Netzwerk ein Übertragungsmedium, was zu einer erhöhten Netzwerkauslastung führt. Daher wird empfohlen, nach Möglichkeit ein separat konfiguriertes Netzwerk für das EtherNet/IP-Netzwerk zu verwenden.<br>

![NG_Network.png](../_assets/2-EtherNet-IP-Adapter/Network/NG_Network.png)<br>
*[Abbildung 2.2.4 Nicht getrenntes Netzwerk]*<br>

![Good_Network.png](../_assets/2-EtherNet-IP-Adapter/Network/Good_Network.png)<br>
*[Abbildung 2.2.5 Getrenntes Netzwerk]*<br>

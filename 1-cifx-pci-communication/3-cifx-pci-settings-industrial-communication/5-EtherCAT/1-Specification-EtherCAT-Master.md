# 1.3.5.1 EtherCAT-Master-Spezifikationen

<br>

##### Protokollmerkmale

| **Kategorie**                       | **Spezifikationen**                  |
| :---                           | :---                     |
| Maximal anschließbare Slaves       | 200                      |
| Maximale Eingangsbyte-Größe            | 1200 Bytes (FB Block Max) |
| Maximale Ausgangsbyte-Größe            | 1200 Bytes (FB Block Max) |
| Maximale Eingangsbyte-Größe (pro Slave)| 256 Bytes                 |
| Maximale Ausgangsbyte-Größe (pro Slave)| 256 Bytes                 |
| E/A-Verbindung                        |                           |
| Minimale E/A-Zykluszeit             | 250 µs (1 ms empfohlen)   |
| Kommunikationsgeschwindigkeit                      | 100 Mbit/s (Full-Duplex)  |
| Auto Negotiation               | Nicht unterstützt                    |
| Quick Connect                  | Nicht unterstützt                    |
| Topologie                      | Linie, Ring               |
| Redundanz                     | Unterstützt (kann nicht gleichzeitig mit Synchronisation angewendet werden) |
| Synchronisation                         | Distributed Clocks        |

<br>

##### Netzwerkmerkmale

| **Kategorie**                      | **Spezifikationen**                  |
| :---                          | :---                     |
| Network Slave Scan            | Unterstützt                      |
| Data Transport Layer          | Ethernet II, IEEE 802.3   |
| Hub                           | Nicht verfügbar                |
| Switch                        | Eingeschränkte Verwendung möglich (zwischen Master und erstem Slave) |

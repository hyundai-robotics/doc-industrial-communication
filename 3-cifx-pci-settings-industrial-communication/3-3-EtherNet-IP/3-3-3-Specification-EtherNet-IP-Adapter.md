# 3.3.3 EtherNet/IP Adapter 사양

<br>

##### Protocol 특성

| **구분**                   | **사양**                  |
| :---                       | :---                      |
| 최대 입력 Bytes 크기        | 240 Bytes (TP) / 504 Bytes (Sycon.net)|
| 최대 출력 Bytes 크기        | 240 Bytes (TP) / 504 Bytes (Sycon.net)|
| IO 연결 (Implicit)         | 1 exclusive Owner, 1 Listen only, 1 Input Only |
| IO 연결                    | Cyclic, Application Trigger, Change of State   |
| IO 최소 Cycle Time         | 1ms                       |
| 통신 속도                  | 10 or 100 Mbit/s          |
| Auto Negotiation           | 지원                      |
| Quick Connect              | 지원                      |
| Topology                   | Tree, Line, Ring          |
| DLR V2 (Ring Topology)     | 지원                      |
| 부가 기능                   | DHCP, BOOTP, ACD  지원    |


<br>

##### Network 특성

| **구분**                   | **사양**                  |
| :---                       | :---                      |
| Data Transport Layer       | Ethernet II, IEEE 802.3   |
| Hub                        | 사용 가능                  |
| Switch                     | 사용 가능                  |
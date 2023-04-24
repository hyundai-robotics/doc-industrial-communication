# 3.4.1 PRFINET IO Controller 사양

<br>

##### Protocol 특성

| **구분**                       | **사양**                  |
| :---                           | :---                     |
| 최대 연결 가능한 Slave 수       | 128개                     |
| 최대 입력 Bytes 크기            | 1080 Bytes                |
| 최대 출력 Bytes 크기            | 1080 Bytes                |
| 최대 입력 Bytes 크기 (Slave 1개)| 1024 Bytes                |
| 최대 출력 Bytes 크기 (Slave 1개)| 1024 Bytes                |
| IO 연결                        |                           |
| IO 최소 Cycle Time             | 1ms                       |
| 통신 속도                       | 100 Mbit/s (Full-Duplex) |
| Auto Negotiation               | 미지원                    |
| Quick Connect                  | 미지원                    |
| Topology                       | Tree, Line               |
| DCP                            | 지원                      |



<br>

##### Network 특성

| **구분**                      | **사양**                  |
| :---                          | :---                     |
| Network Slave Scan            | 지원                      |
| Data Transport Layer          | Ethernet II, IEEE 802.3   |
| Hub                           | 사용 불가능                |
| Switch                        | 제한 사용 가능 (Priority Tagging, LLDP 지원 필요) |
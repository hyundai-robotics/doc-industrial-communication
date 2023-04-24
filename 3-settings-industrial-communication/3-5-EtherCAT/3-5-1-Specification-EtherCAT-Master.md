# 3.5.1 EtherCAT Master 사양

<br>

##### Protocol 특성

| **구분**                       | **사양**                  |
| :---                           | :---                     |
| 최대 연결 가능한 Slave 수       | 200개                      |
| 최대 입력 Bytes 크기            | 1080 Bytes                |
| 최대 출력 Bytes 크기            | 1080 Bytes                |
| 최대 입력 Bytes 크기 (Slave 1개)| 256 Bytes                 |
| 최대 출력 Bytes 크기 (Slave 1개)| 256 Bytes                 |
| IO 연결                        |                           |
| IO 최소 Cycle Time             | 250us (1ms Recommended)   |
| 통신 속도                      | 100 Mbit/s (Full-Duplex)  |
| Auto Negotiation               | 미지원                    |
| Quick Connect                  | 미지원                    |
| Topology                       | Line, Ring                |
| Redundance                     | 지원 (동기화와 동시 적용 불가) |
| 동기화                         | Distributed Clocks        |

<br>

##### Network 특성

| **구분**                      | **사양**                  |
| :---                          | :---                     |
| Network Slave Scan            | 지원                      |
| Data Transport Layer          | Ethernet II, IEEE 802.3   |
| Hub                           | 사용 불가능                |
| Switch                        | 제한 사용 가능 (Master 와 1번째 Slave 사이 ) |

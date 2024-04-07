# 3.7.1 DeviceNet Master 사양

<br>

##### Protocol 특성

| **구분**                       | **사양**                  |
| :---                           | :---                     |
| 최대 연결 가능한 Slave 수        | 63개                      |
| 최대 입력 Bytes 크기             | 1080 Bytes                |
| 최대 출력 Bytes 크기             | 1080 Bytes                |
| 최대 입력 Bytes 크기 (Slave 1개) | 255 Bytes                 |
| 최대 출력 Bytes 크기 (Slave 1개) | 255 Bytes                 |
| IO 연결                         | Bit Strobe, Change of State, Cyclic, Poll |
| IO 최소 Cycle Time              |                           |
| 통신 속도                       | 125 ~ 500 Kbit/s          |
| Auto Baud Rate Detection        | 미지원                    |
| Quick Connect                   | 지원                      |
| Topology                        |                           |



<br>

##### Network 특성

| **구분**                       | **사양**                   |
| :---                           | :---                      |
| Network Slave Scan             | 지원                      |
| Data Transport Layer           | CAN frames                |
| Hub                            | 해당 없음                  |
| Switch                         | 해당 없음                  |

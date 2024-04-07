# 3.7.3 DeviceNet Slave 사양


<br>

##### Protocol 특성

| **구분**                   | **사양**                  |
| :---                       | :---                      |
| 최대 입력 Bytes 크기        | 255 Bytes                 |
| 최대 출력 Bytes 크기        | 255 Bytes                 |
| IO 연결 (Implicit)         |                           |
| IO 연결                    | Bit Strobe, Change of State, Cyclic, Poll |
| IO 최소 Cycle Time         |                           |
| 통신 속도                  | 125 ~ 500 Kbit/s          |
| Auto Baud Rate Detection   | 미지원                    |
| Quick Connect              |                          |
| Topology                   |                          |


<br>

##### Network 특성

| **구분**                       | **사양**                   |
| :---                           | :---                      |
| Data Transport Layer           | CAN frames                |
| Hub                            | 해당 없음                  |
| Switch                         | 해당 없음                  |
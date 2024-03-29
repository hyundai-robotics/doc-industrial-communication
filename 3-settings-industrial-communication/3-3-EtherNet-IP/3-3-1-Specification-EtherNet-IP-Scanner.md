﻿# 3.3.1 EtherNet/IP Scanner 사양

<br>

##### Protocol 특성

| **구분**                       | **사양**                  |
| :---                           | :---                     |
| 최대 연결 가능한 Slave 수        | 64개                      |
| 최대 입력 Bytes 크기             | 1080 Bytes                |
| 최대 출력 Bytes 크기             | 1080 Bytes                |
| 최대 입력 Bytes 크기 (Slave 1개) | 504 Bytes                 |
| 최대 출력 Bytes 크기 (Slave 1개) | 504 Bytes                 |
| IO 연결                         | Cyclic                    |
| IO 최소 Cycle Time              | 1ms                       |
| 통신 속도                       | 10 or 100 Mbit/s          |
| Auto Negotiation                | 지원                      |
| Quick Connect                   | 지원                      |
| Topology                        | Tree, Line, Ring          |
| DLR (Device Level Ring)         | Beacon based 'Ring Node'  |
| 부가 기능                        | DHCP, BOOTP, ACD  지원    |


<br>

##### Network 특성

| **구분**                       | **사양**                  |
| :---                           | :---                     |
| Network Slave Scan             | 미지원                    |
| Data Transport Layer           | Ethernet II, IEEE 802.3   |
| Hub                            | 사용 가능                  |
| Switch                         | 사용 가능                  |
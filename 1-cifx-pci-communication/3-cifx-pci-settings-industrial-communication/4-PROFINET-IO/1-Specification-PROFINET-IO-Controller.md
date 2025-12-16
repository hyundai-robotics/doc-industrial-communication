# 1.3.4.1 PROFINET IO Controller 规格

<br>

##### 协议特性

| **区分**                       | **规格**                  |
| :---                           | :---                     |
| 最大可连接的Slave数 | 128个 |
| 最大输入字节数            | 1200 Bytes （FB Block Max）|
| 最大输出字节数            | 1200 Bytes （FB Block Max）|
| 最大输入字节数（1个Slave）| 1024 Bytes                |
| 最大输出字节数（1个Slave）| 1024 Bytes                |
| IO连接                        |                           |
| IO 最小Cycle Time             | 1ms                       |
| 通信速度                       | 100 Mbit/s (Full-Duplex) |
| Auto Negotiation               | 不支持                    |
| Quick Connect                  | 不支持                    |
| Topology                       | Tree, Line               |
| DCP                            | 支持                      |



<br>

##### 网络特性

| **区分**                      | **规格**                  |
| :---                          | :---                     |
| Network Slave Scan            | 支持                      |
| Data Transport Layer          | Ethernet II, IEEE 802.3   |
| Hub                           | 不可使用                |
| Switch                        | 可限制使用（需支持Priority Tagging、LLDP） |
# 1.3.3.1 EtherNet/IP Scanner规格

<br>

##### 协议特性

| **区分**                       | **规格**                  |
| :---                           | :---                     |
| 最大可连接的Slave数        | 64个                      |
| 最大输入字节数             | 1200 Bytes (FB Block Max) |
| 最大输出字节数             | 1200 Bytes (FB Block Max) |
| 最大输入字节数（1个Slave） | 504 Bytes                 |
| 最大输出字节数（1个Slave） | 504 Bytes                 |
| IO连接                         | Cyclic                    |
| IO 最小Cycle Time              | 1ms                       |
| 通信速度                       | 10 or 100 Mbit/s          |
| Auto Negotiation                | 支持                      |
| Quick Connect                   | 支持                      |
| Topology                        | Tree, Line, Ring          |
| DLR (Device Level Ring)         | Beacon based 'Ring Node'  |
| 附加功能                        | 支持DHCP、BOOTP、ACD    |


<br>

##### 网络特性

| **区分**                       | **规格**                  |
| :---                           | :---                     |
| Network Slave Scan             | 不支持                    |
| Data Transport Layer           | Ethernet II, IEEE 802.3   |
| Hub                            | 可使用                  |
| Switch                         | 可使用                  |
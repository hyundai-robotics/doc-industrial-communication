#### 1.3.5.1 EtherCAT Master 规格

<br>

**协议特性**

| **区分**                       | **规格**                  |
| :---                           | :---                     |
| 最大可连接的Slave数 | 200个 |
| 最大输入字节数            | 1200 Bytes （FB Block Max）|
| 最大输出字节数            | 1200 Bytes （FB Block Max）|
| 最大输入字节数（1个Slave）| 256 Bytes                 |
| 最大输出字节数（1个Slave）| 256 Bytes                 |
| IO连接                        |                           |
| IO 最小Cycle Time             | 250us（1ms Recommended）   |
| 通信速度                      | 100 Mbit/s（Full-Duplex）  |
| Auto Negotiation               | 不支持                    |
| Quick Connect                  | 不支持                    |
| Topology                       | Line, Ring                |
| Redundance                     | 支持（不能与同步化同时应用） |
| 同步化                         | Distributed Clocks        |

<br>

**网络特性**

| **区分**                      | **规格**                  |
| :---                          | :---                     |
| Network Slave Scan            | 支持                      |
| Data Transport Layer          | Ethernet II, IEEE 802.3   |
| Hub                           | 不可使用                |
| Switch                        | 可限制使用（Master与第1个Slave之间） |

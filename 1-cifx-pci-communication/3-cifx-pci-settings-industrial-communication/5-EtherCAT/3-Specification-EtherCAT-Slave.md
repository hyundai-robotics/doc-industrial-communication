#### 1.3.5.3 EtherCAT Slave规格

<br>

**协议特性**

| **区分**                   | **规格**                  |
| :---                       | :---                     |
| 最大输入字节数        | 256 Bytes                |
| 最大输出字节数        | 256 Bytes                |
| IO连接（Implicit）         |                          |
| IO连接                    |                          |
| IO 最小 Cycle Time         | 250us（1ms Recommended）  |
| 通信速度                  | 100 Mbit/s               |
| Auto Negotiation           | 不支持                   |
| Quick Connect              | 不支持                   |
| Topology                   | Line, Ring               |
| 同步化                     | Distributed Clocks       |


<br>

**网络特性**

| **区分**                   | **规格**                  |
| :---                       | :---                      |
| Data Transport Layer       | Ethernet II, IEEE 802.3   |
| Hub                        | 不可使用                |
| Switch                     | 可限制使用（Master与第1个Slave之间） |

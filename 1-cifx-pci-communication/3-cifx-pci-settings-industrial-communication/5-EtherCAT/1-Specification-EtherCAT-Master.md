# 1.3.5.1 EtherCAT Master Specifications

<br>

##### Protocol Characteristics

| **| Category                       | Specifications                  |**                       | **| Category                       | Specifications                  |**                  |
| :---                           | :---                     |
| Maximum Connectable Slave Count       | 200개                      |
| Maximum Input Byte Size            | 1200 Bytes (FB Block Max) |
| Maximum Output Byte Size            | 1200 Bytes (FB Block Max) |
| Maximum Input Byte Size (Per Slave)| 256 Bytes                 |
| Maximum Output Byte Size (Per Slave)| 256 Bytes                 |
| IO Connection                        |                           |
| IO Minimum Cycle Time             | 250us (1ms Recommended)   |
| Communication Speed                      | 100 Mbit/s (Full-Duplex)  |
| Auto Negotiation               | Not supported                    |
| Quick Connect                  | Not supported                    |
| Topology                       | Line, Ring                |
| Redundance                     | Supported (Cannot be applied simultaneously with synchronization) |
| Synchronization                         | Distributed Clocks        |

<br>

##### Network Characteristics

| **| Category                      | Specifications                  |**                      | **| Category                      | Specifications                  |**                  |
| :---                          | :---                     |
| Network Slave Scan            | Supported                      |
| Data Transport Layer          | Ethernet II, IEEE 802.3   |
| Hub                           | Not available                |
| Switch                        | Limited use possible (Between Master and 1st Slave) |

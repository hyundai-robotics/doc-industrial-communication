# 3.5.1 Specifications of the EtherCAT Master

<br>

##### Protocol Characteristics

| **Classification**                       | **Specification**                  |
| :---                           | :---                     |
| Maximum connectable slave count       | 200                      |
| Maximum input byte size            | 1080 bytes                |
| Maximum output byte size            | 1080 bytes                |
| Maximum input byte size (1 slave)| 256 bytes                 |
| Maximum output byte size (1 slave)| 256 bytes                 |
| IO connection                       |                           |
| Minimum IO cycle time             | 250 us (1 ms recommended)   |
| Communication speed                      | 100 Mbit/s (Full-Duplex)  |
| Auto negotiation               | Not supported                   |
| Quick connect                  | Not supported                   |
| Topology                       | Line, Ring                |
| Redundance                     | Supported (cannot be applied together with synchronization) |
| Synchronization                         | Distributed Clocks        |

<br>

##### Network Characteristics

| **Classification**                      | **Specification**                  |
| :---                          | :---                     |
| Network slave scan            | Supported                      |
| Data transport layer          | Ethernet II, IEEE 802.3   |
| Hub                           | Cannot be used                |
| Switch                        | Limited use is allowed (between the master and slave 1) |

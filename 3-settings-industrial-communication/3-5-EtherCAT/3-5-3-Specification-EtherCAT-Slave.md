# 3.5.3 Specifications of an EtherCAT Slave

<br>

##### Protocol Characteristics

| **Classification**                   | **Specification**  
| :---                       | :---                     |
| Maximum input byte size       | 256 bytes                |
| Maximum output byte size        | 256 bytes                |
| IO connection (implicit)         |                          |
| IO connection                    |                          |
| Minimum IO cycle time         | 250 us (1 ms is recommended)  |
| Communication speed                  | 100 Mbit/s               |
| Auto negotiation           | Not supported                   |
| Quick connect              | Not supported                   |
| Topology                   | Line, Ring               |
| Synchronization                     | Distributed Clocks       |


<br>

##### Network Characteristics

| **Classification**         | **Specification**                  |
| :---                       | :---                      |
| Data transport layer       | Ethernet II, IEEE 802.3   |
| Hub                        | Cannot be used                         |
| Switch                     | Limited us is allowed (between the master and slave 1) |

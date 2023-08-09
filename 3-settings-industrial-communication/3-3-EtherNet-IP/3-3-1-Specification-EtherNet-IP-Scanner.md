# 3.3.1 Specifications of an EtherNet/IP Scanner

<br>

##### Protocol Characteristics

| **Classification**                  | **Specification**             |
| :---                                | :---                           |
| Maximum connectable slave count     | 64                             |
| Maximum input byte size             | 1080 bytes                     |
| Maximum output byte size            | 1080 bytes                     |
| Maximum input byte size (1 slave)   | 504 bytes                      |
| Maximum output byte size (1 slave)  | 504 bytes                      |
| IO connection                       | Cyclic                         |
| Minimum IO cycle time               | 1 ms                           |
| Communication speed                 | 10 or 100 Mbit/s               |
| Auto negotiation                    | Supported                      |
| Quick connect                       | Supported                      |
| Topology                            | Tree, Line, Ring               |
| Device Level Ring (DLR)             | Beacon-based "Ring Node"       |
| Additional functions                | DHCP, BOOTP, and ACD-supported |


<br>

##### Network Characteristics

| **Classification**                  | **Specification**       |
| :---                                | :---                     |
| Network slave scan                  | Not supported            |
| Data transport layer                | Ethernet II, IEEE 802.3  |
| Hub                                 | Can be used              |
| Switch                              | Can be used              |
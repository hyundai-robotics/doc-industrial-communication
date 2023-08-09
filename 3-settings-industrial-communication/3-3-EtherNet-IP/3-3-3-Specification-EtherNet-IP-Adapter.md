# 3.3.3 Specifications of an EtherNet/IP Adapter

<br>

##### Protocol Characteristics

| **Classification**           | **Specification**                             |
| :---                         | :---                                           |
| Maximum input byte size      | 240 bytes (TP) / 504 bytes (SYCON.net)         |
| Maximum output byte size     | 240 bytes (TP) / 504 bytes (SYCON.net)         |
| IO connection (implicit)     | 1 exclusive Owner, 1 Listen only, 1 Input Only |
| IO connection                | Cyclic, Application Trigger, Change of State   |
| Minimum IO cycle time        | 1 ms                                           |
| Communication speed          | 10 or 100 Mbit/s                               |
| Auto negotiation             | Supported                                      |
| Quick connect                | Supported                                      |
| Topology                     | Tree, Line, Ring                               |
| DLR V2 (Ring Topology)       | Supported                                      |
| Additional functions         | DHCP, BOOTP, and ACD-supported                 |


<br>

##### Network Characteristics

| **Classification**           | **Specification**        |
| :---                         | :---                      |
| Data transport layer         | Ethernet II, IEEE 802.3   |
| Hub                          | Can be used               |
| Switch                       | Can be used               |
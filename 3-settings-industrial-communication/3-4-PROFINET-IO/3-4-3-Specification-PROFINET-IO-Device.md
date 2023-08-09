# 3.4.3 Specifications of a PROFINET IO Device

<br>

##### Protocol Characteristics

| **Classification**           | **Specification**                     |
| :---                         | :---                                   |
| Maximum input byte size      | 256 bytes (TP) / 1024 Bytes (SYCON.net)|
| Maximum output byte size     | 256 bytes (TP) / 1024 Bytes (SYCON.net)|
| IO connection(implicit)      |                                        |
| IO connection                |                                        |
|  Minimum IO cycle time       | 1 ms                                   |
|  Communication speed         | 100 Mbit/s                             |
| Auto negotiation             | Not supported                          |
| Quick connect                | Not supported                          |
| Topology                     | Tree, Line                             |
| DCP                          | Supported                              |


<br>

##### Network Characteristics

| **Classification**           | **Specification**                  |
| :---                         | :---                                |
| Data transport layer         | Ethernet II, IEEE 802.3             |
| Hub                          | Cannot be used                      |
| Switch                       | Limited use is allowed (Priority Tagging and LLDP need to be supported) |


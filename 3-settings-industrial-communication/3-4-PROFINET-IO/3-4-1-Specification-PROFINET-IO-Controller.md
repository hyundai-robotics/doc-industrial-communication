# 3.4.1 Specifications of the PROFINET IO Controller

<br>

##### Protocol Characteristics

| **Classification**                     | **Specification**        |
| :---                                   | :---                      |
| Maximum connectable slave count        | 128                       |
| Maximum input byte size                | 1080 bytes                |
| Maximum output byte size               | 1080 bytes                |
| Maximum input byte size (1 slave)      | 1024 bytes                |
| Maximum output byte size (1 slave)     | 1024 bytes                |
| IO connection                          |                           |
| Minimum IO cycle time                  | 1 ms                      |
| Communication speed                    | 100 Mbit/s (Full-Duplex)  |
| Auto negotiation                       | Not supported             |
| Quick connect                          | Not supported             |
| Topology                               | Tree, Line                |
| DCP                                    | Supported                 |



<br>

##### Network Characteristics

| **Clssification**                      | **Specification**        |
| :---                                   | :---                      |
| Network slave scan                     | Supported                 |
| Data transport layer                   | Ethernet II, IEEE 802.3   |
| Hub                                    | Cannot be used            |
| Switch                                 | Limited use is allowed (Priority Tagging and Link Layer Discovery Protocol (LLDP) need to be supported)       |
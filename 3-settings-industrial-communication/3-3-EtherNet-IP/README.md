# 3.3 EtherNet/IP

This chapter describes the characteristics of the EtherNet/IP master (scanner) and slave (adapter) and the methods to set them.

<br>

##### EtherNet/IP Overview

EtherNet/IP is an Ethernet-based, open industrial communications protocol developed by ControlNet International (CI) and the Open DeviceNet Vendors Association (ODVA).

In a factory, various devices, such as sensors, remote IOs, motor drivers, human-machine interfaces (HMIs), programmable logic controllers (PLCs), and robot controllers, can be connected to one EtherNet/IP network regardless of the manufacturer.

![[Figure 3.3-1 EtherNet/IP]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/image_1.png>) 

<br>

EtherNet/IP can be classified into following classes according to communication functions.

##### Scanner Class
   * The products of this class correspond to existing fieldbus masters and can send requests for I/O data connections to an EtherNet/IP adapter or EtherNet/IP scanner.

<br>

##### Adapter Class
  * The products of this class correspond to existing fieldbus slaves. They also correspond to the targets of the connection of real-time I/O data requested by an EtherNet/IP scanner.
    
  * Without relying on a scanner, an adapter cannot send/receive real-time I/O data by itself. 

<br>

##### Messaging Class
   * The products of this class can send and receive explicit messages for products of all classes and do not support the sending and receiving of real-time I/O data.
   
   * For example, products of this class may include computer interface cards for program uploads/downloads and network configuration tools.
# 2. EtherNet/IP

This chapter describes the characteristics and configuration methods of the built-in EtherNet/IP Master (Scanner) and Slave (Adapter).
<br>

**EtherNet/IP Overview**

<br>

EtherNet/IP is an Ethernet-based open industrial communication protocol developed by CI (ControlNet International) and ODVA (Open DeviceNet Vendors Association)

In a factory environment, various devices such as sensors, remote I/Os, motor drivers, HMIs, PLCs and robot controllers can be connected to a single EtherNet/IP network, regardless of the manufacturer.

![[Figure 2-1 EtherNet/IP]](<../_assets//2-ethernet-ip/image_1.png>)
 

<br>

EtherNet/IP is classified as follows based on its communication functions:

**Scanner Class**

   * These products correspond to traditional Fieldbus Masters and can request I/O data connections from EtherNet/IP Adapters or Scanners.

<br>

**Adapter Class**

  * These products correspond to traditional Fieldbus Slaves and serve as the connection targets for real-time I/O data requested by an EtherNet/IP Scanner.
    
  * An Adapter cannot transmit or receive real-time I/O data on its own without a request from a Scanner.

<br>

**Messaging Class**

   * These products are capable of sending and receiving explicit messages to and from products of all classes, but they do not support real-time I/O data transmission.
   
   * Examples include computer interface cards for program upload/download and network configuration tools.

<br>

**Abbreviation**

<br>

|Abbreviation|Description|
|---------------|------------------------------|
|Adapter|A device that collects output data from and transmits input data to an EtherNet/IP Scanner|
|Scanner|A device that sends output data to and collects input data from end devices (EtherNet/IP Adapters)|
|LAN| Local Area Network|
|RPI|Requested Packet Interval|
|PLC|Programmable logic controller|
|T2O|Target to Originator (Adapter -> Scanner)|
|O2T|Originator to Target (Scanner -> Adapter)|

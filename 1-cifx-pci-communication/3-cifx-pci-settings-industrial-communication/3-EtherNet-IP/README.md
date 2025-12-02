# 1.3.3 EtherNet/IP

This chapter describes the characteristics of the EtherNet/IP master (scanner) and slave (adapter) and how to set them.

<br>

##### EtherNet/IP Overview

EtherNet/IP is an Ethernet-based open industrial communication protocol developed by CI (ControlNet International) and ODVA (Open DeviceNet Vendors Association).

In the factory, various devices such as sensors, remote IOs, motor drivers, HMIs, PLCs, and robot controllers can be connected to one EtherNet/IP network regardless of manufacturer.

![[Figure 1.3.3-1 EtherNet/IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/image_1.png>)
 

<br>

EtherNet/IP is classified as follows according to the communication function.

##### Scanner Class
   * Products that correspond to existing fieldbus masters and can ask the EtherNet/IP adapters or scanners to perform I/O data connection.

<br>

##### Adapter Class
  * Products that correspond to existing fieldbus slaves and are the targets of Real-Time I/O data connections requested by EtherNet/IP scanners.
    
  * An adapter cannot send and receive Real-Time I/O data on their own without the scanner.

<br>

##### Messaging Class
   * Products that can send and receive explicit messages for the products of all classes, but do not support Real-Time I/O data transmission and reception.
   
   * For example, the products can be computer interface cards for program upload/download and network setting tools, etc.
# 1.3.9 CC-Link IE Field

This chapter describes the characteristics of CC-Link IE field slaves and how to set them.


<br>

##### Fieldbus Overview

Fieldbus is an industry standard that has been opened for connecting devices such as sensors, buttons, motor drivers, and operation interfaces to PLCs (Programmable Logic Controllers) with a single cable and operating them in factories.

Fieldbus provides intelligent services such as central monitoring of the status of the entire network status and reconfiguration of the network.

For example, it is possible to set detailed information, operations, and modes for sensors and switches , not just simple On/Off.

Using a single cable reduces time and costs for wiring, simplifies the configuration, and provides advantage in maintenance.

Also, unlike protocols with non-deterministic response characteristics of general communications, fieldbuses guarantee data response speed to satisfy industrial applications where critical time characteristics are important.

![[Figure 1.3.9-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/image_1.png>)

<br>

One fieldbus network connects one master device and multiple slave devices.
The master device searches and manages the entire network and exchanges data with slave devices.

Generally, a PLC is a master device, while sensors, buttons, controllers, etc. can be configured as slave devices.

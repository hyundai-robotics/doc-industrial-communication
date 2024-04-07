# 3.7 DeviceNet

This chapter describes the characteristics of DeviceNet masters and slaves and the methods to set them.

<br>

##### Fieldbus Overview

Fieldbus is an open industry standard for operating devices such as sensors, buttons, motor drivers, and operation interfaces in a factory by connecting them to a PLC using a single cable.

Fieldbus provides intelligent services such as monitoring the status of the entire network or reconfiguring it from a central location.

For example, Fieldbus makes it possible to set detailed information, operation, and modes of sensors and switches, not just their simple on/off operations.

The use of a single cable helps reduce the time and cost of wiring and makes the configuration simple, which is advantageous for maintenance. 

Moreover, unlike other protocols that have characteristics of the non-deterministic response of general communication, Fieldbus guarantees data response speed, satisfying industrial applications where the characteristics of critical time are important.

![[Figure 3.7-1 Fieldbus]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/image_1.png>) 

<br>

One master and multiple slaves can be connected to one Fieldbus network.
The master device searches/manages the entire network and exchanges data with slave devices.

In general, a PLC is a master device, and other devices such as sensors, buttons, and controllers can be configured as slave devices.
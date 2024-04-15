# 3.8.1 Specifications of a CC-Link Slave

<br>

##### Protocol Characteristics

| **Classification**         | **Specification**  (Version 1.11)    | **Specification**  (Version 2.0)  |
| :---                       | :---                                 | :---                              |
| Maximum input byte size    | 48 bytes                             | 368 bytes                         |
| Maximum output byte size   | 48 bytes                             | 368 bytes                         |
| IO station input           | 4 bytes(RY)                          | Not supported                     |
| IO station output          | 4 bytes(RX)                          | Not supported                     |
| Station                    | 1–4                                  | 1–4                               |
| Extension cycle            | Not supported                        | 1, 2, 4, and 8                    |
| Remote device input        | 16 bytes (RY), 32 bytes (RWw)        | 112 bytes (RY), 256 bytes (RWw)   |
| Remote device output       | 16 bytes (RX), 32 bytes (RWr)        | 112 bytes (RY), 256 bytes (RWr)   |
| Communication speed        | 156 Kbit/s–10000 Kbit/s              | 156 Kbit/s–10000 Kbit/s           |



<br>

##### Network Characteristics

| **Classification**            | **Specification**     |
| :---                          | :---                  |
| Data transport layer          |                       |
| Hub                           | None                  |
| Switch                        | None                  |


<br>

##### CC-Link IO Mapping

<br>

{% hint style="info" %}
\.        CC-Link Version 1
{% endhint %}

<br>

![[Figure 3.8.1-1 CC-Link IO Mapping]](<../../_assets/3-cifx-pci-settings-industrial-communication/3.8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Single
{% endhint %}

<br>

![[Figure 3.8.1-2 CC-Link IO Mapping]](<../../_assets/3-cifx-pci-settings-industrial-communication/3.8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Double
{% endhint %}

<br>

![[Figure 3.8.1-2 CC-Link IO Mapping]](<../../_assets/3-cifx-pci-settings-industrial-communication/3.8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Quadruple
{% endhint %}

<br>

![[Figure 3.8.1-2 CC-Link IO Mapping]](<../../_assets/3-cifx-pci-settings-industrial-communication/3.8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Octuple
{% endhint %}

<br>

![[Figure 3.8.1-2 CC-Link IO Mapping]](<../../_assets/3-cifx-pci-settings-industrial-communication/3.8-CC-Link/3-Slave_spec/image_5.png>)

<br>
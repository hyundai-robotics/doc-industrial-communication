# 1.3.8.1 CC-Link Slave Specifications

<br>

##### Protocol Characteristics

| **Category**                   | **Specifications** (Version 1.11)    | **Specifications** (Version 2.0)     |
| :---                       | :---                       | :---                        |
| Maximum Input Byte Size        | 48 Bytes                   | 368 Bytes                   |
| Maximum Output Byte Size        | 48 Bytes                   | 368 Bytes                   |
| IO Station Input           | 4 Bytes (RY)               | Not supported                       |
| IO Station Output          | 4 Bytes (RX)               | Not supported                       |
| Station                    | 1-4                        | 1-4                         |
| Extension Cycle            | Not supported                      | 1, 2, 4, 8                  |
| Remote Deivce Input        | 16 Bytes(RY), 32 Byte(RWw) | 112 Bytes(RY), 256 Byte(RWw)|
| Remote Deivce Output       | 16 Bytes(RX), 32 Byte(RWr) | 112 Bytes(RY), 256 Byte(RWr)|
| Communication Speed                   | 156–10000 Kbit/s         | 156–10000 Kbit/s          |



<br>

##### Network Characteristics

| **Category**                       | **Specifications**                   |
| :---                           | :---                      |
| Data Transport Layer           |                           |
| Hub                            | Not applicable                  |
| Switch                         | Not applicable                  |


<br>

##### CC-Link IO Mapping

<br>

{% hint style="info" %}
\.        CC-Link Version 1
{% endhint %}

<br>

![[Figure 1.3.8.1-1 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Single
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Double
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle: Quadruple
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Octuple
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_5.png>)

<br>
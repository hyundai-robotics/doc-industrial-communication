# 1.3.8.1 CC-Link Slave 规格

<br>

##### 协议特性

| **区分**                   | **规格**  (Version 1.11)    | **规格**  (Version 2.0)     |
| :---                       | :---                       | :---                        |
| 最大输入字节数        | 48 Bytes                   | 368 Bytes                   |
| 最大输出字节数        | 48 Bytes                   | 368 Bytes                   |
| IO Station Input           | 4 Bytes(RY)                | 不支持                       |
| IO Station Output          | 4 Bytes(RX)                | 不支持                       |
| Station                    | 1 ～ 4                      | 1 ～ 4                       |
| Extension Cycle            | 不支持                      | 1, 2, 4, 8                  |
| Remote Deivce Input        | 16 Bytes(RY), 32 Byte(RWw) | 112 Bytes(RY), 256 Byte(RWw)|
| Remote Deivce Output       | 16 Bytes(RX), 32 Byte(RWr) | 112 Bytes(RY), 256 Byte(RWr)|
| 通信速度                   | 156 ～ 10000 Kbit/s         | 156 ～ 10000 Kbit/s          |



<br>

##### 网络特性

| **区分**                       | **规格**                   |
| :---                           | :---                      |
| Data Transport Layer           |                           |
| Hub                            | 不适用                  |
| Switch                         | 不适用                  |


<br>

##### CC-Link IO映射

<br>

{% hint style="info" %}
\.        CC-Link Version 1
{% endhint %}

<br>

![[图 1.3.8.1-1 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Single
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Double
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Quadruple
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Octuple
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_5.png>)

<br>
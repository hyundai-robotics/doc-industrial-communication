# 3.8.1 CC-Link Slave 사양

<br>

##### Protocol 특성

| **구분**                   | **사양**  (Version 1.11)    | **사양**  (Version 2.0)     |
| :---                       | :---                       | :---                        |
| 최대 입력 Bytes 크기        | 48 Bytes                   | 368 Bytes                   |
| 최대 출력 Bytes 크기        | 48 Bytes                   | 368 Bytes                   |
| IO Station Input           | 4 Bytes(RY)                | 미지원                       |
| IO Station Output          | 4 Bytes(RX)                | 미지원                       |
| Station                    | 1 ~ 4                      | 1 ~ 4                       |
| Extension Cycle            | 미지원                      | 1, 2, 4, 8                  |
| Remote Deivce Input        | 16 Bytes(RY), 32 Byte(RWw) | 112 Bytes(RY), 256 Byte(RWw)|
| Remote Deivce Output       | 16 Bytes(RX), 32 Byte(RWr) | 112 Bytes(RY), 256 Byte(RWr)|
| 통신 속도                   | 156 ~ 10000 Kbit/s         | 156 ~ 10000 Kbit/s          |



<br>

##### Network 특성

| **구분**                       | **사양**                   |
| :---                           | :---                      |
| Data Transport Layer           |                           |
| Hub                            | 해당 없음                  |
| Switch                         | 해당 없음                  |


<br>

##### CC-Link IO 맵핑

<br>

{% hint style="info" %}
\.        CC-Link Version 1
{% endhint %}

<br>

![[그림 3.8.1-1 CC-Link IO Mapping]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Single
{% endhint %}

<br>

![[그림 3.8.1-2 CC-Link IO Mapping]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Double
{% endhint %}

<br>

![[그림 3.8.1-2 CC-Link IO Mapping]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Quadruple
{% endhint %}

<br>

![[그림 3.8.1-2 CC-Link IO Mapping]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Octuple
{% endhint %}

<br>

![[그림 3.8.1-2 CC-Link IO Mapping]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/3-Slave_spec/image_5.png>)

<br>
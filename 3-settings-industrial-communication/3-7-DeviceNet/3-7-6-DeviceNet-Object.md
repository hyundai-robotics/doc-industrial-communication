# 3.7.6 DeviceNet Object


<br>

##### 1. Object


DeviceNet의 장치 내부에는 Object 의 집합체로 구성이 되어있습니다. 각 Object 는 장치 내부에의 특정한 구성요소를 표현합니다.

<br>

![[그림 3.7.6-1 DeviceNet Object]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/6-Object/image_1.png>) 


<br>

Object는 Class Code 를 이용하여 구분합니다.

<br>

![[그림 3.7.6-2 DeviceNet Object]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/6-Object/image_2.png>)

<br>

Object 내부에는 Instance 번호와 Attribute ID로 구성되어 있습니다.

<br>

DeviceNet Master 에서 Explicit Message를 통해 특정 Slave의 Object 에 접근할 수 있습니다.

<br>

{% hint style="info" %}
\.      EX) Crevis GN-9212 의 Object (해당 자료는 Crevis 매뉴얼에서 확인 하실 수 있습니다.)

\.      Identity Object (Class Code 0x01) 의 Vendor ID 값 읽기

\.      Instance : 1

\.      Attribute ID : 1

\.      권한 : Get (읽기만 가능)
{% endhint %}


![[그림 3.7.6-3 DeviceNet Object Crevis GN-9212]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/6-Object/image_3.png>)


<br>

각 Object 와 내부의 Instance 및 Attribute 마다 모두 각기 다른 접근 권한을 가지고 있습니다.

<br>

{% hint style="info" %}
\.      접근 권한

\.      Get : 읽기 권한

\.      Set : 쓰기 권한 

\.      Attribute Single : 한번에 1개의 Attribute 항목만 접근 가능

\.      Attribute All : 한번에 Instance내의 모든 Attribute 접근 가능
{% endhint %}

<br>
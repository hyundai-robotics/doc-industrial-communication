# 3.7.5 DeviceNet 에러 조치

<br>

"[**4.1 ERROR Code**](../../4-monitoring-industrial-communication/4-1-error-code.md)" 참고해 주십시오.

<br>

##### 1. DeviceNet 종단 저항

{% hint style="info" %}
\.      DeviceNet Cable 연결 시 종단에는 저항을 추가해야합니다.

\.      Network Scan이 안되는 경우 종단 저항을 확인해 주십시오.

\.      DeviceNet 종단 저항 : 120옴
{% endhint %}

{% hint style="info" %}
\.      아래 그림과 같이 CIFX-50 DN PCI가 DeviceNet의 종단인 경우 종단 저항을 추가해 주십시오.
{% endhint %}

![[그림 3.7.5-1 DeviceNet 종단 저항]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/5-Error/image_1.png>) 

{% hint style="info" %}
\.      아래 그림과 같이 DeviceNet Remote IO 가 종단인 경우 종단 저항을 추가하거나 DIP Switch를 조작해 주십시오.
{% endhint %}

![[그림 3.7.5-2 DeviceNet 종단 저항]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/5-Error/image_2.png>) 

<br>

##### 2. 통신 속도

{% hint style="info" %}
\.      DeviceNet Master와 Slave 간 통신 속도가 다른 경우 Network Scan이 안될 수 있습니다.

\.      Network Scan이 안되는 경우 통신 속도를 확인해 주십시오.
{% endhint %}

![[그림 3.7.5-3 DeviceNet Baudrate]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/5-Error/image_3.png>) 

<br>

##### 3. DeviceNet ERROR

{% hint style="info" %}
\.      DeviceNet Cable에 24V 전원 공급이 안되는 경우 아래와 같은 ERROR가 나타납니다.

\.      24V 전원 공급을 확인해 주십시오.
{% endhint %}

![[그림 3.7.5-4 DeviceNet Error]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/5-Error/image_4.png>) 
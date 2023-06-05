# 3.10.1 EtherNet/IP - 표준 Remote IO 연결 설정

“[**3.1 산업용 통신 펌웨어 설정**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

##### 1. 산업용 통신 펌웨어 설정에서 EtherNet/IP Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 3.10.1-1 펌웨어 설정]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

![[그림 3.10.1-2 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

##### 3. 통신을 위해 PCI와 Remote IO의 Cable 등을 연결하고 상태를 확인합니다.

![[그림 3.10.1-3 하드웨어 연결]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[그림 3.10.1-4 하드웨어 연결]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

<br>

{% hint style="info" %}
\.      PCI 와 Remote IO를 LAN Cable을 이용하여 연결해 주십시오.

\.      Remote IO 의 DIP Switch는 모두 OFF로 설정해 주십시오.

\.      Remote IO 전원과 Field Power를 모두 연결해 주십시오. (24V DC)
{% endhint %}

<br>

{% hint style="info" %}
\.      Remote IO Crevis M9289 의 공장 출하시 설정 IP는 192.168.100.99 입니다.

\.      Remote IO 의 IP가 192.168.100.99 로 설정되어 있어야 통신 연결이 가능합니다.

\.      “[**3.10.2 Remote IO IP Setting**](../../3-settings-industrial-communication/3-10-EtherNet-IP-Remote-IO/3-10-2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

##### 4. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: 슬레이브 구성 >  EtherNet/IP Remote IO Setting]**

![[그림 3.10.1-5 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>) 

![[그림 3.10.1-6 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>) 

<br>

{% hint style="info" %}
\.      IP는 고정값으로 설정되어 있습니다.

\.      Input, Output Byte 수를 확인합니다.

\.      선택한 Input, Output 수가 Remote IO Slot에 장착된 카드의 IO 수 보다 작거나 같아야 합니다.
{% endhint %}

<br>

{% hint style="info" %}
\.      Input Module  
\.      M12DF : Digital 16점  
\.      M3534 : Analog 4점  
{% endhint %}

{% hint style="info" %}
\.      Output Module  
\.      M225F : Digital 16점  
\.      M226F : Digital 16점  
\.      M2768 : Digital 8점   
\.      M4534 : Analog 4점  
{% endhint %}

{% hint style="info" %}
\.      Special Module  
\.      M5112 : Conveyer I/F 
{% endhint %}

<br>

##### 5. 설정 완료 후 제어기를 재부팅합니다.

![[그림 3.10.1-7 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>) 

![[그림 3.10.1-8 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
\.      설정 완료 후 제어기를 재부팅해 주십시오.
{% endhint %}

<br>

##### 6. 설정값이 반영되어있는지 후, 통신 상태를 확인합니다.

![[그림 3.10.1-9 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>) 

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**4 산업용 통신 모니터링**](../../4-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[그림 3.10.1-10 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>) 

{% hint style="info" %}
\.      통신 연결이 안되는 경우 Remote IO의 IP를 확인해야합니다.

\.      아래를 따라 확인해 주십시오. (192.168.100.99 가 아닌 경우)

\.      “[**3.10.2 Remote IO IP Setting**](../../3-settings-industrial-communication/3-10-EtherNet-IP-Remote-IO/3-10-2-Settings-Remote-IO-IP.md)"
{% endhint %}

![[그림 3.10.1-11 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>) 

![[그림 3.10.1-12 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>) 
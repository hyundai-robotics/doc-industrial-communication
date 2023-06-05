# 3.8.2 CC-Link Slave 설정

“[**3.1 산업용 통신 펌웨어 설정**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      CC-Link Connector 연결은 아래를 참고해 주십시오.

\.      (“[**2.2 커넥터**](../../2-mounting-settings-industrial-communication-card/2-2-Connector.md)”)
{% endhint %}

<br>

##### 1. TP를 이용하여 산업용 통신 펌웨어 설정에서 CC-Link Slave를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 3.8.4-1 펌웨어 설정]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.

![[그림 3.8.4-2 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

##### 3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: 슬레이브 구성 >  CC-Link Slave]**

![[그림 3.8.4-3 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/4-Slave_setting/image_3.png>) 

![[그림 3.8.4-4 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

##### 4. 각 항목별 설명

{% hint style="info" %}
\.      [Station Address]

\.      CC-Link는 Station Address를 통해 Slave를 식별합니다. (1 ~ 64)
{% endhint %}

{% hint style="info" %}
\.      [통신 속도(Baudrate)]

\.      156, 625, 2500, 5000, 10000 Kbit/s  중 선택 가능합니다.
{% endhint %}

{% hint style="info" %}
\.      [CC-Link Version]

\.      Version 1 : IO Station 사용 가능, Extension Cycle 사용 불가

\.      Version 2 : IO Station 사용 불가, Extension Cycle 사용 가능
{% endhint %}

{% hint style="info" %}
\.      [점유 Station 수]

\.      IO Station : 1개 점유

\.      Remote Device : 1 ~ 4 개 선택 가능 

\.      점유하는 Station 수에 따라 할당되는 IO Byte 영역의 크기가 달라집니다.
{% endhint %}

{% hint style="info" %}
\.      [Extension Cycle]

\.      Version 2에서 사용 가능

\.      Remote Device : 1배(Single), 2배(Double), 4배(Quadruple), 8배(Octuple) 선택 가능 

\.      Extension Cycle에 따라 할당되는 IO Byte 영역의 크기가 달라집니다.
{% endhint %}

<br>

{% hint style="info" %}
\.      **IO Byte 영역에 대해서는 아래 링크를 참고해 주십시오.**

\.      **(“[**3.8.1 CC-Link Slave 사양**](../../3-settings-industrial-communication/3-8-CC-Link/3-8-1-Specification-CC-Link-Slave.md)”)**
{% endhint %}

<br>

##### 5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**4 산업용 통신 모니터링**](../../4-monitoring-industrial-communication/README.md)”)참고해 주십시오.

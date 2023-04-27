# 3.3.4 EtherNet/IP Adapter 설정

“[**3.1 산업용 통신 펌웨어 설정**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.


<br>

##### 1. TP를 이용하여 산업용 통신 펌웨어 설정에서 EtherNet/IP Slave를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 3.3.4-1 펌웨어 설정]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.

![[그림 3.3.4-2 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

##### 3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: 슬레이브 구성 >  EtherNet/IP Slave]**

![[그림 3.3.4-3 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[그림 3.3.4-4 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

##### 4. 각 항목 별 설명

{% hint style="info" %}
\.      [IP 설정 (IP Setting)]

\.      고정 IP : 사용자가 IP 주소, 서브넷 마스크, 게이트 웨이 정보를 설정합니다.

\.      동적할당(DHCP) : DHCP 서버에서 IP 주소를 할당 받습니다.
{% endhint %}

{% hint style="info" %}
\.      [통신 에러시 입력 (Action in Bus Error)]

\.      Clear : 통신 에러 발생시 모든 입력을 0 으로 초기화 합니다.

\.      Hold : 통신 에러 발생시 마지막 유효 입력 값을 유지합니다.
{% endhint %}

{% hint style="info" %}
\.      [통신 에러 허용시간 (Error Allowed Time)]

\.      지정한 허용 시간동안 통신에러가 지속되면 필드버스 이상 신호와 알람을 출력합니다.
{% endhint %}

{% hint style="info" %}
\.      [입력 바이트 수 (Input Byte)]

\.      입력 바이트 수 : Master -> Slave 로 입력되는 데이터 크기를 설정합니다.

\.      O -> T : Originator(Master) -> Target (Slave)
{% endhint %}

{% hint style="info" %}
\.      [출력 바이트 수 (Output Byte)]

\.      출력 바이트 수 : Slave -> Master 로 출력하는 데이터 크기를 설정합니다.

\.      T -> O : Target (Slave) -> Originator(Master)
{% endhint %}

{% hint style="info" %}
\.      [Run / Idle Header]

\.      제어기에 적용된 CIFX-50 RE EtherNet/IP Adapter 는 Scanner와 IO 교환 시 32Bit Run / Idle Header 를 사용합니다. (Default)

\.      Scanner 사양에 따라 입력 및 출력 32Bit Run / Idle Header 사용 여부를 적절히 설정하여 주십시오.
{% endhint %}

<br>

{% hint style="info" %}
\.        [Quick Connect]

\.        EtherNet/IP는 Quick Connect 기능을 지원합니다.

\.        Quick Connect 기능 사용이 필요한 경우 Sycon.net 을 이용하여 EtherNet/IP Adapter를 설정해 주십시오.

\.        (1) Master, Slave Quick Connect 지원 제품 필요  
\.        (2) Auto Negotiation 사용시 Quick Connect 사용 불가  
\.        (3) Auto MDI-X 사용시 Quick Connect 사용 불가  
\.        (4) 100 Mbit/s, Full Duplex 사용 필요  
{% endhint %}

<br>

##### 5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**4 산업용 통신 모니터링**](../../4-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[그림 3.3.4-5 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/4-Slave_setting/image_5.png>) 
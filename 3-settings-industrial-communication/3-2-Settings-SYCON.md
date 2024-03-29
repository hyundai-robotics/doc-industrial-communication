﻿# 3.2 SYCON.NET 설정

Hi6 제어기는 “**Sycon.net**” 프로그램을 이용하여 산업용 통신 설정을 진행합니다. 설정 방법은 다음과 같습니다. (“[**1.1 Sycon.net 설치**](../1-install-program/1-1-sycon-net.md)”을 참고하여 설치해주시기 바랍니다.)

<br>

##### 1. 통신 설정 관련 참고 자료입니다.
**\“Sycon.net v1.0500\DVD\_2018-12-1\_1\_0500\Documentation\4. Training Material\EN”** 자료들을 참고 할 수 있습니다.
   *   참고자료

       1\) EtherNetIP Scanner - Configuration and Testing TM 02 EN.pdf

       2\) PROFIBUS DP Master - Configuration and Testing TM 02 EN.pdf

       3\) PROFINET IO Controller - Configuration and Testing TM 02 EN.pdf

<br>

##### 2. Sycon.net 설치된 PC와 로봇 제어기의 범용 LAN포트를 연결 합니다. (PCI LAN Port X)
**\[시스템 > 2: 제어 파라미터 > 9: 네트워크]** 메뉴룰 터치하여 범용 LAN포트의 IP를 확인합니다. Ping Test 등을 통해 연결 여부를 확인해 주십시오.

![[그림 3.2-1 네트워크 IP]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_1.png>) 

{% hint style="info" %}
\.      IP Address는 사용자 설정에 따라 변경 가능합니다.
{% endhint %}

<br>

##### 3. Sycon.net 을 실행합니다.

![[그림 3.2-2 Sycon.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_2.png>)

<br>

##### 4. 화면 오른쪽 Device Catalog 에서 설정한 통신 Protocol에 맞는 항목을 클릭하여 Drag & Drop 으로 중앙의 버스 라인에 놓습니다. 

![[그림 3.2-3 Sycon.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_3.png>)
![[그림 3.2-4 Sycon.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_4.png>)

<br>

##### 5. 가져온 항목을 더블클릭하여 설정합니다.

{% hint style="info" %}
\.      가져온 CIFX PCI (그림) “Double Click”

\.      Settings -> Driver 

\.      netX Driver를 선택합니다.
{% endhint %}

![[그림 3.2-5 Sycon.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_5.png>)

{% hint style="info" %}
\.     Setting -> Driver -> netX Driver -> TCP Connection 

\.     IP Address : 연결된 제어기의 범용 LAN Port IP 주소를 입력해 주십시오.
{% endhint %}

![[그림 3.2-6 Sycon.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_6.png>)

{% hint style="info" %}
\.      Device Assignment -> Scan클릭

\.      통신(Channel Protocol 확인)을 선택 후 “Apply” 이후 “OK”
{% endhint %}

{% hint style="warning" %}
**\[주의]**: Channel Protocol 과 Slot 번호를 반드시 확인해 주십시오.
{% endhint %}

{% hint style="warning" %}
**\[주의]**: Scan 이 안되는 경우 제어기와의 Cable 연결 상태, 펌웨어 설정을 확인해 주십시오.
{% endhint %}

![[그림 3.2-7 Sycon.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_7.png>)


{% hint style="info" %}
\.      CIFX PCI 그림 우클릭 -> DOWNLOAD
{% endhint %}

![[그림 3.2-8 Sycon.net]](<../_assets/3-Settings-Industrial-Communication/3.2-Setting-SYCON/image_8.png>)
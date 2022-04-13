# 3.2.1 Sycon.net 사용 방법

Hi6 제어기의 산업용 통신을 사용할 경우 “**Sycon.net**” 프로그램을 이용하여 통신 설정을 해주어야 합니다. 설정 방법은 다음과 같습니다. (“[**1.1 Sycon.net**](../../1-install-program/1-1-sycon-net.md)”을 참고하여 설치해주시기 바랍니다.)

1. Hi6Com(협동로봇 : Hi6MiniCom)의 LAN3포트를 PC와 연결 합니다.
2. 통신 설정 방법은 “Sycon.net v1.0500\DVD\_2018-12-1\_1\_0500\Documentation\4. Training Material\EN” 안에 파일들을 참고 하시면 됩니다.
   *   참고파일 이름

       1\) EtherNetIP Scanner - Configuration and Testing TM 02 EN.pdf

       2\) PROFIBUS DP Master - Configuration and Testing TM 02 EN.pdf

       3\) PROFINET IO Controller - Configuration and Testing TM 02 EN.pdf

{% hint style="info" %}
1\.      Hi6 Driver를 연결하기 netX Driver 설정 방법 예시 입니다.

2\.      IP Address는 제어기 설정에 맞추어 설정 하시면 됩니다.

3\.      EtherCAT Master 설정 방법 (CIFX 카드 연결)
{% endhint %}

![](<../../_assets/image (6).png>)

{% hint style="info" %}
4\.      연결한CIFX 카드(그림) “Double Click”

5\.      Driver -> Netx Driver 설정
{% endhint %}

![](<../../_assets/image (13).png>)

{% hint style="info" %}
6\.      netX Driver -> TCP Connection 다음과 같이 세팅 (IP Address는 제어기에 따라 변할 수&#x20;

&#x20;        있으니 확인 바랍니다.)
{% endhint %}

![](<../../_assets/image (19).png>)

{% hint style="info" %}
7\.      Device Assignment -> Scan클릭(아무것도 나오지 않을 경우: Device selection을 suitale&#x20;

&#x20;        only -> all로 변경 후 다시 Scan 클릭)

8\.      설정한 통신(Channel Protocol 확인)을 선택 후 “Apply” 이후 “OK”
{% endhint %}

![](<../../_assets/image (2).png>)

{% hint style="warning" %}
**\[주의]**: Access path위치가 cifX(num)\_Ch0 으로 되어 있지 않을 경우 하단의 Access path에서 변경하여 Apply)
{% endhint %}

{% hint style="info" %}
9\.      필요한 부분들을 세팅 하고 “CIFX 그림 우클릭” -> DOWNLOAD
{% endhint %}

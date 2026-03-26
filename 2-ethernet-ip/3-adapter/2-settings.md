### 2.3.2 EtherNet/IP 어댑터 (슬레이브) 설정

<br>

**1. 티칭팬던트를 통한 EtherNet/IP 어댑터의 설정 및 모니터링**

<br>

**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 3: EtherNet/IP 설정]**

<br>

![Config.PNG](../../_assets/2-ethernet-ip/3-adapter/Config.png)<br>
*[그림 2.3.1 설정]*

<br>

{% hint style="info" %}
   [프로토콜 설정]

      - OFF : EtherNet/IP 사용 안함   
      - 어댑터 : EtherNet/IP Adapter 모드   
      - 스캐너 : EtherNet/IP Scanner 모드   
      - 어댑터 + 스캐너 : EtherNet/IP Adapter + Scanner 동시 사용 모드   
{% endhint %}

<br>

{% hint style="info" %}
   [Port 설정]

      - 제어기 범용 LAN1 ~ 3 사용 가능 (상태 OK 확인 필요)
{% endhint %}

<br>

{% hint style="info" %}
   [IO 설정]

      - 입력 및 출력 바이트 수 : 0 ~ 240 바이트 설정 가능
{% endhint %}

<br>

{% hint style="info" %}
   [통신 상태 확인]   
   
      - 라이선스: 현재 라이선스 상태   
      - 실행: EtherNet/IP 기능 동작 상태 표시   
      - 통신: EtherNet/IP 통신 연결 상태 표시   
      - 에러: EtherNet/IP 오류 상태 표시   
{% endhint %}

<br>
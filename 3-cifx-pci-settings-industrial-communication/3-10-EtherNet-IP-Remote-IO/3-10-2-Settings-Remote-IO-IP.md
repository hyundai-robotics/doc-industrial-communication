# 3.10.2 Remote IO IP 주소 설정

Crevis M9289 EtherNet/IP Network Adpater 의 IP 주소 설정 방법입니다.

<br>

{% hint style="info" %}
\.      Remote IO Crevis M9289 의 공장 출하시 설정 IP는 192.168.100.99 입니다.

\.      Remote IO 의 IP를 알지 못하거나 변경이 필요한 경우 아래를 따라 주십시오.
{% endhint %}

<br>

##### 1. PC와 Remote IO를 LAN Cable을 이용해 직접 연결합니다.

![[그림 3.10.2-1 LAN 연결]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

##### 2. Remote IO Adapter의 9번 DIP Switch만 ON으로 변경합니다.

![[그림 3.10.2-2 DIP Switch]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

##### 3. Bootpsvr.exe 프로그램을 실행합니다.
   * 해당 프로그램은 Crevis 사에서 제공합니다. (홈페이지에서 IO Guide Pro 다운로드 후 설치)

![[그림 3.10.2-3 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[그림 3.10.2-4 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
\.      Start BootP를 누른 상태에서 M9289 모듈의 전원을 분리하고 다시 인가하여 재부팅합니다.
{% endhint %}

![[그림 3.10.2-5 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>


##### 4. Adapter 장치를 재부팅하면 BootpSvr.exe 프로그램에 Device 정보가 나타납니다.

![[그림 3.10.2-6 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

##### 5. Device를 선택하여 IP를 설정합니다.

![[그림 3.10.2-7 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[그림 3.10.2-8 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

##### 6. IP 설정이 끝난 Adapter의 DIP Switch를 모두 OFF로 변경한 후 장치를 재부팅합니다.

{% hint style="info" %}
\.      DIP Switch의 상태 Adapter 재부팅 여부를 반드시 확인해 주십시오.
{% endhint %}

![[그림 3.10.2-9 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

##### 7. PC 에서 Ping Test 등을 이용하여 IP를 확인합니다.

![[그림 3.10.2-10 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

##### 8. IP 주소가 정상적으로 변경이 되었다면 설정을 진행합니다.

{% hint style="info" %}
\.      "[**3.10.1 EtherNet/IP - 표준 Remote IO 연결 설정**](../../3-settings-industrial-communication/3-10-EtherNet-IP-Remote-IO/3-10-1-Settings-EtherNet-IP-Remote-IO.md)" 절차를 따라 설정을 진행해 주십시오.
{% endhint %}

## 2.3.2 EtherNet/IP 스캐너 (마스터) 설정

<br>

#### 지원 버전 미정

<br>

“[**2.1 네트워크 설정**](../../2-ethernet-ip/1-network.md)" 및 "[**2.2 라이선스 설정**](../../2-ethernet-ip/2-license.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

##### 1. 메뉴를 터치하여 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 3: EtherNet/IP 설정]**

<br>

![[그림 2.3.2-1 스캐너 설정]](<../../_assets/2-ethernet-ip/3-scanner/img_1.png>) 

<br>

![[그림 2.3.2-2 스캐너 설정]](<../../_assets/2-ethernet-ip/3-scanner/img_2.png>) 

<br>

{% hint style="info" %}
\.      [Protocol 설정]

\.      * OFF : EtherNet/IP 사용 안함   
\.      * Adapter : EtherNet/IP Adapter 모드   
\.      * Scanner : EtherNet/IP Scanner 모드   
\.      * Adapter + Scanner : EtherNet/IP Adapter + Scanner 동시 사용 모드    (같은 LAN Port)
{% endhint %}

{% hint style="info" %}
\.      [Port 설정]

\.      * 제어기 범용 LAN1 ~ 3 사용 가능 (상태 OK 확인 필요)
{% endhint %}

<br>

##### 2. Scanner 모드를 선택하고 "장치 추가(Add Device)" 버튼을 눌러 다음 화면으로 진입합니다.

<br>

![[그림 2.3.2-3 스캐너 장치 추가]](<../../_assets/2-ethernet-ip/3-scanner/img_3.png>) 

<br>

##### 3. 연결할 장치와 동일하게 설정을 입력하고 저장합니다.

<br>

{% hint style="info" %}
\.      [장치 설정]

\.      * Device No. : 장치 연결 순서 (IO 데이터 배치 순서)   
\.      * IP Address : 장치의 IP 주소   
\.      * Device Name : 장치 이름 (통신 연결과는 무관, 단순 식별용)   
\.      * RPI (ms) : IO 데이터 갱신 주기   

\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      * Run/Idle Header : IO 데이터 헤더 유무 선택   
\.      * Instance No. : IO 데이터 교환을 위한 Input / Output Assembly의 Instance 번호   
\.      * IO Size : IO 데이터 크기 (bytes 단위)   
{% endhint %}

<br>

{% hint style="info" %}
\.      예시에서는 3개의 Adapter 장치를 연결합니다.    
\.      - Crevis M9289 Remote IO   
\.      - Crevis M9289 Remote IO   
\.      - CIFX PCI EtherNet/IP Adapter    
{% endhint %}

<br>

{% hint style="info" %}
\.      예시의 Remote IO의 IP 설정은 아래 매뉴얼 링크를 참조하여 진행해 주십시오.

\.      “[**1.3.10.2 Remote IO IP Setting**](../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

![[그림 2.3.2-4 Remote IO 연결]](<../../_assets/2-ethernet-ip/3-scanner/img_4.png>) 

<br>

![[그림 2.3.2-5 Remote IO 연결]](<../../_assets/2-ethernet-ip/3-scanner/img_5.png>) 

<br>

![[그림 2.3.2-6 Remote IO 연결]](<../../_assets/2-ethernet-ip/3-scanner/img_6.png>) 

<br>

![[그림 2.3.2-7 Remote IO 연결]](<../../_assets/2-ethernet-ip/3-scanner/img_7.png>) 

<br>

{% hint style="info" %}
\.      연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      [Adapter 1]   
\.      Crevis M9289   
\.      - M7002 : None   
\.      - M2768 : O > T 1bytes   
\.      - M2768 : O > T 1bytes   
\.      - M12DF : T > O 2bytes   
\.      - M12DF : T > O 2bytes   
\.      - M2768 : O > T 1bytes   
\.      - M2768 : O > T 1bytes   

\.      [IO Assembly 정보]   
\.      [T > O]   
\.      - Size: 4bytes   
\.      - Instance: 1   
\.      - Run/Idle Header: No   
\.
\.      [O > T]    
\.      - Size: 4bytes   
\.      - Instance: 2   
\.      - Run/Idle Header: 32Bit   
{% endhint %}

<br>

![[그림 2.3.2-8 스캐너 장치 추가]](<../../_assets/2-ethernet-ip/3-scanner/img_8.png>) 

<br>

![[그림 2.3.2-9 Remote IO 연결]](<../../_assets/2-ethernet-ip/3-scanner/img_9.png>) 

<br>

{% hint style="info" %}
\.      연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      [Adapter 2]   
\.      Crevis M9289   
\.      - M7001 : T > O  1 bytes   
\.      - M12DF : T > O  2 bytes   
\.      - M12DF : T > O  2 bytes   
\.      - M225F : O > T  2 bytes   
\.      - M225F : O > T  2 bytes   
\.      - M225F : O > T  2 bytes   
\.      - M2628 : O > T  1 bytes   
\.      - M2618 : O > T  1 bytes   
\.      - M5112 : T > O  14 bytes / O > T  2 bytes    


\.      [IO Assembly 정보]   
\.      [T > O]   
\.      - Size: 19 bytes   
\.      - Instance: 1   
\.      - Run/Idle Header: No   
\.
\.      [O > T]    
\.      - Size: 10 bytes   
\.      - Instance: 2   
\.      - Run/Idle Header: 32Bit   
{% endhint %}

<br>

{% hint style="info" %}
\.      같은 방법으로 PCI Adapter도 IO Size와 설정 정보를 입력합니다.   
{% endhint %}

<br>


![[그림 2.3.2-10 스캐너 장치 추가]](<../../_assets/2-ethernet-ip/3-scanner/img_10.png>) 

<br>

##### 4. OK 버튼을 눌러 통신 설정을 전송합니다.

<br>

![[그림 2.3.2-11 스캐너 설정]](<../../_assets/2-ethernet-ip/3-scanner/img_11.png>) 

<br>

##### 5. 통신이 정상적으로 연결되었는지 상태를 확인합니다.

<br>

![[그림 2.3.2-12 통신 상태 모니터링]](<../../_assets/2-ethernet-ip/3-scanner/img_12.png>) 

<br>

{% hint style="info" %}
\.      [통신 상태 확인]

\.      장치 번호 색상   
\.       - 초록색 : 통신 연결 OK   
\.       - 빨간색 : 통신 연결 NG   
{% endhint %}

<br>

![[그림 2.3.2-13 통신 상태 모니터링]](<../../_assets/2-ethernet-ip/3-scanner/img_13.png>) 

<br>

##### 6. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../5-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
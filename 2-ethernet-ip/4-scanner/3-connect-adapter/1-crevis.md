## 2.4.3.1 외부 Adapter 장치 연결 - Crevis Remote IO

<br>

{% hint style="info" %}
\.      EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

\.      “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
\.      예시의 Remote IO의 IP 설정은 아래 매뉴얼 링크를 참조하여 진행해 주십시오.

\.      “[**1.3.10.2 Remote IO IP Setting**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

**1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.**

![[그림 2.4.3.1-1 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_1.png>) 

<br>

![[그림 2.4.3.1-2 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_2.png>) 

<br>

![[그림 2.4.3.1-3 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_3.png>) 

<br>

**2. EZ-EDS 프로그램으로 EDS 파일을 열어 장치 정보를 확인합니다.**

<br>

![[그림 2.4.3.1-4 EDS 파일 정보]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_4.png>) 

<br>

{% hint style="info" %}
\.      Connection Manager에서 연결 타입 확인   
\.      * 예시에서는 Exclusive Owner

\.      Real Time Transfer Format에서 헤더 여부 확인   
\.      * Input (T > O) : 헤더 없음   
\.      * Output (O > T) : 32-bit run/idle header   

\.      Create / Decode path 를 눌러 Instance ID 확인   
{% endhint %}

<br>

![[그림 2.4.3.1-5 EDS 파일 정보]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_5.png>) 

<br>

{% hint style="info" %}
\.      * Input (T > O) : 1   
\.      * Output (O > T) : 2   
{% endhint %}

<br>

**3. 장치 매뉴얼에서 IO size를 확인합니다.**

<br>

{% hint style="info" %}
\.      현재 연결할 장치의 IO 구성 확인 
{% endhint %}

<br>

![[그림 2.4.3.1-6 Remote IO 구성]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_6.png>) 

<br>

{% hint style="info" %}
\.      슬롯 구성별 매뉴얼을 참고하여 IO size 확인
{% endhint %}

<br>

![[그림 2.4.3.1-7 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_7.png>) 

<br>

![[그림 2.4.3.1-8 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_8.png>) 

<br>

**4. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.**

<br>

![[그림 2.4.3.1-8 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_9.png>)

<br>

{% hint style="info" %}
\.      연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      [Adapter 구성]   
\.      Crevis M9289   
\.      - M7002 : None   
\.      - M2768 : 1byte (O > T)   
\.      - M2768 : 1byte (O > T)   
\.      - M12DF : 2bytes (T > O)   
\.      - M12DF : 2bytes (T > O)   
\.      - M2768 : 1byte (O > T)   
\.      - M2768 : 1byte (O > T)   

\.      [IO Assembly 정보]   
\.      [T > O]   
\.      - Size: 4bytes   
\.      - Instance: 1   
\.      - Run/Idle Header: No   

\.      [O > T]    
\.      - Size: 4bytes   
\.      - Instance: 2   
\.      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
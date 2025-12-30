## 2.4.3.2 외부 Adapter 장치 연결 - Wago Remote IO

<br>

#### 지원 버전 미정

<br>

{% hint style="info" %}
\.      EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

\.      “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
\.      해당 장치의 IP 설정은 Wago 매뉴얼을 참조하여 진행해 주십시오.
{% endhint %}

<br>

##### 1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.

![[그림 2.4.3.2-1 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_1.png>) 

<br>

##### 2. 장치 매뉴얼에서 Instance ID를 확인합니다.

<br>

![[그림 2.4.3.2-2 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_2.png>) 

<br>

{% hint style="info" %}
\.      Input (T > O)   
\.      * 104: Status  + Analog  + Digital   
\.      * 105: Status  + Digital   
\.      * 106: Status  + Analog   
\.      * 107: Analog  + Digital   
\.      * 108: Digital   
\.      * 109: Analog   

\.      Output (O > T)   
\.      * 101: Analog + Digital   
\.      * 102: Digital   
\.      * 103: Analog   
{% endhint %}

<br>

##### 2. EZ-EDS 프로그램으로 EDS 파일을 열어 장치 정보를 확인합니다.

<br>

![[그림 2.4.3.2-3 EDS 파일 정보]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_3.png>) 

<br>

{% hint style="info" %}
\.      Connection Manager에서 연결 타입 확인   
\.      * 예시에서는 Exclusive Owner

\.      Real Time Transfer Format에서 헤더 여부 확인   
\.      * Input (T > O) : 헤더 없음   
\.      * Output (O > T) : 32-bit run/idle header   
{% endhint %}

<br>

##### 3. 장치 매뉴얼에서 IO size를 확인합니다.

<br>

{% hint style="info" %}
\.      현재 연결할 장치의 IO 구성 확인 
{% endhint %}

<br>

![[그림 2.4.3.2-4 Remote IO 구성]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_4.png>) 

<br>

{% hint style="info" %}
\.      슬롯 구성별 매뉴얼을 참고하여 IO size 확인
{% endhint %}

<br>

![[그림 2.4.3.2-5 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_5.png>) 

<br>

![[그림 2.4.3.2-6 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_6.png>) 

<br>

##### 4. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.

<br>

![[그림 2.4.3.2-7 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_7.png>)

<br>

{% hint style="info" %}
\.      연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      [Adapter 구성]   
\.      Wago 750-366   
\.      - Status 1byte (T > O) (Instance ID 104, 105, 106 선택시)   
\.      - 753-436 : 1byte (T > O)   
\.      - 753-536 : 1byte (O > T)   

\.      [IO Assembly 정보]   
\.      [T > O]   
\.      - Size: 2bytes   
\.      - Instance: 105   
\.      - Run/Idle Header: No   

\.      [O > T]    
\.      - Size: 1bytes   
\.      - Instance: 101   
\.      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
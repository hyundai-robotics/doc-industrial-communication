#### 2.4.3.6 외부 Adapter 장치 연결 - Rockwell Automation (AB) Remote IO

<br>

{% hint style="info" %}
   - EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

   - “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 해당 장치의 IP 설정은 Rockwell Automation (AB) Point I/O 1734-AENTR 매뉴얼을 참조하여 진행해 주십시오.
{% endhint %}

<br>

**1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.**

<br>

![[그림 2.4.3.6-1 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_1.png>) 

<br>

![[그림 2.4.3.6-2 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_2.png>) 

<br>

**2. EZ-EDS 프로그램으로 EDS 파일을 열어 장치 정보를 확인합니다.**

<br>

![[그림 2.4.3.6-3 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_3.png>) 

<br>

![[그림 2.4.3.6-4 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_4.png>) 

<br>

{% hint style="info" %}
   - Connection Manager에서 연결 타입 확인   
      - 예시에서는 Exclusive Owner

   - Real Time Transfer Format에서 헤더 여부 확인   
      - Input (T > O) : 헤더 없음   
      - Output (O > T) : 32-bit run/idle header   

   - Create / Decode path 를 눌러 Instance ID 확인   
      - Input (T > O) : 101   
      - Output (O > T) : 100   
      - Configuration : 102   
{% endhint %}

<br>

**3. 장치 매뉴얼에서 IO size를 확인합니다.**

<br>

{% hint style="info" %}
   - 현재 연결할 장치의 IO 구성 확인 
{% endhint %}

<br>

![[그림 2.4.3.6-5 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_5.png>) 

<br>

{% hint style="info" %}
   - 슬롯 구성별 매뉴얼을 참고하여 IO size 확인
{% endhint %}

<br>

![[그림 2.4.3.6-6 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_6.png>) 

<br>

![[그림 2.4.3.6-7 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_7.png>) 

<br>

**4. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.**

<br>

![[그림 2.4.3.6-8 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_8.png>)

<br>

{% hint style="info" %}
   - 연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
      - Input (T > O) : Slave > Master 연결   
      - Output (O > T) : Master > Slave 연결   

   [Adapter 구성]   
   - Point I/O 1734-AENTR    
      - 상태 값 : 8byte (T > O)    
      - 1734-IB8 : 1byte (T > O)   
      - 1734-OB8E : 1byte (O > T) + 1byte (T > O, 상태 값)   

   [IO Assembly 정보]   
   [T > O]   
      - Size: 10bytes   
      - Instance: 101   
      - Run/Idle Header: No   

   [O > T]    
      - Size: 1byte   
      - Instance: 100   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>

![[그림 2.4.3.6-9 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_9.png>)

<br>

{% hint style="info" %}
   - 연결할 장치의 매뉴얼을 확인하여 부가 설정값을 올바르게 입력해 주십시오.   
      - Input (T > O) : Slave > Master 연결   
      - Output (O > T) : Master > Slave 연결   

   [부가 설정 값]   
      - Config Segment : ON   
      - Instance: 102   
      - Size: 10bytes    

   [Config Segment 정보]    
      - (4bytes) 1 : 헤더    
      - (2bytes) 3 : 연결된 슬롯 + 1   
      - (1byte)  0 : T > O Alignment (byte 단위)      
      - (1byte)  1 : T > O 슬롯별 데이터 크기      
      - (1byte)  0 : O > T Alignment (byte 단위)      
      - (1byte)  1 : O > T 슬롯별 데이터 크기      
{% endhint %}

<br>
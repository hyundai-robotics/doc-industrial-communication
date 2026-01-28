#### 2.4.3.5 외부 Adapter 장치 연결 - Beckhoff Remote IO

<br>

{% hint style="info" %}
   - EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

   - “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 해당 장치의 IP 설정은 Beckhoff 매뉴얼을 참조하여 진행해 주십시오.
{% endhint %}

<br>

**1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.**

![[그림 2.4.3.5-1 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_1.png>) 

<br>

**2. 장치 웹페이지에 접속하여 IP 주소를 설정합니다.**

<br>

{% hint style="info" %}
   - 예시에서 초기 IP 설정은 192.168.1.2 로 되어있습니다. (DIP 스위치 2번 ON)
{% endhint %}

<br>

![[그림 2.4.3.5-2 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_2.png>) 

<br>

![[그림 2.4.3.5-3 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_3.png>) 

<br>

{% hint style="info" %}
   - 예시에서는 IP를 192.168.10.95로 설정합니다. 

   - IP 주소 입력 후 체크 버튼을 눌러 저장합니다. 
{% endhint %}

<br>

![[그림 2.4.3.5-4 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_4.png>) 

<br>

{% hint style="info" %}
   - DIP 스위치를 아래와 같이 설정한 후 장치를 재부팅합니다.   
      - 1 ~ 8번  : ON   
      - 9 ~ 10번 : OFF   
{% endhint %}

<br>

![[그림 2.4.3.5-5 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_5.png>) 

<br>

![[그림 2.4.3.5-6 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_6.png>) 

<br>

**3. 장치 웹페이지에 접속하여 EtherNet/IP 설정 정보를 확인합니다.**

<br>

{% hint style="info" %}
   - 설정한 IP 주소로 다시 접속하여 IP 주소 및 EtherNet/IP 구성 정보를 확인합니다.
{% endhint %}

<br>

![[그림 2.4.3.5-7 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_7.png>) 

<br>

![[그림 2.4.3.5-8 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_8.png>) 

<br>

{% hint style="info" %}
   - Input (T > O)   
      - Instance ID: 129   
      - Byte Size: 6      

   - Output (O > T)   
      - Instance ID: 130   
      - Byte Size: 6   
{% endhint %}

<br>

**4. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.**

<br>

![[그림 2.4.3.5-9 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_9.png>)

<br>

{% hint style="info" %}
   - 연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
      - Input (T > O) : Slave > Master 연결   
      - Output (O > T) : Master > Slave 연결   

   [Adapter 구성]   
   - Beckhoff EK-9500   
      - EK-1008 : 1byte (T > O)   
      - EK-2008 : 1byte (O > T)   

   [IO Assembly 정보]   
   [T > O]   
      - Size: 6bytes   
      - Instance: 129   
      - Run/Idle Header: No   

   [O > T]    
      - Size: 6bytes   
      - Instance: 130   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
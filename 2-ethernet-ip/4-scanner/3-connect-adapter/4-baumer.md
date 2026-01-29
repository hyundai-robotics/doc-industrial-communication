#### 2.4.3.4 외부 Adapter 장치 연결 - Baumer OM-70

<br>

{% hint style="info" %}
   - EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

   - "[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 해당 장치의 IP 설정은 Baumer 매뉴얼을 참조하여 진행해 주십시오.
{% endhint %}

<br>

**1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.**

![[그림 2.4.3.4-1 Baumer OM-70]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_1.png>) 

<br>

**2. 장치 매뉴얼에서 Instance ID 및 IO Size를 확인합니다.**

<br>

![[그림 2.4.3.4-2 Baumer OM-70]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_2.png>) 

<br>

{% hint style="info" %}
   [Input Only Connection]   

   - Input (T > O)   
      - Instance ID: 100   
      - Size : 34 bytes   

   - Output (O > T)   
      - Instance ID: 238   
      - Size : 0 byte    
{% endhint %}

<br>

**3. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.**

<br>

![[그림 2.4.3.4-3 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_3.png>)

<br>
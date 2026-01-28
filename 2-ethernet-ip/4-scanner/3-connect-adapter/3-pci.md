#### 2.4.3.3 외부 Adapter 장치 연결 - Hilscher CIFX PCI EtherNet/IP Adapter

<br>

{% hint style="info" %}
   - EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

   - “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 해당 장치의 IP 설정은 Hilscher 매뉴얼을 참조하여 진행해 주십시오.
{% endhint %}

<br>

**1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.**

![[그림 2.4.3.3-1 CIFX PCI]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_1.png>) 

<br>

**2. EZ-EDS 프로그램으로 EDS 파일을 열어 장치 정보를 확인합니다.**

<br>

![[그림 2.4.3.3-2 EDS 파일 정보]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_2.png>) 

<br>

{% hint style="info" %}
   - Connection Manager에서 연결 타입 확인   
      - 예시에서는 Exclusive Owner

   - Real Time Transfer Format에서 헤더 여부 확인   
      - Input (T > O) : 32-bit run/idle header   
      - Output (O > T) : 32-bit run/idle header   
{% endhint %}

<br>

![[그림 2.4.3.3-3 EDS 파일 정보]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_3.png>) 

<br>

{% hint style="info" %}
   - Param에서 Instance ID 확인   
      - Input (T > O) : 101   
      - Output (O > T) : 100   
{% endhint %}

<br>

**3. 장치에 설정된 IO size를 확인합니다.**

<br>

{% hint style="info" %}
   - 현재 연결할 장치의 IO Size 확인 (해당 PCI 장치 설정 참조)   
{% endhint %}

<br>

**4. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.**

<br>

![[그림 2.4.3.3-4 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_4.png>)

<br>

{% hint style="info" %}
   - 연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
      - Input (T > O) : Slave > Master 연결   
      - Output (O > T) : Master > Slave 연결   

   [IO Assembly 정보]   
   [T > O]   
      - Size: 240 bytes (PCI 장치에 설정된 값)   
      - Instance: 101   
      - Run/Idle Header: 32Bit   

   [O > T]    
      - Size: 240 bytes (PCI 장치에 설정된 값)   
      - Instance: 100   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
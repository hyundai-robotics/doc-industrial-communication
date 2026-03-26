### 2.4.2 EtherNet/IP 스캐너 (마스터) 설정

<br>

"[**2.1 네트워크 설정**](../../2-ethernet-ip/1-network.md)" 및 "[**2.2 라이선스 설정**](../../2-ethernet-ip/2-license.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

**1. 메뉴를 터치하여 설정 화면으로 진입 합니다.**

<br>

**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 3: EtherNet/IP 설정]**

<br>

![[그림 2.4.2-1 스캐너 설정]](<../../_assets/2-ethernet-ip/4-scanner/img_1.png>) 

<br>

![[그림 2.4.2-2 스캐너 설정]](<../../_assets/2-ethernet-ip/4-scanner/img_2.png>) 

<br>

{% hint style="info" %}
   [Protocol 설정]

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

**2. Scanner 모드를 선택하고 "장치 추가(Add Device)" 버튼을 눌러 다음 화면으로 진입합니다.**

<br>

![[그림 2.4.2-3 스캐너 장치 추가]](<../../_assets/2-ethernet-ip/4-scanner/img_3.png>) 

<br>

**3. 연결할 장치와 동일하게 설정을 입력하고 저장합니다.**

<br>

{% hint style="info" %}
   [장치 설정]

      - Device No. : 장치 연결 순서 (IO 데이터 배치 순서)   
      - IP Address : 장치의 IP 주소   
      - Device Name : 장치 이름 (통신 연결과는 무관, 단순 식별용)   
      - RPI (ms) : IO 데이터 갱신 주기   
      - Connection Type   
            - Exclusive Owner (I/O) : Scanner - Adapter 입출력 연결   
            - Input Only : Adapter의 입력 신호만 연결   
            - Listen Only : Adapter 가 다른 Scanner와 I/O 연결 되어있는 상태에서 입력 신호만 연결   

      - Input (T > O) : Slave > Master 연결   
      - Output (O > T) : Master > Slave 연결   

      - Run/Idle Header : IO 데이터 헤더 유무 선택   
      - Instance No. : IO 데이터 교환을 위한 Input / Output Assembly의 Instance 번호   
      - IO Size : IO 데이터 크기 (bytes 단위)   
{% endhint %}

<br>

{% hint style="info" %}
   - 연결 예시는 아래 매뉴얼을 참고해주십시오.    
   - "[**2.3.3.1 외부 Adapter 장치 연결 - Crevis Remote IO**](3-connect-adapter/1-crevis.md)"

   - "[**2.3.3.2 외부 Adapter 장치 연결 - Wago Remote IO**](3-connect-adapter/2-wago.md)"

   - "[**2.3.3.3 외부 Adapter 장치 연결 - Hilscher CIFX PCI EtherNet/IP Adapter**](3-connect-adapter/3-pci.md)"

   - "[**2.3.3.4 외부 Adapter 장치 연결 - Baumer OM-70**](3-connect-adapter/4-baumer.md)"  
{% endhint %}

<br>

![[그림 2.4.2-4 스캐너 장치 추가]](<../../_assets/2-ethernet-ip/4-scanner/img_4.png>) 

<br>

**4. OK 버튼을 눌러 통신 설정을 전송합니다.**

<br>

![[그림 2.4.2-5 스캐너 설정]](<../../_assets/2-ethernet-ip/4-scanner/img_5.png>) 

<br>

**5. 통신이 정상적으로 연결되었는지 상태를 확인합니다.**

<br>

![[그림 2.4.2-6 통신 상태 모니터링]](<../../_assets/2-ethernet-ip/4-scanner/img_6.png>) 

<br>

{% hint style="info" %}
   [통신 상태 확인]   

      - 라이선스: 현재 라이선스 상태   
      - 실행: EtherNet/IP 기능 동작 상태 표시   
      - 통신: EtherNet/IP 통신 연결 상태 표시   
      - 에러: EtherNet/IP 오류 상태 표시   
{% endhint %}

<br>

{% hint style="info" %}
   [장치 번호 색상]   

      - 초록색 : 통신 연결 OK   
      - 빨간색 : 통신 연결 NG   
{% endhint %}

<br>

![[그림 2.4.2-7 통신 상태 모니터링]](<../../_assets/2-ethernet-ip/4-scanner/img_7.png>) 

<br>

**6. 통신 설정 완료 후 IO Block 을 할당합니다.**

{% hint style="info" %}
   **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  ("[**4. 산업용 통신 IO Block 할당**](../../5-io-block-allocation.md)")를 확인해 주십시오.**
{% endhint %}
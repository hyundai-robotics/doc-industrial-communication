#### 1.3.7.3 DeviceNet Master 설정 (TP)

"[1.3.1 CIFX PCI 슬롯 설정](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
   - DeviceNet Connector 연결은 아래를 참고해 주십시오.

      ("[1.2.2 커넥터](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. PCI 슬롯 설정에서 DeviceNet Master를 선택하고 로봇 제어기를 재부팅합니다.**

![[그림 1.3.7.3-1 PCI 슬롯 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_1.png>) 

<br>

**2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.**

<br>

{% hint style="info" %}
   - TP 에서 산업용 통신 상태를 확인하는 절차는 ("[1.4 CIFX PCI 통신 모니터링](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")참고해 주십시오.
{% endhint %}

<br>

![[그림 1.3.7.3-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

**3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다.**

**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬롯 통신 설정 >  DeviceNet Master]**

![[그림 1.3.7.3-3 마스터 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_3.png>) 

![[그림 1.3.7.3-4 마스터 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_4.png>) 

<br>

**4. 각 항목별 설명**

{% hint style="warning" %}
**\[TP 네트워크 스캔 제한 사항]**   
   - Poll Connection만 지원   
   - Quick Start 미지원   

{% endhint %}

<br>

{% hint style="info" %}
   [사용 여부]   
   - Off: DeviceNet Master 사용 안함   
   - On: DeviceNet Master 사용   

   [통신 속도]   
   - 125 kbit/s   
   - 250 kbit/s   
   - 500 kbit/s   

   [마스터 MAC ID]   
   - DeviceNet Master의 MAC ID = 0 으로 고정   

   [IO 업데이트 주기]   
   - 최소 전송 간격 (Production Inhibit Time): IO 업데이트의 최소 사이 간격 시간   
   - 예상 패킷 주기 (Expected Packet Rate): 패킷이 정상적으로 들어올 것으로 예상하는 시간 (Timeout 연관)   

{% endhint %}

<br>

**5. 통신 환경에 따라 설정 후 "네트워크 스캔" 버튼을 클릭합니다.**

<br>

{% hint style="warning" %}
   **Network Scan 시 아래 사항을 반드시 확인해 주십시오.**

   **(1) 케이블 연결 여부**  
   **(2) 종단저항 연결 또는 종단 DIP Switch 사용 여부**  
   **(3) Master - Slave 통신 속도 설정 여부**  

   **원활한 통신 연결을 위해 ("[1.3.7.6 DeviceNet ERROR 조치](../7-DeviceNet/6-Error-DeviceNet.md)")을 반드시 확인해 주십시오.**
{% endhint %}

<br>

![[그림 1.3.7.3-5 마스터 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_5.png>) 

<br>

**6. 장치들의 설정을 확인 후 "확인" 버튼을 눌러 통신을 적용 합니다.**

<br>

![[그림 1.3.7.3-6 마스터 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_6.png>) 

<br>

**7. 노드 설정 값 설명**

{% hint style="info" %}
   [노드 정보 설명]   
   - Node: 장치의 MAC ID   
   - Product Name: 장치 제품 명칭   
   - Vendor ID: 장치 제조사의 고유 번호   
   - Status: 장치의 상태 값   
   
   [IO 설정]   
   - Output Size (Produced Size): Master --> Slave 출력 크기 (byte 단위)   
   - Input Size (Consumed Size): Slave --> Master 입력 크기 (byte 단위)   
   
   [IO 업데이트 주기]   
   - PIT (Production Inhibit Time): IO 업데이트의 최소 사이 간격 시간   
   - EPR (Expected Packet Rate): 패킷이 정상적으로 들어올 것으로 예상하는 시간 (Timeout 연관)   

{% endhint %}

<br>

{% hint style="info" %}
   [예상 패킷 주기 (PIT: Production Inhibit Time)]   
   - 네트워크 스캔 후 연결된 장치들의 IO Size를 고려하여 예상 패킷 주기를 자동으로 계산합니다.   

   - 예시 1)   
      - 125 Kbit/s   
      - 전체 Input + Output: 100 byte   
      - 1Cycle 소요 시간: 100 x 8 (bit) / 125K = 6.4ms   
      - 통신 부하 33% 적용: 6.4 ms x 3 = 19.2ms --> 20ms PIT 적용   

   - 예시 2)   
      - 250 Kbit/s   
      - 전체 Input + Output: 500 byte   
      - 1Cycle 소요 시간: 500 x 8 (bit) / 250K = 16ms   
      - 통신 부하 33% 적용: 16 ms x 3 = 48ms PIT 적용   

   - PIT 값은 각 장치별로 변경이 가능합니다.   
   - 주기가 짧을 수록 장치에 걸리는 부하가 커질 수 있습니다. (각 장치별 사양 확인 필요)   

{% endhint %}

<br>

![[그림 1.3.7.3-7 마스터 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_7.png>) 

<br>

**8. 통신 상태 확인**

<br>

{% hint style="info" %}
   - TP 에서 산업용 통신 상태를 확인하는 절차는 ("[1.4 CIFX PCI 통신 모니터링](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")참고해 주십시오.   
{% endhint %}

<br>

![[그림 1.3.7.3-8 통신 상태 확인]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_8.png>) 

<br>

![[그림 1.3.7.3-9 통신 상태 확인]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Master_setting-tp/image_9.png>) 

<br>

**9. 통신 설정 완료 후 IO Block 을 할당합니다.**

{% hint style="info" %}
   **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  ("[5. 산업용 통신 IO 읽기 및 쓰기](../../../5-io-block-allocation.md)")를 확인해 주십시오.**
{% endhint %}
#### 1.3.9.2 CC-Link IE Field Slave 설정

"[1.3.1 CIFX PCI 슬롯 설정](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.


<br>

**1. TP를 이용하여 산업용 통신 펌웨어 설정에서 CC-Link IE Field Slave를 선택하고 로봇 제어기를 재부팅합니다.**

![[그림 1.3.9.2-1 펌웨어 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_1.png>) 

<br>

**2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.**

![[그림 1.3.9.4-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

**3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다.**

**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬레이브 슬롯 설정 >  CC-Link IE Field Slave]**

![[그림 1.3.9.4-3 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>) 

![[그림 1.3.9.4-4 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>) 

<br>

**4. 각 항목별 설명**

{% hint style="info" %}
   [Network Number]

   - CC-Link IE Field network 번호 (1~239)
{% endhint %}

{% hint style="info" %}
   [Station Address]

   - 연결된 network 내에 장치 ID (1 ~ 120)
{% endhint %}

{% hint style="info" %}
   [IO Type]

   - IO Type은 master 장치 설정에 의해 결정됨   
      - Mixed: 입력과 출력이 다른 인덱스 사용 (서로 다른 주소)   
      - Input: 입력 전용   
      - Output: 출력 전용   
      - FrontBackMixture: 입력과 출력이 같은 인덱스 사용 (동일한 주소)   
{% endhint %}

{% hint style="info" %}
   [Device Type]

   - Device Type에 따라 설정 가능한 IO 최대 크기가 상이합니다.

   - Intelligent Device Station   
      - RY, RX (max): 256 bytes   
      - RWw, RWr (max): 1024 words

   - Remote Device Station   
      - RY, RX (max): 16 bytes   
      - RWw, RWr (max): 64 words
{% endhint %}

{% hint style="info" %}
   [IO Size]

   - Master -> Slave   
      - RWw (word data)   
      - RY (bit data)   

   - Slave -> Master   
      - RWr (word data)   
      - RX (bit data)  
{% endhint %}

<br>

**5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.**

TP 에서 산업용 통신 상태를 확인하는 절차는 ("[1.4 CIFX PCI 통신 모니터링](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")참고해 주십시오.

<br>

**6. 통신 설정 완료 후 IO Block 을 할당합니다.**

{% hint style="info" %}
   **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  ("[5. 산업용 통신 IO 읽기 및 쓰기](../../../5-io-block-allocation.md)")를 확인해 주십시오.**
{% endhint %}

<br>

![[그림 1.3.9.4-5 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>) 
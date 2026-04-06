#### 1.3.6.4 PROFIBUS-DP Slave 설정

"[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
   **[PROFIBUS-DP Slave GSD File 다운로드]**

   - "[**5. Slave 장치 설명 파일**](../../../5-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

<br>

**1. TP를 이용하여 산업용 통신 펌웨어 설정에서 PROFIBUS-DP Slave를 선택하고 로봇 제어기를 재부팅합니다.**

![[그림 1.3.6.4-1 펌웨어 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

**2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.**

![[그림 1.3.6.4-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

**3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다.**

**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬레이브 슬롯 설정 >  PROFIBUS-DP Slave]**

![[그림 1.3.6.4-3 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[그림 1.3.6.4-4 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

<br>

**4. 각 항목 별 설명**

{% hint style="info" %}
   [Station Address]

   - PROFIBUS-DP는 Station Address를 통해 Slave를 식별합니다.
{% endhint %}

{% hint style="info" %}
   [입력 바이트 수 (Input Byte)]

   - 입력 바이트 수 : Master -> Slave 로 입력되는 데이터 크기를 설정합니다.
{% endhint %}

{% hint style="info" %}
   [출력 바이트 수 (Output Byte)]

   - 출력 바이트 수 : Slave -> Master 로 출력하는 데이터 크기를 설정합니다.
{% endhint %}

{% hint style="info" %}
   [**Master 에서 Module 설정 시**]

   - 설정한 바이트 수와 일치하도록 Master에서 Module을 지정해 주어야합니다.

   - 순서 : Master Input (64 ~ 1) -> Master Output (64 ~ 1)

   - EX) Master Input 109 bytes  <---  Slave Output 109 bytes   
         - Input 109 Bytes : 64Byte + 32Byte + 8Byte + 4Byte + 1 Byte

   - EX) Master Output 120 bytes  --->  Slave Input 120 bytes   
         - Output 120 Bytes : 64Byte + 32Byte + 16Byte + 8Byte


   - EX) Master Input 12 bytes  <---  Slave Output 12 bytes   
         - Input 12 Bytes : 8Byte + 4Byte

   - EX) Master Output 200 bytes  --->  Slave Input 200 bytes   
         - Output 200 Bytes : 64Byte + 64Byte + 64Byte + 8Byte

   - 입력 Module이 출력 Module 보다 앞에 위치합니다.
{% endhint %}

![[그림 1.3.6.4-5 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>) 


<br>

**5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.**

TP 에서 산업용 통신 상태를 확인하는 절차는 ("[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)")참고해 주십시오.

![[그림 1.3.6.4-6 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>) 

<br>

**6. 통신 설정 완료 후 IO Block 을 할당합니다.**

{% hint style="info" %}
   **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  ("[**5. 산업용 통신 IO Block 할당**](../../../5-io-block-allocation.md)")를 확인해 주십시오.**
{% endhint %}
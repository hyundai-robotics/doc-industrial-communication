#### 1.3.5.4 EtherCAT Slave 설정

<br>

{% hint style="info" %}
   **[EtherCAT Slave ESI File 다운로드]**

   - "[6. Slave 장치 설명 파일](../../../6-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

<br>

"[1.3.1 CIFX PCI 슬롯 설정](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

**1. TP를 이용하여 산업용 통신 PCI 슬롯 설정에서 EtherCAT Slave를 선택하고 로봇 제어기를 재부팅합니다.**

![[그림 1.3.9.2-1 PCI 슬롯 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Slave_setting/image_1.png>) 

<br>

**2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.**

![[그림 1.3.9.4-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

**3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다.**

**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬롯 통신 설정 >  EtherCAT Slave]**

![[그림 1.3.9.4-3 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Slave_setting/image_3.png>) 

![[그림 1.3.9.4-4 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Slave_setting/image_4.png>) 

<br>

**4. 각 항목별 설명**

{% hint style="info" %}
   [IO 종류 및 크기]   
   - TxPDO: 슬레이브 -> 마스터   
   - RxPDO: 마스터 -> 슬레이브   
   - 최대 크기: 256 bytes   
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

![[그림 1.3.9.4-5 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Slave_setting/image_5.png>) 
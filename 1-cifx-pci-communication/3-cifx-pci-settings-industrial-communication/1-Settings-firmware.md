## 1.3.1 CIFX PCI 슬롯 설정.

CIFX PCI 슬롯의 통신 방식을 설정합니다. 설정 적용을 위해서는 제어기 전원을 차단한 후 다시 공급해주시기 바랍니다.

<br>

“[**1.2.1 PCI 산업용 통신 카드**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" 참고하여 아래 방법을 진행해 주십시오.

<br>

**1. 메뉴를 터치하여 슬롯 설정 화면으로 진입 합니다.**
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 1: PCI 슬롯 설정 > 1 채널]** 


<br>

**2. 아래 화면을 참고하여 슬롯과 통신 방식(Master/Slave), 프로토콜을 선택 합니다.**
   * 슬롯 번호는 PCI 통신 카드의 Rotary Swtich 번호 입니다.
   * 통신 설정 변경을 원하지 않을 경우 **\[OK]** 버튼을 터치하여 종료합니다.

{% hint style="warning" %}
**\[주의]**: **\[초기화]** 또는 **\[적용]** 버튼을 터치하면 현재 탭의 슬롯 정보가 초기화 됩니다. Config 파일도 같이 초기화 되니 유의하시기 바랍니다.
{% endhint %}

![[그림 1.3.1-1 PCI 슬롯 설정]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[그림 1.3.1-2 PCI 슬롯 설정(master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[그림 1.3.1-3 PCI 슬롯 설정(Slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

**3. 슬롯 설정을 완료 합니다.**
**\[적용]** 메뉴를 터치

![[그림 1.3.1-4 PCI 슬롯 설정]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[주의]**

<1>. **\[적용]** 버튼을 터치하여 설정 시 해당 슬롯에 적용 되어있는 CONFIG 파일이 모두 삭제된 후 변경됩니다. 통신을 변경 하실 경우 기존 설정을 별도로 보관하는 것을 권장합니다.

<2>. **\[적용]** 버튼을 터치하지 않고 **\[OK]**버튼을 터치할 경우 선택한 통신이 적용되지 않습니다.
{% endhint %}

<br>

**4. 각 슬롯마다 2. \~ 3.번을 반복하여 설정해 줍니다.**

<br>

**5. 제어기를 재부팅하여 설정한 통신을 적용합니다.**
**\[서비스 > 19: 산업용 통신 모니터링]** 메뉴를 터치하여 설정한 통신이 적용 되었는지 확인합니다.

![[그림 1.3.1-5 산업용 통신 설정 화면]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[주의]**: 슬롯 설정 후 제어기를 재부팅 할 때 설정값이 적용됩니다.
{% endhint %}

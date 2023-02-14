# 3.3 산업용 통신 DIO Block 할당 설정

“[**3.1 산업용 통신 펌웨어 설정**](../3-1-firmware.md)” 및 “[**3.2 산업용 통신 추가 설정(Master 및 Slave)**](../3-2-addition-industrial-communication-master-slave/)” 작업 완료 후 제어기와의 통신을 위한 DIO Block 할당 방법 입니다.

제어기의 범용 입출력 신호를 사용하는 방법을 설정합니다. 사용 안함(None), PLC, Fieldbus에 연결하여 사용할 수 있습니다.

1. **\[2: 제어 파라미터 > 2: 입출력 신호 설정 > 6: DIO 블록 할당]** 메뉴를 터치하십시오.
2. 선택된 FB 주소의 DIO 블록을 연결 설정한 후 **\[OK]** 버튼을 터치하십시오.
   * Fieldbus로 설정시 보드 번호는 PCI 통신카드의 Rotary Switch 번호 입니다.

![](<../../_assets/image_11.png>)

* **\[None]**: 선택된 FB 주소의 DIO 블록을 할당하지 않습니다. 제어기의 초기 설정값으로 아무것도 선택하지 않을 경우 None으로 설정됩니다.
* **\[PLC]**: 선택된 FB 주소의 DIO 블록을 PLC로 연결하여 사용합니다. PLC 동작은 MULTIPROG 프로그램을 이용합니다.
* **\[Fieldbus]**: 선택된 FB 주소의 DIO 블록을 PCI 통신 카드(Fieldbus)로 연결하여 사용합니다. DIO 블록을 PCI 통신 카드로 연결할 경우 PCI 보드 선택창이 활성화됩니다.

{% hint style="warning" %}
**\[주의]**: 같은 통신 카드를 PLC/Fieldbus에서 동시 사용이 불가능합니다. 둘 중 한 가지로만 데이터를 연결하여 사용해야 합니다.
{% endhint %}

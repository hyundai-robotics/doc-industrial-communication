# 6. 산업용 통신 DIO Block 할당 설정

산업용 통신 설정 완료 후 제어기와의 통신을 위한 DIO Block 할당 방법 입니다.

산업용 통신 IO를 사용하기 위해 fb0 \~ fb9 영역에 할당해야 합니다.

<br>

##### 1. DIO 블록 할당 메뉴를 선택
   **\[시스템 > 2: 제어 파라미터 > 2: 입출력 신호 설정 > 6: DIO 블록 할당]** 메뉴를 터치하십시오.

<br>

##### 2. 원하는 fb 영역에 산업용 통신 Slot 번호 지정
   지정 후 **\[OK]** 버튼을 터치하십시오.

![[그림 6-1]](<_assets/6-DIO-Allocation/newFB.png>)


{% hint style="warning" %}
**\[주의]**: 내장 PLC와 함께 사용하는 경우 IO 속성, DI/DO - X/Y 를 확인해 주십시오. 
{% endhint %}

{% hint style="warning" %}
**\[주의]**: EtherNet/IP 어댑터의 경우 최대 블록사이즈는 120 Bytes 이며 최대 2개까지 선택할 수 있습니다. 2개를 초과하는 선택은 무시 됩니다.
{% endhint %}

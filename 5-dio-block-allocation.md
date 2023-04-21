﻿# 5. 산업용 통신 DIO Block 할당 설정

산업용 통신 설정 완료 후 제어기와의 통신을 위한 DIO Block 할당 방법 입니다.

산업용 통신 IO를 사용하기 위해 fb0 \~ fb9 영역에 할당해야 합니다.

1. **\[시스템 > 2: 제어 파라미터 > 2: 입출력 신호 설정 > 6: DIO 블록 할당]** 메뉴를 터치하십시오.

2. 원하는 fb 영역에 산업용 통신 Slot 번호를 지정합니다.
   지정 후 **\[OK]** 버튼을 터치하십시오.

![그림 5-1](<_assets/5-DIO-Allocation/image_1.png>)


{% hint style="warning" %}
**\[주의]**: 내장 PLC와 함께 사용하는 경우 IO 속성, DI/DO - X/Y 를 확인해 주십시오. 
{% endhint %}
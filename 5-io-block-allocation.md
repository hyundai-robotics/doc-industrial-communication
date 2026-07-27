# 5. 산업용 통신 IO 읽기 및 쓰기

산업용 통신 설정 완료 후 제어기와의 통신을 위한 IO Block 할당 방법 입니다.

산업용 통신 IO를 사용하기 위해 fb0 \~ fb9 영역에 할당해야 합니다.

<br>

{% hint style="info" %}
   - fb 블록의 IO 읽기/쓰기 방법은 아래 매뉴얼을 참조해 주십시오.

      **\[제어기 조작설명서 : 범용 입력]**   
      **\[제어기 조작설명서 : 범용 출력]**   
{% endhint %}

<br>

**1. IO 블록 할당 메뉴를 선택**
   **\[시스템 > 2: 제어 파라미터 > 2: 입출력 신호 설정 > 6: FB 블록 할당]** 메뉴를 터치하십시오.

<br>

**2. 원하는 fb 영역에 산업용 통신 종류 지정**
   지정 후 **\[OK]** 버튼을 터치하십시오.

![[그림 5-1]](<_assets/5-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[주의]**: 내장 PLC와 함께 사용하는 경우 IO 속성, DI/DO - X/Y 를 확인해 주십시오. 
{% endhint %}

{% hint style="info" %}

   **[fb block 할당 방법]**

   - fb 블록 1개의 크기는 120byte (960점) 입니다.   
   - fb 블록 할당 예시   
      - PCI 슬롯 1: CC-Link Slave   
      - 설정: Version 2 / 3국 점유 / 확장 싸이클릭 8배   
      - I/O 크기   
         - RX/Y: 80 byte   
         - RWr/w: 192 byte   
         - 총: 272 byte   

      - fb 블록 번호가 낮은 순서대로 IO 맵핑   
         - fb2: PCI 슬롯 1 ( ~ 120 byte)   
         - fb4: PCI 슬롯 1 ( ~ 240 byte)   
         - fb5: PCI 슬롯 1 ( ~ 272 byte)   

{% endhint %}

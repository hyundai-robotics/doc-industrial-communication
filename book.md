# Hi6 로봇제어기 기능설명서 - 산업용 통신

{% hint style="warning" %}
본 제품 설명서에서 제공되는 정보는 현대로보틱스의 자산입니다.

현대로보틱스의 서면에 의한 동의 없이 전부 또는 일부를 무단 전재 및 재배포할 수 없으며, 제3자에게 제공되거나 다른 목적에 사용할 수 없습니다.



본 설명서는 사전 예고 없이 변경될 수 있습니다.



**Copyright ⓒ 2020 by Hyundai Robotics**
{% endhint %}
# 1. 프로그램 설치

산업용 통신 관련 프로그램 설치 방법입니다.
# 1.1 Sycon.net

PCI 통신 카드에 사용하는 통신 Configuration을 만들어주는 프로그램 입니다.

**1.**    현대 로보틱스 홈페이지([www.hyundai-robotics.com](http://www.hyundai-robotics.com)) -> 고객지원 -> 응용소프트웨어 에서 “**Sycon.net**”을 다운로드 합니다.

**2.**    압축 해제 -> 내부 폴더에서 “**Communication-Solutions.exe**”를 실행 -> “**Install SYCON.net Configuration Software**” 선택 하여 프로그램을 설치 합니다.

![그림 1 Sycon.net 설치 화면](<../_assets/image_5.png>)
# 1.2 Multiprog

PCI 통신 카드 연결 이후 DIO 데이터 교환을 위해서 사용하는 PLC 프로그램 입니다. (‘3.3 산업용 통신 DIO Block 할당 설정’에서 “**PLC**”로 세팅 후 사용하시기 바랍니다.)

**1.**    현대로보틱스 홈페이지([www.hyundai-robotics.com](http://www.hyundai-robotics.com)) -> 고객지원 -> 응용 소프트웨어 에서 “**Hi6 Multiprog**”을 다운로드 합니다.

**2.**    다음 내용을 따라 설치를 진행 하시면 됩니다.

{% hint style="info" %}
1. MP5.51 Express.zip 압축풀기
2. MULTIPROG 5.51.msi 실행
   * 설치 시 에러가 발생될 경우 setup.exe로 설치
3. MP eCLR Addon.zip 압축풀기
4. I486\_LE\_GCC3\_eCLR.exe 실행
5. MULTIPROG 5.51 Build 653.zip 압축풀기
6. MULTIPROG 5.51 Build 653 폴더 내 "multiprog\_set\_batch\_express.bat" 파일 실행(관리자 권한으로 실행)

![](<../_assets/image_10.png>)


*   프로젝트 빌드에 문제 있을 경우 다음과 같이 추가 작업 : MULTIPROG 5.51 Build 653내의 파일들이 제대로 복사가 안되었을 수 있습니다.

    \-> MULTIPROG 5.51 Build 653 폴더의 모든 파일을 MULTIPROG 설치 경로의 같은 폴더안에 복사 : MULTIPROG 5.51 Build 653내의 파일을 아래의 'Default 설치'위치를 찾아가서 붙여넣기

    * Default 설치 : C:\Program Files (x86)\PHOENIX CONTACT Software\MULTIPROG 5.51 Express Build 653 폴더에 복사(덮어쓰기 3개 파일)


\*\*확인 방법\*\*

\-> Default 설치(혹은 설치위치) 위치의 다음 파일들 확인


{% endhint %}

![](../_assets/image.png)

(만약 Pro 버전사용을 원하신다면 “**Hi6 MultiProg 개발환경 설치 안내.pdf**”를 이용하여 설치 하시기 바랍니다. 단, License가 필요하니 현대로보틱스 본사에 요청하여 따로 구매 하시기 바랍니다. License가 없을 경우 Pro 버전은 30일만 사용가능하니 참고 바랍니다.)
# 2. 산업용 통신 카드 장착 및 설정

산업용 통신을 사용하기 위해서는 PCI 통신 카드(hilscher 사)가 필요합니다. 필요한 통신에 맞추어서 통신 카드를 연결 방법은 다음과 같습니다.

1. 구입한 PCI 통신 카드를 제어기 내부 Hi6Com(협동로봇 : Hi6Com Mini)에 장착하십시오.
2. PCI 통신 카드의 Rotary Switch를 돌려서 1 \~ 4번 내에서 설정해주십시오.(여러 개의 PCI 통신 카드 사용시 번호를 모두 다르게 설정하십시오.)

![그림 2 LCD 로봇 시스템의 기본 구성](<_assets/image_14.png>)

{% hint style="warning" %}
**\[주의]**: Rotary Switch번호는 PCI 카드마다 다르게 설정하시기 바랍니다.
{% endhint %}
# 3. 산업용 통신 설정

산업용 통신을 사용하기 위해서는 PCI 통신 카드 장착 후 티치 팬던트 및 Sycon.net프로그램을 이용하여 설정 해주어야 합니다.
# 3.1 산업용 통신 펌웨어 설정

사용하기 위한 산업용 통신 펌웨어를 설정하는 방법은 다음과 같습니다. 설정이 완료 후 펌웨어를 적용하기 위해서는 제어기 전원을 껏다가 켜주시기 바랍니다.

1. **\[설정 > 2: 제어 파라미터 > 11: 산업용 통신 > 1: 펌웨어 설정 > 1 채널]** 메뉴를 터치하여 펌웨어 설정 화면으로 진입 합니다.
2. 아래 화면을 참고하여 먼저 설정하신 슬롯을 선택, 그 다음으로 통신 방식(Master/Slave)을 설정, 마지막으로 원하는 프로토콜을 선택 합니다.
   * 슬롯 번호는 PCI 통신 카드의 Rotary Swtich 번호 입니다.
   * 통신 펌웨어 설정을 원하지 않을 경우 **\[초기화]** 버튼 터치하면 현재 보고있는 탭의 펌웨어 정보가 초기화 됩니다. Config 파일도 같이 초기화 되니 유의하시기 바랍니다.

![그림 3 축 산업용 통신 설정 화면(master)](<../_assets/image_7.png>) ![그림 3 축 산업용 통신 설정 화면(Slave)](<../_assets/image_3.png>)

3\. **\[적용]** 메뉴를 터치하여 펌웨어 설정을 완료 합니다.

{% hint style="warning" %}
**\[주의]**

1. **\[적용]** 버튼을 터치하여 펌웨어 설정 완료 시 해당 슬롯에 세팅 되어있는 CONFIG 파일이 모두 삭제 됩니다. 사용도중 통신 펌웨어를 변경 하실 경우 기존 CONFIG 세팅을 따로 BACKUP 해 주시기 바랍니다.
2. **\[적용]** 버튼을 터치하지 않고 **\[OK]**버튼을 터치할 경우 세팅한 펌웨어가 적용되지 않습니다.
{% endhint %}

4\. 각 슬롯마다 2. \~ 3.번을 반복하여 펌웨어를 설정해 줍니다.

5\. 제어기 전원을 껏다 켜주시면 설정하신 펌웨어가 적용 됩니다.

{% hint style="warning" %}
**\[주의]**: 펌웨어의 사용 설정 시 제어기의 전원을 끈 후 다시 켜야만 설정값이 시스템에 적용됩니다.
{% endhint %}
# 3.2 산업용 통신 추가 설정(Master 및 Slave)

산업용 통신 펌웨어 설정 후 통신을 사용하기 위한 세팅은 현대로보틱스 사이트에서 “**Sycon.net**” 프로그램을 이용하여서 설정해주시기 바랍니다.
# 3.2.1 Sycon.net 사용 방법

Hi6 제어기의 산업용 통신을 사용할 경우 “**Sycon.net**” 프로그램을 이용하여 통신 설정을 해주어야 합니다. 설정 방법은 다음과 같습니다. (“[**1.1 Sycon.net**](../../1-install-program/1-1-sycon-net.md)”을 참고하여 설치해주시기 바랍니다.)

1. Hi6Com(협동로봇 : Hi6MiniCom)의 LAN3포트를 PC와 연결 합니다.
2. 통신 설정 방법은 “Sycon.net v1.0500\DVD\_2018-12-1\_1\_0500\Documentation\4. Training Material\EN” 안에 파일들을 참고 하시면 됩니다.
   *   참고파일 이름

       1\) EtherNetIP Scanner - Configuration and Testing TM 02 EN.pdf

       2\) PROFIBUS DP Master - Configuration and Testing TM 02 EN.pdf

       3\) PROFINET IO Controller - Configuration and Testing TM 02 EN.pdf

{% hint style="info" %}
1\.      Hi6 Driver를 연결하기 netX Driver 설정 방법 예시 입니다.

2\.      IP Address는 제어기 설정에 맞추어 설정 하시면 됩니다.

3\.      EtherCAT Master 설정 방법 (CIFX 카드 연결)
{% endhint %}

![](<../../_assets/image_6.png>)

{% hint style="info" %}
4\.      연결한CIFX 카드(그림) “Double Click”

5\.      Driver -> Netx Driver 설정
{% endhint %}

![](<../../_assets/image_13.png>)

{% hint style="info" %}
6\.      netX Driver -> TCP Connection 다음과 같이 세팅 (IP Address는 제어기에 따라 변할 수&#x20;

&#x20;        있으니 확인 바랍니다.)
{% endhint %}

![](<../../_assets/image_19.png>)

{% hint style="info" %}
7\.      Device Assignment -> Scan클릭(아무것도 나오지 않을 경우: Device selection을 suitale&#x20;

&#x20;        only -> all로 변경 후 다시 Scan 클릭)

8\.      설정한 통신(Channel Protocol 확인)을 선택 후 “Apply” 이후 “OK”
{% endhint %}

![](<../../_assets/image_2.png>)

{% hint style="warning" %}
**\[주의]**: Access path위치가 cifX(num)\_Ch0 으로 되어 있지 않을 경우 하단의 Access path에서 변경하여 Apply)
{% endhint %}

{% hint style="info" %}
9\.      필요한 부분들을 세팅 하고 “CIFX 그림 우클릭” -> DOWNLOAD
{% endhint %}
# 3.3 산업용 통신 DIO Block 할당 설정

“[**3.1 산업용 통신 펌웨어 설정**](../3-1-firmware.md)” 및 “[**3.2 산업용 통신 추가 설정(Master 및 Slave)**](../3-2-addition-industrial-communication-master-slave/)” 작업 완료 후 제어기와의 통신을 위한 DIO Block 할당 방법 입니다.

제어기의 범용 입출력 신호를 사용하는 방법을 설정합니다. 사용 안함(None), PLC, Fieldbus에 연결하여 사용할 수 있습니다.

1. **\[2: 제어 파라미터 > 2: 입출력 신호 설정 > 6: DIO 블록 할당]** 메뉴를 터치하십시오.
2. 선택된 FB 주소의 DIO 블록을 연결 설정한 후 **\[OK]** 버튼을 터치하십시오.
   * Fieldbus로 설정시 보드 번호는 PCI 통신카드의 Rotary Switch 번호 입니다.
   * PLC로 사용시 “[**3.3.1 Multiprog 사용 방법**](1-using-multiprog.md)”을 참고하시기 바랍니다.

![](<../../_assets/image_11.png>)

* **\[None]**: 선택된 FB 주소의 DIO 블록을 할당하지 않습니다. 제어기의 초기 설정값으로 아무것도 선택하지 않을 경우 None으로 설정됩니다.
* **\[PLC]**: 선택된 FB 주소의 DIO 블록을 PLC로 연결하여 사용합니다. PLC 동작은 MULTIPROG 프로그램을 이용합니다.
* **\[Fieldbus]**: 선택된 FB 주소의 DIO 블록을 PCI 통신 카드(Fieldbus)로 연결하여 사용합니다. DIO 블록을 PCI 통신 카드로 연결할 경우 PCI 보드 선택창이 활성화됩니다.

{% hint style="warning" %}
**\[주의]**: 같은 통신 카드를 PLC/Fieldbus에서 동시 사용이 불가능합니다. 둘 중 한 가지로만 데이터를 연결하여 사용해야 합니다.
{% endhint %}
# 3.3.1 Multiprog 사용 방법

산업용 통신 설정 이후 Hi6 제어기의 DIO Block 할당을 PLC로 설정하였다면, ProconOS를 이용하여 DIO데이터를 교환하기 위해 다음과 같이 설정이 필요 합니다. (“[**1.2 Multiprog**](../../1-install-program/1-2-multiprog.md)”장을 참고하여 설치하여 주시기 바랍니다.)

1. 설치 후 사용 방법은 Mutiprog 내에 설명서를 참고 바랍니다. –

{% hint style="info" %}
1\.      Hi6 Multiprog 간단한 설정 방법 예시 입니다.

2\.      IP Address는 제어기 설정에 맞추어 설정 하시면 됩니다.

3\.      프로젝트 생성(Multiprog 실행 -> “File” -> “New Project” -> Project Wizard 클릭 및 OK)
{% endhint %}

![](<../../_assets/image_20.png>)

{% hint style="info" %}
4\.      순서에 따라 Project 생성

(1)    프로젝트 생성
{% endhint %}

![](<../../_assets/image_15.png>)

{% hint style="info" %}
(2) POU 및 프로그램이 언어 설정
{% endhint %}

![](<../../_assets/image_18.png>)

{% hint style="info" %}
(3) Resource 및 Type설정 (Type에 “Hi6”가 없으면 설치가 잘못된 것 이므로 설치가 잘되었는지 확인)
{% endhint %}

![](<../../_assets/image_1.png>)

{% hint style="info" %}
(4) Task 생성
{% endhint %}

![](<../../_assets/image_8.png>)

{% hint style="info" %}
5\.      프로젝트 속성 설정

(1)    하드웨어 속성 설정 : IO\_Confiuration 더블 클릭 -> Input/Output 속성 설정
{% endhint %}

![](<../../_assets/image_16.png>)

{% hint style="info" %}
* HI6 DIO input <-> Multiprog output / HI6 DIO output <-> Multiprog input으로 연결 되어 있습니다.
* CIFX input <-> Multiprog input / HI6 DIO output <-> Multiprog output으로 연결 되어 있습니다.

&#x20;

(2)    IO 세팅 방법 : 이름 설정 -> Task 설정 -> Board /IO module 선택 -> Driver Parameter 선택하여 설정(Offset 0 : Hi6 제어기 FB0.0, 단위 : Byte)
{% endhint %}

![](<../../_assets/image_9.png>)

{% hint style="info" %}
(3) IP 주소 설정 : Resource : Hi6(만든 이름따라 다름) 우 클릭 -> Settings -> Parameter의 IP Hi6와 맞춤
{% endhint %}

![](<../../_assets/image_4.png>)

{% hint style="info" %}
6\.      PLC 프로그램 작성 (사용자 필요에 따라서 프로그래밍)

7\.      프로그램 다운로드 : Online -> Project Control… -> Download 클릭
{% endhint %}

![](<../../_assets/image_17.png>)
# 4. 산업용 통신 모니터링

“[**2. 산업용 통신 카드 장착 및 설정**](2-mounting-setting-industrial-communication-card.md)” 및 “[**3. 산업용 통신 설정**](3-setting-industrial-communication/)” 절차를 따라 통신 설정 이후 동작여부를 다음과 같은 화면에서 확인 가능합니다.

**\[메뉴 > 19: 산업용 통신 모니터링]** 을 터치하여 들어갈 수 있으며, 해당 화면에서 설정한 펌웨어 정보, 통신 상태, 통신 구성 상태 등을 확인 가능합니다.

![](<_assets/image_12.png>)

{% hint style="info" %}
**\[재시작]** 버튼을 이용하여 해당 PCI 통신 카드의 산업용 통신을 재시작 시킬 수 있습니다.
{% endhint %}

# 3.3.1 Multiprog 사용 방법

산업용 통신 설정 이후 Hi6 제어기의 DIO Block 할당을 PLC로 설정하였다면, ProconOS를 이용하여 DIO데이터를 교환하기 위해 다음과 같이 설정이 필요 합니다. (“[**1.2 Multiprog**](../../1-install-program/1-2-multiprog.md)”장을 참고하여 설치하여 주시기 바랍니다.)

1. 설치 후 사용 방법은 Mutiprog 내에 설명서를 참고 바랍니다. –

{% hint style="info" %}
1\.      Hi6 Multiprog 간단한 설정 방법 예시 입니다.

2\.      IP Address는 제어기 설정에 맞추어 설정 하시면 됩니다.

3\.      프로젝트 생성(Multiprog 실행 -> “File” -> “New Project” -> Project Wizard 클릭 및 OK)
{% endhint %}

![](<../../_assets/image (20).png>)

{% hint style="info" %}
4\.      순서에 따라 Project 생성

(1)    프로젝트 생성
{% endhint %}

![](<../../_assets/image (15).png>)

{% hint style="info" %}
(2) POU 및 프로그램이 언어 설정
{% endhint %}

![](<../../_assets/image (18).png>)

{% hint style="info" %}
(3) Resource 및 Type설정 (Type에 “Hi6”가 없으면 설치가 잘못된 것 이므로 설치가 잘되었는지 확인)
{% endhint %}

![](<../../_assets/image (1).png>)

{% hint style="info" %}
(4) Task 생성
{% endhint %}

![](<../../_assets/image (8).png>)

{% hint style="info" %}
5\.      프로젝트 속성 설정

(1)    하드웨어 속성 설정 : IO\_Confiuration 더블 클릭 -> Input/Output 속성 설정
{% endhint %}

![](<../../_assets/image (16).png>)

{% hint style="info" %}
* HI6 DIO input <-> Multiprog output / HI6 DIO output <-> Multiprog input으로 연결 되어 있습니다.
* CIFX input <-> Multiprog input / HI6 DIO output <-> Multiprog output으로 연결 되어 있습니다.

&#x20;

(2)    IO 세팅 방법 : 이름 설정 -> Task 설정 -> Board /IO module 선택 -> Driver Parameter 선택하여 설정(Offset 0 : Hi6 제어기 FB0.0, 단위 : Byte)
{% endhint %}

![](<../../_assets/image (9).png>)

{% hint style="info" %}
(3) IP 주소 설정 : Resource : Hi6(만든 이름따라 다름) 우 클릭 -> Settings -> Parameter의 IP Hi6와 맞춤
{% endhint %}

![](<../../_assets/image (4).png>)

{% hint style="info" %}
6\.      PLC 프로그램 작성 (사용자 필요에 따라서 프로그래밍)

7\.      프로그램 다운로드 : Online -> Project Control… -> Download 클릭
{% endhint %}

![](<../../_assets/image (17).png>)

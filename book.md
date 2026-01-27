
[__SOURCE](README.md)
# Hi7 제어기 기능설명서 - 산업용 통신

[__SOURCE](1-cifx-pci-communication/README.md)
# 1. CIFX PCI 통신

CIFX PCI를 이용한 산업용 통신 매뉴얼입니다. 

[__SOURCE](1-cifx-pci-communication/1-cifx-pci-install-program/README.md)
# 1.1 CIFX PCI 프로그램 설치

산업용 통신 관련 프로그램 설치 방법입니다.

[__SOURCE](1-cifx-pci-communication/1-cifx-pci-install-program/1-sycon-net.md)
# 1.1.1 SYCON.net 설치

"Sycon.net" 은 Hilscher 에서 제공하는 PCI 통신 카드의 Configuration을 구성하는 프로그램 입니다.

<br>

##### 1. SYCON.net 최신 버전 다운로드 경로

{% hint style="info" %}
\.      **[https://hilscher.atlassian.net/](https://hilscher.atlassian.net/wiki/spaces/HILKB/overview?mode=global) -> Software -> SYCON.net** 를 클릭합니다.
{% endhint %}

<br>

![[그림 1.1.1-1 Sycon.net 설치 화면]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_1.png>)

<br>

![[그림 1.1.1-2 Sycon.net 설치 화면]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_2.png>)

<br>

{% hint style="info" %}
\.      최신버전 (Current Release)을 선택하고 다운로드 합니다.
{% endhint %}

<br>

![[그림 1.1.1-3 Sycon.net 설치 화면]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_3.png>)

<br>

![[그림 1.1.1-4 Sycon.net 설치 화면]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_4.png>)

<br>

{% hint style="info" %}
\.      다운로드한 SYCON.NET  Setup.exe 파일을 실행하여 프로그램을 설치합니다.
{% endhint %}

<br>

![[그림 1.1.1-5 Sycon.net 설치 화면]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_5.png>)

<br>

![[그림 1.1.1-6 Sycon.net 설치 화면]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_6.png>)

<br>

{% hint style="info" %}
\.      설치한 SYCON.NET 프로그램을 실행하여 정상적으로 설치가 완료되었는지 확인합니다.
{% endhint %}

<br>

![[그림 1.1.1-7 Sycon.net 설치 화면]](<../../_assets/1-cifx-pci-communication/1-cifx-pci-install-program/1-Sycon/image_7.png>)

<br>


##### 2. 현대 로보틱스 홈페이지에서 프로그램 다운로드

{% hint style="info" %}
\.      [www.hd-hyundairobotics.com](https://hd-hyundairobotics.com/) -> 산업용 로봇 홈페이지 -> 고객지원 -> 응용소프트웨어에서 “**Sycon.net**”을 다운로드 합니다.
{% endhint %}

<br>

{% hint style="info" %}
\.      압축 해제 -> SYCON.NET  Setup.exe 파일을 실행하여 프로그램을 설치합니다.
{% endhint %}

<br>

{% hint style="info" %}
\.      당사 홈페이지에서 제공하는 SYCON.net 프로그램은 최신버전과 다를 수 있습니다.
{% endhint %}

<br>
[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/README.md)
# 1.2 CIFX PCI 통신 카드 장착 및 설정

산업용 통신을 사용하기 위해서는 PCI 통신 카드(hilscher 사)가 필요합니다. 필요한 통신에 맞추어서 통신 카드의 설정과 커넥터를 결선합니다.

[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)
# 1.2.1 PCI 산업용 통신 카드


<br>

##### 1. 구입한 PCI 통신 카드를 제어기 내부 메인모듈에 장착하십시오.

<br>

##### 2. PCI 통신 카드의 Rotary Switch를 돌려서 Slot(슬롯) 번호를 설정해 주십시오.

<br>

{% hint style="warning" %}
**\[주의]**: 제어기 내부 PCI 슬롯의 물리적 위치와 통신 카드의 Rotary Switch 슬롯 번호 설정은 서로 무관합니다. 
{% endhint %}

<br>

##### 3. Slot(슬롯) 번호는 1 \~ 3번 내에서 PCI 통신 카드 별 각각 설정해주십시오.
  (여러 개의 PCI 통신 카드 사용시 번호를 모두 다르게 설정해야 합니다.)

![[그림 1.2.1-1 PCI 통신 카드]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_2.png>)

<br>

![[그림 1.2.1-2 PCI 통신 카드]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI/image_3.png>)

{% hint style="warning" %}
**\[주의]**: Rotary Switch번호는 PCI 카드마다 다르게 설정하시기 바랍니다.
{% endhint %}


[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)
# 1.2.2 커넥터

<br>

##### 산업용 통신 방식에 맞는 커넥터와 케이블을 사용하십시오.

![[그림 1.2.2-1 산업용 통신 커넥터]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector/image_2.png>)

{% hint style="info" %}
\.      DeviceNet 종단 저항 : 120옴

\.      CC-Link 종단 저항 : 110옴
{% endhint %}

<br>

{% hint style="warning" %}
**\[주의]**: 통신 케이블 전원과 IO 전원은 서로 분리하여 구성해 주십시오.
{% endhint %}

<br>
[__SOURCE](1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led.md)
# 1.2.3 LED 설명

<br>

### PCI LED 설명

<br>

![[Figure 1.2.3-1 PCI Communication Card]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_1.png>)
![](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_2.png>)

<br>

![[Figure 1.2.3-3 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_3.png>)

<br>

![[Figure 1.2.3-4 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_4.png>)

<br>

![[Figure 1.2.3-5 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_5.png>)

<br>

![[Figure 1.2.3-6 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_6.png>)

<br>

![[Figure 1.2.3-7 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_7.png>)

<br>

![[Figure 1.2.3-8 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_8.png>)

<br>

![[Figure 1.2.3-9 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_9.png>)

<br>

![[Figure 1.2.3-10 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_10.png>)

<br>

![[Figure 1.2.3-11 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_11.png>)

<br>

![[Figure 1.2.3-12 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_12.png>)

<br>

![[Figure 1.2.3-13 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_13.png>)

<br>

![[Figure 1.2.3-14 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_14.png>)

<br>

![[Figure 1.2.3-15 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_15.png>)

<br>

![[Figure 1.2.3-16 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_16.png>)

<br>

![[Figure 1.2.3-17 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_17.png>)

<br>

![[Figure 1.2.3-18 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_18.png>)

<br>

![[Figure 1.2.3-19 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_19.png>)

<br>

![[Figure 1.2.3-20 PCI LED]](<../../_assets/1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/3-Led/image_20.png>)

<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/README.md)
# 1.3 CIFX PCI 통신 설정

산업용 통신을 사용하기 위해 PCI 통신 카드 장착한 후, 티치 팬던트 및 Sycon.net프로그램을 이용하여 설정을 진행해 주십시오.

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)
# 1.3.1 CIFX PCI 슬롯 설정.

CIFX PCI 슬롯의 통신 방식을 설정합니다. 설정 적용을 위해서는 제어기 전원을 차단한 후 다시 공급해주시기 바랍니다.

<br>

“[**1.2.1 PCI 산업용 통신 카드**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" 참고하여 아래 방법을 진행해 주십시오.

<br>

##### 1. 메뉴를 터치하여 슬롯 설정 화면으로 진입 합니다.
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 1: PCI 슬롯 설정 > 1 채널]** 


<br>

##### 2. 아래 화면을 참고하여 슬롯과 통신 방식(Master/Slave), 프로토콜을 선택 합니다.
   * 슬롯 번호는 PCI 통신 카드의 Rotary Swtich 번호 입니다.
   * 통신 설정 변경을 원하지 않을 경우 **\[OK]** 버튼을 터치하여 종료합니다.

{% hint style="warning" %}
**\[주의]**: **\[초기화]** 또는 **\[적용]** 버튼을 터치하면 현재 탭의 슬롯 정보가 초기화 됩니다. Config 파일도 같이 초기화 되니 유의하시기 바랍니다.
{% endhint %}

![[그림 1.3.1-1 PCI 슬롯 설정]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[그림 1.3.1-2 PCI 슬롯 설정(master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[그림 1.3.1-3 PCI 슬롯 설정(Slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

##### 3. 슬롯 설정을 완료 합니다.
**\[적용]** 메뉴를 터치

![[그림 1.3.1-4 PCI 슬롯 설정]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[주의]**

<1>. **\[적용]** 버튼을 터치하여 설정 시 해당 슬롯에 적용 되어있는 CONFIG 파일이 모두 삭제된 후 변경됩니다. 통신을 변경 하실 경우 기존 설정을 별도로 보관하는 것을 권장합니다.

<2>. **\[적용]** 버튼을 터치하지 않고 **\[OK]**버튼을 터치할 경우 선택한 통신이 적용되지 않습니다.
{% endhint %}

<br>

##### 4. 각 슬롯마다 2. \~ 3.번을 반복하여 설정해 줍니다.

<br>

##### 5. 제어기를 재부팅하여 설정한 통신을 적용합니다.
**\[서비스 > 19: 산업용 통신 모니터링]** 메뉴를 터치하여 설정한 통신이 적용 되었는지 확인합니다.

![[그림 1.3.1-5 산업용 통신 설정 화면]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[주의]**: 슬롯 설정 후 제어기를 재부팅 할 때 설정값이 적용됩니다.
{% endhint %}

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)
# 1.3.2 SYCON.NET 설정

PCI 통신 카드는 “**Sycon.net**” 프로그램을 이용하여 산업용 통신 설정을 진행합니다. 설정 방법은 다음과 같습니다. (“[**1.1 Sycon.net 설치**](../../1-cifx-pci-install-program/1-sycon-net.md)”을 참고하여 설치해주시기 바랍니다.)

<br>

##### 1. Sycon.net 설치된 PC와 로봇 제어기의 범용 LAN포트를 연결 합니다. (PCI LAN Port X)
**\[시스템 > 2: 제어 파라미터 > 9: 네트워크]** 메뉴를 터치하여 범용 LAN포트의 IP를 확인합니다. Ping Test 등을 통해 연결 여부를 확인해 주십시오.

![[그림 1.3.2-1 네트워크 IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_1.png>)
![[그림 1.3.2-2 네트워크 IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_2.png>) 

{% hint style="info" %}
\.      IP Address는 사용자 설정에 따라 변경 가능합니다.
{% endhint %}

<br>

##### 2. Sycon.net 을 실행합니다.

![[그림 1.3.2-3 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_3.png>)

<br>

##### 3. 화면 오른쪽 Device Catalog 에서 설정한 통신 Protocol에 맞는 항목을 클릭하여 Drag & Drop 으로 중앙의 버스 라인에 놓습니다. 

![[그림 1.3.2-4 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_4.png>)
![[그림 1.3.2-5 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_5.png>)

<br>

##### 4. 가져온 항목을 더블클릭하여 설정합니다.

{% hint style="info" %}
\.      가져온 CIFX PCI (그림) “Double Click”

\.      Settings -> Driver 

\.      netX Driver를 선택합니다.
{% endhint %}

![[그림 1.3.2-6 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_6.png>)

{% hint style="info" %}
\.     Setting -> Driver -> netX Driver -> TCP Connection 

\.     IP Address : 연결된 제어기의 범용 LAN Port IP 주소를 입력해 주십시오.
{% endhint %}

![[그림 1.3.2-7 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_7.png>)

{% hint style="info" %}
\.      Device Assignment -> Scan클릭

\.      통신(Channel Protocol 확인)을 선택 후 “Apply” 이후 “OK”
{% endhint %}

{% hint style="warning" %}
**\[주의]**: Channel Protocol 과 Slot 번호를 반드시 확인해 주십시오.
{% endhint %}

{% hint style="warning" %}
**\[주의]**: Scan 이 안되는 경우 제어기와의 Cable 연결 상태, 펌웨어 설정을 확인해 주십시오.
{% endhint %}

![[그림 1.3.2-8 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_8.png>)


{% hint style="info" %}
\.      CIFX PCI 그림 우클릭 -> DOWNLOAD
{% endhint %}

![[그림 1.3.2-9 Sycon.net]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/image_9.png>)
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)
# 1.3.2.1 SYCON.NET 도움말



<br>

##### SYCON.net 이용 중 매뉴얼에 설명이 부족한 부분은 아래 "help" 기능을 참고해 주십시오.

<br>

![[그림 1.3.2.1-1 SYCON.net help]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/1-Help-SYCON/image_1.png>) 

<br>

![[그림 1.3.2.1-2 SYCON.net help]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Setting-SYCON/1-Help-SYCON/image_2.png>) 

<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/README.md)
# 1.3.3 EtherNet/IP

이 장에서는 EtherNet/IP Master(Scanner) 와 Slave(Adapter)의 특성과 설정 방법에 대해 기술합니다. 

<br>

##### EtherNet/IP 개요

EthetNet/IP 는 CI(ControlNet International)와 ODVA(Open DeviceNet Vendors Association)에 의해 개발된 이더넷 기반의 개방형 산업용 통신 프로토콜입니다.

공장에서 센서, 리모트 IO, 모터 드라이버, HMI, PLC, 로봇 제어기 등 다양한 장치가 제조사와 무관하게 하나의 EtherNet/IP 네트워크에 연결될 수 있습니다.

![[그림 1.3.3-1 EtherNet/IP]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/image_1.png>)
 

<br>

EtherNet/IP 는 통신 기능에 따라 아래와 같이 구분합니다.

##### Scanner Class
   * 기존 필드버스 마스터(Master)에 해당되는 제품들로 EtherNet/IP Adapter 또는 Scanner 에게 I/O 데이터 연결을 요청할 수 있습니다.

<br>

##### Adapter Class
  * 기존 필드버스 슬레이브(Slave)에 해당되는 제품들로 EtherNet/IP Scanner 에 의해 요청되는 Real-Time I/O 데이터의 연결 타겟(Target)에 해당됩니다.
    
  * Adapter는 Scanner 에 의하지 않고서는 스스로 Real-Time I/O 데이터를 송수신 할 수 없습니다.

<br>

##### Messaging Class
   * 모든 Class 의 제품의 대해 Explicit 메세지 송수신이 가능한 제품들로 Real-Time I/O 데이터 송수신은 지원하지 않습니다.
   
   * 예를 들면 프로그램 업로드 / 다운로드용 컴퓨터 인터페이스 카드, 네트워크 설정 Tool 등이 해당 될 수 있습니다.
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/1-Specification-EtherNet-IP-Scanner.md)
# 1.3.3.1 EtherNet/IP Scanner 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>최대 연결 가능한 slave 수</td>
		<td>64개</td>
	</tr>
    <tr>
		<td>최대 입력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 입력 크기 (1 slave)</td>
		<td>504 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기 (1 slave)</td>
		<td>504 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td>Cyclic</td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td>최소 1ms</td>
	</tr>
    <tr>
		<td>통신 속도</td>
		<td>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Tree, Line, Ring</td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>DLR (Device Level Ring)</td>
		<td>Beacon based 'Ring Node'</td>
	</tr>
    <tr>
		<td>부가 기능</td>
		<td>DHCP, BOOTP, ACD 지원</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>10 or 100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>사용 가능</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>사용 가능</td>
	</tr>
</tbody>
</table>
<br>

##### 물리적 연결

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>케이블</td>
		<td>최소 Cat5 이상, STP 케이블</td>
	</tr>
	<tr>
		<td>길이</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Settings-EtherNet-IP-Scanner.md)
# 1.3.3.2 EtherNet/IP Scanner 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 및 "[**1.3.2 SYCON.NET 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      SYCON.net 이용 중 매뉴얼에 설명이 부족한 부분은  ""[**1.3.2 SYCON.NET 도움말**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" 기능을 참고해 주십시오.
{% endhint %}

<br>

##### 1. PCI 슬롯 설정에서 EtherNet/IP Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.3.2-1 PCI 슬롯 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

<br>

{% hint style="info" %}
\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

<br>

![[그림 1.3.3.2-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

##### 3. Sycon.net 을 이용하여 EtherNet/IP Scanner PCI 장치를 선택합니다.

![[그림 1.3.3.2-3 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_3.png>)
![[그림 1.3.3.2-4 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

##### 4. PCI 장치를 Scan 하고 EtherNet/IP Scanner 적용(Apply)합니다.

![[그림 1.3.3.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

##### 5. 설정을 다운로드 합니다.

![[그림 1.3.3.2-6 EtherNet/IP Scanner Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

##### 6. EtherNet/IP Scanner 에 연결할 Adapter(Slave) 모듈을 준비합니다.
   * 이번 예제에서는 Crevis 사의 M9289 EtherNet/IP Adapter를 사용합니다.
   * 시스템 전원과 필드 전원을 공급해 주어 모듈을 활성화 시켜 주십시오.

![[그림 1.3.3.2-7 Crevis M9289]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

##### 7. EtherNet/IP 통신 연결을 위해 Apdapter(Slave) 의 IP Address를 설정합니다.

{% hint style="info" %}
\.      Dip Switch 를 이용한 IP Address 설정
{% endhint %}

![[그림 1.3.3.2-8 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
\.      BootpSvr.exe 을 이용한 IP Address 설정 방법
{% endhint %}

<br>

##### 8. (Bootp 예제) Bootp를 이용하여 Slave 장치의 IP Address를 설정합니다.
   * 9번 DIP Switch만 ON으로 변경합니다.

![[그림 1.3.3.2-9 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_9.png>)

   * M9289 Adapter LAN 포트에 PC를 연결합니다.

![[그림 1.3.3.2-10 Crevis M9289 LAN Port]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

##### 9. PC 에서 BootpSvr.exe 를 실행합니다.
   * 해당 프로그램은 Crevis 사에서 제공합니다. (홈페이지에서 IO Guide Pro 다운로드 후 설치)

![[그림 1.3.3.2-11 Crevis IO Guide Pro]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_11.png>)

![[그림 1.3.3.2-12 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
\.      Start BootP를 누른 상태에서 M9289 모듈의 전원을 분리하고 다시 인가하여 재부팅합니다.
{% endhint %}

![[그림 1.3.3.2-13 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

##### 10. Adapter 장치를 재부팅하면 BootpSvr.exe 프로그램에 Device 정보가 나타납니다.

![[그림 1.3.3.2-14 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

##### 11. Device를 선택하여 IP를 설정합니다.

![[그림 1.3.3.2-15 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_15.png>)![[그림 1.3.3.2-16 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

##### 12. IP 설정이 끝난 Adapter의 DIP Switch를 모두 OFF로 변경한 후 장치를 재부팅합니다.

{% hint style="info" %}
\.      DIP Switch의 상태 Adapter 재부팅 여부를 반드시 확인해 주십시오.
{% endhint %}

![[그림 1.3.3.2-17 Crevis DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

##### 13. Slave 장치의 EDS 파일을 등록합니다.

{% hint style="info" %}
\.      Sycon.net에 등록되지 않은 Device를 사용하기 위해 EDS 파일이 필요합니다.

\.      M9289 Adapter의 EDS 파일은 Crevis 홈페이지에서 다운로드 할 수 있습니다.
{% endhint %}

![[그림 1.3.3.2-18 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
\.      다운로드한 EDS 파일을 Sycon.net 에 등록합니다.

\.      EDS File 등록시 산업용 통신 Protocol (EtherNet/IP)를 확인해 주십시오.
{% endhint %}

![[그림 1.3.3.2-19 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_19.png>)![[그림 1.3.3.2-20 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_20.png>)
![[그림 1.3.3.2-21 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_21.png>)

![[그림 1.3.3.2-22 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

##### 14. Network Scan

{% hint style="info" %}
\.      EtherNet/IP Scanner 는 Network Scan 기능을 지원하지 않습니다.
{% endhint %}

<br>

##### 15. Slave(Adapter) 장치 Configuration

{% hint style="info" %}
\.      동록한 Device를 끌어와 EtherNet/IP Master 버스 라인에 올려 놓습니다.
{% endhint %}

![[그림 1.3.3.2-23 Sycon.net Bus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      해당 Device (Adapter)를 더블클릭하여 설정을 진행합니다.

\.      해당 Device에 장착된 IO 장치에 알맞게 Input / Output Byte 수를 설정합니다.

\.      이 예제에서는 아래와 같이 설정했습니다.
{% endhint %}

<br>

![[그림 1.3.3.2-24 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.        O -> T : Originator(Master) -> Target (Slave)

\.        Output : EtherNet/IP Scanner  -> M9289

\.        [Output Module]   
\.         1. M225F (2Bytes)   
\.         **=> 2Bytes**   
{% endhint %}

<br>

![[그림 1.3.3.2-25 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.        T -> O : Target (Slave) -> Originator(Master)

\.        Input : M9289 -> EtherNet/IP Scanner

\.        [Input Module]   
\.         1. M7001  (1Byte)   
\.         2. M12DF  (2Bytes)   
\.         **=> 3Bytes**


\.         1.M7002 (0Byte)
\.         2.M12DF (2Bytes)
\.         **=> 2Bytes**  
{% endhint %}

<br>

##### 16. Master(Scanner) 장치 Configuration
    

{% hint style="info" %}
\.        Master Device를 우클릭하여 Disconnect 합니다.
{% endhint %}

![[그림 1.3.3.2-26 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Master Device를 더블클릭합니다.

\.        Master Device의 IP Address를 설정합니다. 
{% endhint %}

![[그림 1.3.3.2-27 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.        Slave Device의 IP Address를 설정합니다. 
{% endhint %}

![[그림 1.3.3.2-28 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.        Slave Device의 Scan Time을 설정합니다. 

\.        해당 값을 조절하여 적절한 통신 속도를 설정해 주십시오.
{% endhint %}

![[그림 1.3.3.2-29 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.        Address Table에서 Slave 장치의 설정을 확인해 주십시오.

\.        Input / Output IO Byte 수와 시작 Address 를 확인해 주십시오.
{% endhint %}

![[그림 1.3.3.2-30 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
\.        [Quick Connect]

\.        EtherNet/IP는 Quick Connect 기능을 지원합니다.
{% endhint %}

{% hint style="info" %}
\.        Quick Connect 기능 사용을 위해 아래 조건을 만족해야 합니다.

\.        (1) Master, Slave Quick Connect 지원 제품 필요  
\.        (2) Auto Negotiation 사용시 Quick Connect 사용 불가  
\.        (3) Auto MDI-X 사용시 Quick Connect 사용 불가  
\.        (4) 100 Mbit/s, Full Duplex 사용 필요  
{% endhint %}

{% hint style="info" %}
\.        설정을 완료 후 Download를 진행해 주십시오.
{% endhint %}

![[그림 1.3.3.2-31 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

##### 17. 통신 상태 확인

{% hint style="info" %}
\.        Sycon.net 과 TP 에서 통신 상태를 확인 합니다.

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      Connected 된 Master 장치를 더블클릭하여 통신 상태를 확인 할 수 있습니다.
{% endhint %}

![[그림 1.3.3.2-32 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_32.png>)

![[그림 1.3.3.2-33 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
\.        Sycon.net 의 Diagnosis 기능을 이용하여 통신 상태와 함게 IO 입출력 상태를 모니터링 할 수 있습니다.
{% endhint %}

![[그림 1.3.3.2-34 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_34.png>)

<br>

##### 18. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/3-Specification-EtherNet-IP-Adapter.md)
# 1.3.3.3 EtherNet/IP Adapter 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>최대 입력 크기</td>
		<td>240 bytes (TP) / 504 bytes (Sycon.net)</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>240 bytes (TP) / 504 bytes (Sycon.net)</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td>1 exlusive Owner <br>1 Listen Only <br>1 Input Only</td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td>최소 1ms</td>
	</tr>
    <tr>
		<td>통신 속도</td>
		<td>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Tree, Line, Ring</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>DLR V2 (Device Level Ring)</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>부가 기능</td>
		<td>DHCP, BOOTP, ACD 지원</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>10 or 100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>사용 가능</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>사용 가능</td>
	</tr>
</tbody>
</table>
<br>

##### 물리적 연결

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>케이블</td>
		<td>최소 Cat5 이상, STP 케이블</td>
	</tr>
	<tr>
		<td>길이</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Settings-EtherNet-IP-Adapter.md)
# 1.3.3.4 EtherNet/IP Adapter 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      **[EtherNet/IP Adapter EDS File 다운로드]**

\.      “[**5. Slave 장치 설명 파일**](../../../5-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

<br>

##### 1. TP를 이용하여 산업용 통신 펌웨어 설정에서 EtherNet/IP Slave를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.3.4-1 펌웨어 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.

![[그림 1.3.3.4-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

##### 3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬레이브 슬롯 설정 >  EtherNet/IP Slave]**

![[그림 1.3.3.4-3 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[그림 1.3.3.4-4 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

##### 4. 각 항목 별 설명

{% hint style="info" %}
\.      [IP 설정 (IP Setting)]

\.      고정 IP : 사용자가 IP 주소, 서브넷 마스크, 게이트 웨이 정보를 설정합니다.

\.      동적할당(DHCP) : DHCP 서버에서 IP 주소를 할당 받습니다.
{% endhint %}

{% hint style="info" %}
\.      [통신 에러시 입력 (Action in Bus Error)]

\.      Clear : 통신 에러 발생시 모든 입력을 0 으로 초기화 합니다.

\.      Hold : 통신 에러 발생시 마지막 유효 입력 값을 유지합니다.
{% endhint %}

{% hint style="info" %}
\.      [통신 에러 허용시간 (Error Allowed Time)]

\.      지정한 허용 시간동안 통신에러가 지속되면 필드버스 이상 신호와 알람을 출력합니다.
{% endhint %}

{% hint style="info" %}
\.      [입력 바이트 수 (Input Byte)]

\.      입력 바이트 수 : Master -> Slave 로 입력되는 데이터 크기를 설정합니다.

\.      O -> T : Originator(Master) -> Target (Slave)
{% endhint %}

{% hint style="info" %}
\.      [출력 바이트 수 (Output Byte)]

\.      출력 바이트 수 : Slave -> Master 로 출력하는 데이터 크기를 설정합니다.

\.      T -> O : Target (Slave) -> Originator(Master)
{% endhint %}

{% hint style="info" %}
\.      [Run / Idle Header]

\.      제어기에 적용된 CIFX-50 RE EtherNet/IP Adapter 는 Scanner와 IO 교환 시 32Bit Run / Idle Header 를 사용합니다. (Default)

\.      Scanner 사양에 따라 입력 및 출력 32Bit Run / Idle Header 사용 여부를 적절히 설정하여 주십시오.
{% endhint %}

<br>

{% hint style="info" %}
\.        [Quick Connect]

\.        EtherNet/IP는 Quick Connect 기능을 지원합니다.

\.        Quick Connect 기능 사용이 필요한 경우 Sycon.net 을 이용하여 EtherNet/IP Adapter를 설정해 주십시오.

\.        (1) Master, Slave Quick Connect 지원 제품 필요  
\.        (2) Auto Negotiation 사용시 Quick Connect 사용 불가  
\.        (3) Auto MDI-X 사용시 Quick Connect 사용 불가  
\.        (4) 100 Mbit/s, Full Duplex 사용 필요  
{% endhint %}

<br>

##### 5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[그림 1.3.3.4-5 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_5.png>) 

<br>

##### 6. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error-EtherNet-IP.md)
# 1.3.3.5 EtherNet/IP 에러 조치

EthernNet/IP 설정 중 발생할 수 있는 주요 Error 를 해결하기 위한 방법입니다.

Sycon.Net 의 Diagnosis 를 이용해 Error를 확인 할 수 있습니다.

<br>

"[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)" 참고해 주십시오.

<br>

##### 1. 통신 케이블 단선 에러

{% hint style="info" %}
\.      LAN Cable 의 연결 상태를 확인해 주십시오.

\.      Adapter Device 의 전원이 켜져 있는지 확인해 주십시오.
{% endhint %}

![[그림 1.3.3.5-1 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_1.png>) 


<br>

##### 2. IP Address 설정 Error

{% hint style="info" %}
\.      Master - Slave Device 의 IP Address 를 확인해 주십시오.

\.      Adapter Device의 설정된 IP Address 와 Sycon.net 에서 입력한 값이 다른 경우 Error 가 발생합니다.

{% endhint %}

![[그림 1.3.3.5-2 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_2.png>) 

![[그림 1.3.3.5-3 Communication Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/5-Error/image_3.png>) 



[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/README.md)
# 1.3.4 PROFINET IO

이 장에서는 PROFINET IO Master(Controller) 와 Slave(Device)의 특성과 설정 방법에 대해 기술합니다. 

<br>

##### PROFINET IO 개요

PROFINET IO 는 PROFIBUS-DP와 산업용 이더넷으로부터 진보적으로 발전된 이더넷 기반의 개방형 산업용 통신 프로토콜입니다.

![[그림 1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>) 

<br>

데이터 교환을 위해 Provider, Consumer 모델을 따르고 있으며 아래 3가지 Class로 제품을 구분할 수 있습니다.

##### IO Controller Class
   * 기존 PROFIBUS-DP Class 1 마스터(Master)에 해당되는 제품으로 PLC와 같이 자동화 프로그램이 동작하는 제품입니다.

   * IO Controller 는 자신에게 설정된 IO Device 들에게 출력 데이터를 공급하고, 입력 데이터를 소비합니다.

<br>

##### IO Device Class
  * 기존 PROFIBUS-DP 슬레이브(Slave)에 해당되는 제품으로 PLC와 같은 IO Controller에 PROFINET IO를 통해 연결됩니다.
    
  * IO Device 는 IO Controller 에게 출력 데이터를 공급하고, 입력 데이터를 제공하고, 출력 데이터를 소비합니다.

<br>

##### IO Supervisor Class
   * 기존 PROFIBUS-DP 에서 Class 2 마스터(Master)에 해당되는 제품으로 네트워크 구성 및 진단을 목적으로 한 프로그래밍 장치, PC, HMI 등이 있습니다.

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/1-Specification-PROFINET-IO-Controller.md)
# 1.3.4.1 PRFINET IO Controller 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>최대 연결 가능한 slave 수</td>
		<td>128개</td>
	</tr>
    <tr>
		<td>최대 입력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 입력 크기 (1 slave)</td>
		<td>1024 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기 (1 slave)</td>
		<td>1024 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td>최소 1ms</td>
	</tr>
   <tr>
		<td>통신 속도</td>
		<td>100 Mbit/s (Full-Duplex)</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Tree, Line</td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>DCP</td>
		<td>지원</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>사용 불가능</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>제한 사용 가능 (Priority Tagging, LLDP 지원 필요)</td>
	</tr>
</tbody>
</table>
<br>

##### 물리적 연결

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>케이블</td>
		<td>최소 Cat5 이상, STP 케이블</td>
	</tr>
	<tr>
		<td>길이</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Settings-PROFINET-IO-Controller.md)
# 1.3.4.2 PROFINET IO Controller 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 및 "[**1.3.2 SYCON.NET 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      SYCON.net 이용 중 매뉴얼에 설명이 부족한 부분은  ""[**1.3.2 SYCON.NET 도움말**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" 기능을 참고해 주십시오.
{% endhint %}

<br>

##### 1. PCI 슬롯 설정에서 PROFINET IO Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.4.2-1 PCI 슬롯 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

<br>

{% hint style="info" %}
\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

<br>

![[그림 1.3.4.2-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

##### 3. Sycon.net 을 이용하여 PROFINET IO Controller PCI 장치를 선택합니다.

![[그림 1.3.4.2-3 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_3.png>)
![[그림 1.3.4.2-4 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

##### 4. PCI 장치를 Scan 하고 PROFINET IO Controller 적용(Apply)합니다.

![[그림 1.3.4.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

##### 5. 설정을 다운로드 합니다.

![[그림 1.3.4.2-6 PROFINET IO Controller Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

##### 6. PROFINET IO Controller 에 연결할 Device(Slave) 모듈을 준비합니다.
   * 이번 예제에서는 Crevis 사의 M9287 PROFINET IO Device를 사용합니다.
   * 시스템 전원과 필드 전원을 공급해 주어 모듈을 활성화 시켜 주십시오.

![[그림 1.3.4.2-7 Crevis M9287]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
\.      DIP Switch 을 이용한 PROFINET IO Device 이름 설정 방법

\.      M9287-XX : Dip Switch 로 설정한 번호

\.      이번 예제에서는 1번 Dip Switch를 이용해 이름을 M9287-01 로 설정하였습니다.
{% endhint %}

<br>

##### 7. (Dip Switch 예제) DIP Switch를 이용하여 Slave 장치의 이름을 설정합니다.
   * 1번 DIP Switch만 ON으로 변경합니다.


![[그림 1.3.4.2-8 Crevis M9287 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      DIP Switch 설정 후 장치를 재부팅 해주십시오.
{% endhint %}

<br>

##### 8. Slave 장치의 GSDML 파일을 등록합니다.

{% hint style="info" %}
\.      Sycon.net에 등록되지 않은 Device를 사용하기 위해 GSDML 파일이 필요합니다.

\.      M9287 Device의 GSDML 파일은 Crevis 홈페이지에서 다운로드 할 수 있습니다.
{% endhint %}

![[그림 1.3.4.2-9 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      다운로드한 GSDML 파일을 Sycon.net 에 등록합니다.

\.      GSDML File 등록시 산업용 통신 Protocol (PROFINET IO)를 확인해 주십시오.
{% endhint %}

![[그림 1.3.4.2-10 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_10.png>)![[그림 1.3.4.2-11 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_11.png>)
![[그림 1.3.4.2-12 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_12.png>)

![[그림 1.3.4.2-13 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_13.png>)


<br>

##### 9. Network Scan

{% hint style="info" %}
\.      PROFINET IO Controller 는 Network Scan 기능을 지원합니다.
{% endhint %}

{% hint style="info" %}
\.      PROFINET IO Master 장치에서 우클릭 후 Network Scan을 클릭합니다.
{% endhint %}

![[그림 1.3.4.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      GSDML 파일이 등록되지 않은 경우 Network Scan을 하면 Slave 정보는 나타나지만 등록은 불가능합니다.
{% endhint %}

![[그림 1.3.4.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      정상적으로 GSDML 파일이 등록된 경우 Network Scan을 통해 Slave 장치를 추가할 수 있습니다.
{% endhint %}

![[그림 1.3.4.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_16.png>)

![[그림 1.3.4.2-17 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_17.png>)

![[그림 1.3.4.2-18 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

##### 10. Slave(Device) 장치 Configuration

{% hint style="info" %}
\.      Slave 장치 Configuration을 위해 Master 장치의 Disconnect를 클릭합니다.
{% endhint %}

![[그림 1.3.4.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      Slave 장치를 더블클릭합니다.
{% endhint %}

![[그림 1.3.4.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      PROFINET IO Slave(Device) 설정을 위해 M9287에 연결되어 있는 Slot을 추가합니다.

\.      Slot 1 : M7001  
\.      Slot 2 : M12DF  
\.      Slot 3 : M225F  
{% endhint %}

![[그림 1.3.4.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_21.png>)

![[그림 1.3.4.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

##### 11. Master(Controller) 장치 Configuration

{% hint style="info" %}
\.      Master 장치를 더블클릭합니다.
{% endhint %}

![[그림 1.3.4.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      Master 장치와 Slave 장치의 IP 주소를 설정해줍니다.

\.      PROFINET IO Device의 Slave IP 주소는 Master 에서 설정합니다.

\.      IP 주소는 Master와 Slave가 같은 대역안에서 서로 중복되지 않도록 해주십시오.
{% endhint %}

![[그림 1.3.4.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_24.png>)

![[그림 1.3.4.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      Master 장치에서 Slave 장치의 Slot 정보가 올바른지 확인해주십시오.
{% endhint %}

![[그림 1.3.4.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.      Address Table에서 각 Slave Slot의 할당된 IO 및 시작 주소를 확인 합니다.
{% endhint %}

![[그림 1.3.4.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.      PROFINET IO의 IO 통신속도를 설정합니다.
{% endhint %}

![[그림 1.3.4.2-28 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.      설정을 완료 후 Download를 진행해 주십시오.
{% endhint %}

![[그림 1.3.4.2-29 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

##### 12. 통신 상태 확인

{% hint style="info" %}
\.        Sycon.net 과 TP 에서 통신 상태를 확인 합니다.

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      Connected 된 Master 장치를 더블클릭하여 통신 상태를 확인 할 수 있습니다.
{% endhint %}

![[그림 1.3.4.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_30.png>)

![[그림 1.3.4.2-31 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
\.        Sycon.net 의 Diagnosis 기능을 이용하여 통신 상태와 함게 IO 입출력 상태를 모니터링 할 수 있습니다.
{% endhint %}

![[그림 1.3.4.2-32 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_32.png>)

<br>

##### 13. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/3-Specification-PROFINET-IO-Device.md)
# 1.3.4.3 PROFINET IO Deivce 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>최대 입력 크기</td>
		<td>256 bytes (TP) / 1024 bytes (Sycon.net)</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>256 bytes (TP) / 1024 bytes (Sycon.net)</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td>최소 1ms</td>
	</tr>
    <tr>
		<td>통신 속도</td>
		<td>100 Mbit/s (Full-duplex)</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Tree, Line</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>DCP</td>
		<td>지원</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>사용 불가능</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>제한 사용 가능 (Priority Tagging LLDP 지원 필요)</td>
	</tr>
</tbody>
</table>
<br>

##### 물리적 연결

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>케이블</td>
		<td>최소 Cat5 이상, STP 케이블</td>
	</tr>
	<tr>
		<td>길이</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Settings-PROFINET-IO-Device.md)
# 1.3.4.4 PROFINET IO Device 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      **[PROFINET IO Device GSDML File 다운로드]**

\.      “[**5. Slave 장치 설명 파일**](../../../5-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

<br>

##### 1. TP를 이용하여 산업용 통신 펌웨어 설정에서 PROFINET IO Slave를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.4.4-1 펌웨어 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.

![[그림 1.3.4.4-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

##### 3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬레이브 슬롯 설정 >  PROFINET IO Slave]**

![[그림 1.3.4.4-3 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[그림 1.3.4.4-4 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

##### 4. 각 항목 별 설명

{% hint style="info" %}
\.      [Station Name]

\.      PROFINET IO는 Station Name을 통해 Slave를 식별합니다.

\.      Naming Rule
\.       > PROFINET IO 로 연결된 Device들의 이름이 중복될 수 없습니다.  
\.       > 최대 240자로 이름을 설정할 수 있습니다.  
\.       > 특수 문자는 "." , "-" 를 사용할 수 있습니다.  
\.       > 문자는 영어 소문자와 숫자를 사용할 수 있습니다.  
\.       > 이름 시작과 끝은 영어 소문자 또는 숫자로 시작해야 합니다.  
{% endhint %}

{% hint style="info" %}
\.      [입력 바이트 수 (Input Byte)]

\.      입력 바이트 수 : Master -> Slave 로 입력되는 데이터 크기를 설정합니다.
{% endhint %}

{% hint style="info" %}
\.      [출력 바이트 수 (Output Byte)]

\.      출력 바이트 수 : Slave -> Master 로 출력하는 데이터 크기를 설정합니다.
{% endhint %}

<br>

{% hint style="info" %}
\.      [**Master 에서 Slot 설정 시**]

\.      Master Input (32byte)  <--  Slave Output (32bytes)

\.      Master Output (256bytes = 64bytes * 4)  -->  Slave Input (256bytes)

\.      4, 8, 16, 32, 64 Bytes -> 각 Bytes 에 맞는 Slot 지정  
\.      128, 256 Bytes -> 64 Bytes Slot 다수 지정 (2개, 4개)

\.      입력 Slot이 출력 Slot 보다 앞에 위치 합니다.
{% endhint %}

<br>

![[그림 1.3.4.4-5 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_5.png>) 


<br>

##### 5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[그림 1.3.4.4-6 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/4-Slave_setting/image_6.png>) 

<br>

##### 6. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/5-Error-PROFINET-IO.md)
# 1.3.4.5 PROFINET IO 에러 조치

<br>

"[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)" 참고해 주십시오.




[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/README.md)
# 1.3.5 EtherCAT

이 장에서는 EtherCAT Master 와 Slave의 특성과 설정 방법에 대해 기술합니다. 

<br>

##### EtherCAT 개요

EtherCAT은 Beckhoff Automation 에서 개발된 이더넷 기반의 Fieldbus 시스템입니다.

EtherCAT 프로토콜은 매우빠른 IO Data 업데이트와 정확한 동기화를 위한 기능을 제공합니다. 

<br>

##### EtherCAT Master
   * 기존 필드버스 마스터(Master)에 해당되는 제품으로 EtherCAT 슬레이브(Slave) 장치들에게 IO 데이터 연결을 요청할 수 있습니다.

<br>

##### EtherCAT Slave
   * 기존 필드버스 슬레이브(Slave)에 해당되는 제품으로 EtherCAT Master 장치에 연결됩니다.

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/1-Specification-EtherCAT-Master.md)
# 1.3.5.1 EtherCAT Master 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>최대 연결 가능한 slave 수</td>
		<td>200개</td>
	</tr>
    <tr>
		<td>최대 입력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 입력 크기 (1 slave)</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기 (1 slave)</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td>최소 250us (1ms 이상 권장)</td>
	</tr>
   <tr>
		<td>통신 속도</td>
		<td>100 Mbit/s (Full-Duplex)</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Line, Ring</td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>Redendance</td>
		<td>지원 (동기화와 동시 적용 불가)</td>
	</tr>
    <tr>
		<td>동기화</td>
		<td>DC (Distributed Clocks)</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>사용 불가능</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>제한 사용 가능 (Master와 1번째 Slave 사이)</td>
	</tr>
</tbody>
</table>
<br>

##### 물리적 연결

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>케이블</td>
		<td>최소 Cat5 이상, STP 케이블</td>
	</tr>
	<tr>
		<td>길이</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Settings-EtherCAT-Master.md)
# 1.3.5.2 EtherCAT Master 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 및 "[**1.3.2 SYCON.NET 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      SYCON.net 이용 중 매뉴얼에 설명이 부족한 부분은  ""[**1.3.2 SYCON.NET 도움말**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" 기능을 참고해 주십시오.
{% endhint %}

<br>

##### 1. PCI 슬롯 설정에서 EtherCAT Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.5.2-1 PCI 슬롯 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

<br>

{% hint style="info" %}
\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

<br>

![[그림 1.3.5.2-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_2.png>) 

<br>

##### 3. Sycon.net 을 이용하여 EtherCAT Master PCI 장치를 선택합니다.

![[그림 1.3.5.2-3 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_3.png>)
![[그림 1.3.5.2-4 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_4.png>) 

<br>

##### 4. PCI 장치를 Scan 하고 EtherCAT Master 적용(Apply)합니다.

![[그림 1.3.5.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_5.png>) 

<br>

##### 5. 설정을 다운로드 합니다.

![[그림 1.3.5.2-6 EtherCAT Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_6.png>) 

<br>

##### 6. EtherCAT Master 에 연결할 Slave 모듈을 준비합니다.
   * 이번 예제에서는 Crevis 사의 M9386 EtherCAT Slave를 사용합니다.
   * 시스템 전원과 필드 전원을 공급해 주어 모듈을 활성화 시켜 주십시오.

![[그림 1.3.5.2-7 Crevis M9386]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_7.png>) 

<br>

##### 7. Slave 장치의 Station Address

{% hint style="info" %}
\.      EtherCAT Slave 장치의 Station Address 는 Master 에서 설정합니다.
{% endhint %}

<br>

##### 8. Slave 장치의 XML 파일을 등록합니다.

{% hint style="info" %}
\.      Sycon.net에 등록되지 않은 Device를 사용하기 위해 XML 파일이 필요합니다.

\.      M9386 Device의 XML 파일은 Crevis 홈페이지에서 다운로드 할 수 있습니다.
{% endhint %}

![[그림 1.3.5.2-8 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      다운로드한 XML 파일을 Sycon.net 에 등록합니다.

\.      XML File 등록시 산업용 통신 Protocol (EtherCAT)를 확인해 주십시오.
{% endhint %}

![[그림 1.3.5.2-9 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_9.png>)

<br>

![[그림 1.3.5.5-10 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_10.png>)

<br>

![[그림 1.3.5.2-11 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_11.png>)

<br>

![[그림 1.3.5.2-12 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_12.png>)


<br>

##### 9. Network Scan

{% hint style="warning" %}
\.      **EtherCAT 은 사용할 수 있는 Cable 결선과 Port 가 지정되어 있습니다.**

\.      **원활한 통신 연결을 위해 (“[**1.3.5.5 EtherCAT 케이블 결선**](../5-EtherCAT/5-EtherCAT-Topology.md)”)을 반드시 확인해 주십시오.**
{% endhint %}

{% hint style="info" %}
\.      EtherCAT Master 는 Network Scan 기능을 지원합니다.
{% endhint %}

{% hint style="info" %}
\.      EtherCAT Master 장치에서 우클릭 후 Network Scan을 클릭합니다.
{% endhint %}

![[그림 1.3.5.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      XML 파일이 등록되지 않은 경우 Network Scan을 하면 Slave 정보는 나타나지만 등록은 불가능합니다.
{% endhint %}

{% hint style="info" %}
\.      정상적으로 XML 파일이 등록된 경우 Network Scan을 통해 Slave 장치를 추가할 수 있습니다.
{% endhint %}

![[그림 1.3.5.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_14.png>)

<br>

##### 10. Slave 장치 Configuration

{% hint style="info" %}
\.      Slave 장치 Configuration을 위해 Master 장치의 Disconnect를 클릭합니다.
{% endhint %}

![[그림 1.3.5.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Slave 장치를 더블클릭합니다.
{% endhint %}

![[그림 1.3.5.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      EtherCAT Slave 설정을 위해 M9386에 연결되어 있는 Slot을 추가합니다.

\.      Slot 1 : M7001  
\.      Slot 2 : M12DF  
\.      Slot 3 : M225F  
{% endhint %}

![[그림 1.3.5.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_17.png>)

![[그림 1.3.5.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_18.png>)


<br>

##### 11. Master 장치 Configuration

{% hint style="info" %}
\.      Master 장치를 더블클릭합니다.
{% endhint %}

![[그림 1.3.5.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      Synchronization : Freerun / DC(Distributed Clocks) 선택

\.      Redundancy 사용 유무 (Distributed Clocks 과 함께 사용 불가)

\.      Bus Cycle Time : 최소 250us 지원 가능 (1ms 이상 권장)
{% endhint %}

<br>

{% hint style="info" %}
\.      각 Slave의 Station Address 를 설정할 수 있습니다.
{% endhint %}

![[그림 1.3.5.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Address Table에서 각 Slave Slot의 할당된 IO 및 시작 주소를 확인 합니다.
{% endhint %}

![[그림 1.3.5.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_21.png>)


{% hint style="info" %}
\.      설정을 완료 후 Download를 진행해 주십시오.
{% endhint %}

![[그림 1.3.5.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_22.png>)

<br>

##### 12. 통신 상태 확인

{% hint style="info" %}
\.        Sycon.net 과 TP 에서 통신 상태를 확인 합니다.

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      Connected 된 Master 장치를 더블클릭하여 통신 상태를 확인 할 수 있습니다.
{% endhint %}

![[그림 1.3.5.2-23 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_23.png>)

![[그림 1.3.5.2-24 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.        Sycon.net 의 Diagnosis 기능을 이용하여 통신 상태와 함게 IO 입출력 상태를 모니터링 할 수 있습니다.
{% endhint %}

![[그림 1.3.5.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_25.png>)

<br>

##### 13. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/3-Specification-EtherCAT-Slave.md)
# 1.3.5.3 EtherCAT Slave 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>최대 입력 크기</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td>최소 250us (1ms 이상 권장)</td>
	</tr>
    <tr>
		<td>통신 속도</td>
		<td>100 Mbit/s (Full-Duplex)</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Line, Ring</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>동기화</td>
		<td>DC (Distributed Clocks)</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>사용 불가능</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>제한 사용 가능 (Master와 1번째 Slave 사이)</td>
	</tr>
</tbody>
</table>
<br>

##### 물리적 연결

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>케이블</td>
		<td>최소 Cat5 이상, STP 케이블</td>
	</tr>
	<tr>
		<td>길이</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/4-Settings-EtherCAT-Slave.md)
# 1.3.5.4 EtherCAT Slave 설정

매뉴얼 준비중입니다.

<br>

{% hint style="info" %}
\.      **[EtherCAT Slave ESI File 다운로드]**

\.      “[**5. Slave 장치 설명 파일**](../../../5-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-EtherCAT-Topology.md)
# 1.3.5.5 EtherCAT 케이블 결선 (Topology)

<br>

EtherCAT 기존 산업용 통신들과 달리 Cable 결선과 사용할 수 있는 Ethernet Port에 제약이 있습니다.

##### 1. Ethernet Port

{% hint style="info" %}
\.      EthreCAT Master와 Slave를 연결하는 경우 Port 0번을 사용해야 합니다.
{% endhint %}

![[그림 1.3.5.5-1 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
\.      Master에 Slave 가 1개 연결되는 경우
{% endhint %}

![[그림 1.3.5.5-2 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
\.      Master에 Slave 가 2개 이상 연결되는 경우

\.      Slave Port 1번에서 다음 Slave Port 0번으로 연결합니다.
{% endhint %}

![[그림 1.3.5.5-3 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_3.png>) 

<br>

##### 2. Redundancy 

{% hint style="info" %}
\.      Master에서 Redundancy 기능을 사용하는 경우 

\.      마지막 Slave의 Port 1번과 Master의 Port 1번을 연결하여 Ring 구조를 형성합니다.
{% endhint %}

![[그림 1.3.5.5-4 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_4.png>) 


<br>

##### 3. Cable 결선 ERROR


"[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)" 참고해 주십시오.

<br>

{% hint style="info" %}
\.      Network Scan 이 안되는 경우

\.      Master에 연결된 Port와 Cable을 확인해 주십시오.
{% endhint %}

![[그림 1.3.5.5-5 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
\.      Topology Error (Configuration 에서 Error)

\.      Master와 Slave 간 Cable 결선을 확인해 주십시오.
{% endhint %}

![[그림 1.3.5.5-6 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
\.      Topology Error 2 (Configuration 에서는 정상이나 진단시 Error)

\.      Master와 Slave 간 Cable 결선을 확인해 주십시오.

\.      Slave와 Slave 간 Cable 결선을 확인해 주십시오.
{% endhint %}

![[그림 1.3.5.5-7 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_7.png>)

![[그림 1.3.5.5-8 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
\.      Mandatory Slave Missing Error

\.      Slave와 Slave 간 Cable 결선을 확인해 주십시오.
{% endhint %}

![[그림 1.3.5.5-9 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_9.png>)
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/README.md)
# 1.3.6 PROFIBUS-DP

이 장에서는 PROFIBUS-DP Master 와 Slave의 특성과 설정 방법에 대해 기술합니다. 

<br>

##### Fieldbus 개요

필드버스(Fieldbus)는 공장에서의 센서나 버튼, 모터 드라이버, 조작 인터페이스 등의 장치를 PLC(Programmable Logic Controller) 와 단일 케이블로 연결하여 동작시키기 위해 개방화된 산업표준입니다.

필드버스는 전체 네트워크의 상태를 중앙에서 모니터링 하거나 재구성하는 등의 지능적인 서비스를 제공합니다.

예를 들면 센서나 스위치에 대해, 단순한 On/Off 만이 아닌 상세한 정보, 동작, 모드 설정 등이 가능합니다.

단일 케이블을 사용하여 배선에 드는 시간과 비용을 절감할 수 있고, 구성이 간단해져 유지보수에 유리합니다.

또한 일반적인 통신의 비결정적 응답 (Non-deterministic Response) 특성의 프로토콜과는 달리, 데이터 응답속도가 보장되어 임계시간 특성이 중요한 산업용도를 만족합니다.

![[그림 1.3.6-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/image_1.png>) 

<br>

1개의 필드버스 네트워크에는 1개의 마스터 (Master) 장치와 다수의 슬레이브(Slave) 장치가 연결됩니다.
마스터 장치는 네트워크 전체를 검색 / 관리하고 슬레이브 장치들과 데이터를 교환합니다.

일반적으로 PLC는 마스터 장치이고, 그 외에 센서나 버튼, 제어기등이 슬레이브 장치로 구성될 수 있습니다.
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/1-Specification-PROFIBUS-DP-Master.md)
# 1.3.6.1 PROFIBUS-DP Master 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>최대 연결 가능한 slave 수</td>
		<td>125개</td>
	</tr>
    <tr>
		<td>최대 입력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 입력 크기 (1 slave)</td>
		<td>244 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기 (1 slave)</td>
		<td>244 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td> - </td>
	</tr>
   <tr>
		<td>통신 속도</td>
		<td>9.6 ~ 12,000 Kbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>Auto Baudrate Detection</td>
		<td>미지원</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>PROFIBUS FDL</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Settings-PROFIBUS-DP-Master.md)
# 1.3.6.2 PROFIBUS-DP Master 설정


“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 및 "[**1.3.2 SYCON.NET 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      SYCON.net 이용 중 매뉴얼에 설명이 부족한 부분은  ""[**1.3.2 SYCON.NET 도움말**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" 기능을 참고해 주십시오.
{% endhint %}

<br>

##### 1. PCI 슬롯 설정에서 PROFIBUS-DP Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.6.2-1 PCI 슬롯 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

<br>

{% hint style="info" %}
\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

<br>

![[그림 1.3.6.2-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_2.png>) 

<br>

##### 3. Sycon.net 을 이용하여 PROFIBUS-DP Master PCI 장치를 선택합니다.

![[그림 1.3.6.2-3 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[그림 1.3.6.2-4 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

##### 4. PCI 장치를 Scan 하고 PROFIBUS-DP Master 적용(Apply)합니다.

![[그림 1.3.6.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>


##### 5. 설정을 다운로드 합니다.

![[그림 1.3.6.2-6 PROFIBUS-DP Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

##### 6. PROFIBUS-DP Master 에 연결할 Slave 모듈을 준비합니다.
   * 이번 예제에서는 Crevis 사의 GN-9222 PROFIBUS-DP Slave를 사용합니다.
   * 시스템 전원과 필드 전원을 공급해 주어 모듈을 활성화 시켜 주십시오.

![[그림 1.3.6.2-7 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_7.png>) 


<br>

##### 7. Slave 장치의 설정

{% hint style="info" %}
\.      PROFIBUS-DP Slave 장치의 Node 번호와 종단을 설정합니다.
{% endhint %}

![[그림 1.3.6.2-8 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_8.png>) 


{% hint style="info" %}
\.      종단 : DIP Switch를 사용하여 종단 설정 (예제 : 종단 처리 ON)

\.      Node ID (Station Number) : DIP Switch를 사용하여 설정 (예제 : Node 3번)
{% endhint %}

<br>

##### 8. Slave 장치의 GSD 파일을 등록합니다.

{% hint style="info" %}
\.      Sycon.net에 등록되지 않은 Device를 사용하기 위해 GSD 파일이 필요합니다.

\.      GN-9222 Device의 GSD 파일은 Crevis 홈페이지에서 다운로드 할 수 있습니다.
{% endhint %}

![[그림 1.3.6.2-9 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      다운로드한 GSD 파일을 Sycon.net 에 등록합니다.

\.      GSD File 등록시 산업용 통신 Protocol (PROFIBUS-DP)를 확인해 주십시오.
{% endhint %}

![[그림 1.3.6.2-10 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_10.png>)

<br>

![[그림 1.3.6.5-11 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_11.png>)

![[그림 1.3.6.5-12 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_12.png>)



<br>

##### 9. Network Scan

{% hint style="warning" %}
\.      **Network Scan 시 아래 사항을 반드시 확인해 주십시오.**

\.      **(1) 케이블 연결 여부**  
\.      **(2) 종단 DIP Switch 사용 여부**  
{% endhint %}

{% hint style="info" %}
\.      PROFIBUS-DP Master 는 Network Scan 기능을 지원합니다.
{% endhint %}

{% hint style="info" %}
\.      PROFIBUS-DP Master 장치에서 우클릭 후 Network Scan을 클릭합니다.
{% endhint %}

![[그림 1.3.6.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      GSD 파일이 등록되지 않은 경우 Network Scan을 하면 Slave 정보는 나타나지만 등록은 불가능합니다.
{% endhint %}

{% hint style="info" %}
\.      정상적으로 GSD 파일이 등록된 경우 Network Scan을 통해 Slave 장치를 추가할 수 있습니다.
{% endhint %}

![[그림 1.3.6.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

##### 10. Slave 장치 Configuration

{% hint style="info" %}
\.      Slave 장치 Configuration을 위해 Master 장치의 Disconnect를 클릭합니다.
{% endhint %}

![[그림 1.3.6.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Slave 장치를 더블클릭합니다.
{% endhint %}

![[그림 1.3.6.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      PROFIBUS-DP Slave의 설정을 확인 합니다.

\.      Slot 1 : GN-9222  
\.      Slot 2 : GT-12DF (Input 2 Byte)  
\.      Slot 3 : GT-227F (Output 2 Byte)  
\.      Slot 4 : GT-3154 (Input 8 Byte)  
\.      Slot 5 : GT-4254 (Output 8 Byte)  
{% endhint %}

![[그림 1.3.6.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_17.png>)

<br>

![[그림 1.3.6.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_18.png>)


<br>

##### 11. Master 장치 Configuration

{% hint style="info" %}
\.      Master 장치를 더블클릭합니다.
{% endhint %}

![[그림 1.3.6.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_19.png>)


{% hint style="info" %}
\.      PROFIBUS-DP 통신 속도를 설정합니다.

\.      9.6 ~ 12000 Kbit/s 
{% endhint %}

![[그림 1.3.6.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Master 장치에서 Slave 장치의 Slot 정보가 올바른지 확인해주십시오.
{% endhint %}

![[그림 1.3.6.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
\.      Address Table에서 각 Slave Slot의 할당된 IO 및 시작 주소를 확인 합니다.
{% endhint %}

![[그림 1.3.6.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
\.      Station Table 에서 각 장치가 활성 상태인지 확인합니다.
{% endhint %}

![[그림 1.3.6.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      설정을 완료 후 Download를 진행해 주십시오.
{% endhint %}

![[그림 1.3.6.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

##### 12. 통신 상태 확인

{% hint style="info" %}
\.        Sycon.net 과 TP 에서 통신 상태를 확인 합니다.

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      Connected 된 Master 장치를 더블클릭하여 통신 상태를 확인 할 수 있습니다.
{% endhint %}

![[그림 1.3.6.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[그림 1.3.6.2-26 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Sycon.net 의 Diagnosis 기능을 이용하여 통신 상태와 함게 IO 입출력 상태를 모니터링 할 수 있습니다.
{% endhint %}

![[그림 1.3.6.2-27 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_27.png>)

<br>

##### 13. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/3-Specification-PROFIBUS-DP-Slave.md)
# 1.3.6.3 PROFIBUS-DP Slave 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>최대 입력 크기</td>
		<td>244 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>244 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td> - </td>
	</tr>
    <tr>
		<td>통신 속도</td>
		<td>9.6 ~ 12,000 Kbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>Auto Baudrate Detection</td>
		<td>지원</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>PROFIBUS FDL</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Settings-PROFIBUS-DP-Slave.md)
# 1.3.6.4 PROFIBUS-DP Slave 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      **[PROFIBUS-DP Slave GSD File 다운로드]**

\.      “[**5. Slave 장치 설명 파일**](../../../5-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

<br>

##### 1. TP를 이용하여 산업용 통신 펌웨어 설정에서 PROFIBUS-DP Slave를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.6.4-1 펌웨어 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.

![[그림 1.3.6.4-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

##### 3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬레이브 슬롯 설정 >  PROFIBUS-DP Slave]**

![[그림 1.3.6.4-3 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_3.png>) 

![[그림 1.3.6.4-4 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_4.png>) 

<br>

##### 4. 각 항목 별 설명

{% hint style="info" %}
\.      [Station Address]

\.      PROFIBUS-DP는 Station Address를 통해 Slave를 식별합니다.
{% endhint %}

{% hint style="info" %}
\.      [입력 바이트 수 (Input Byte)]

\.      입력 바이트 수 : Master -> Slave 로 입력되는 데이터 크기를 설정합니다.
{% endhint %}

{% hint style="info" %}
\.      [출력 바이트 수 (Output Byte)]

\.      출력 바이트 수 : Slave -> Master 로 출력하는 데이터 크기를 설정합니다.
{% endhint %}

{% hint style="info" %}
\.      [**Master 에서 Module 설정 시**]

\.      설정한 바이트 수와 일치하도록 Master에서 Module을 지정해 주어야합니다.

\.      순서 : Master Input (64 ~ 1) -> Master Output (64 ~ 1)

\.      EX) Master Input 109 bytes  <---  Slave Output 109 bytes   
\.          Input 109 Bytes : 64Byte + 32Byte + 8Byte + 4Byte + 1 Byte

\.      EX) Master Output 120 bytes  --->  Slave Input 120 bytes   
\.          Output 120 Bytes : 64Byte + 32Byte + 16Byte + 8Byte


\.      EX) Master Input 12 bytes  <---  Slave Output 12 bytes   
\.          Input 12 Bytes : 8Byte + 4Byte

\.      EX) Master Output 200 bytes  --->  Slave Input 200 bytes   
\.          Output 200 Bytes : 64Byte + 64Byte + 64Byte + 8Byte

\.      입력 Module이 출력 Module 보다 앞에 위치합니다.
{% endhint %}

![[그림 1.3.6.4-5 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_5.png>) 


<br>

##### 5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[그림 1.3.6.4-6 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/4-Slave_setting/image_6.png>) 

<br>

##### 6. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/5-Error-PROFIBUS-DP.md)
# 1.3.6.5 PROFIBUS-DP 에러 조치

<br>

"[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)" 참고해 주십시오.

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/README.md)
# 1.3.7 DeviceNet

이 장에서는 DeviceNet Master 와 Slave의 특성과 설정 방법에 대해 기술합니다. 

<br>

##### Fieldbus 개요

필드버스(Fieldbus)는 공장에서의 센서나 버튼, 모터 드라이버, 조작 인터페이스 등의 장치를 PLC(Programmable Logic Controller) 와 단일 케이블로 연결하여 동작시키기 위해 개방화된 산업표준입니다.

필드버스는 전체 네트워크의 상태를 중앙에서 모니터링 하거나 재구성하는 등의 지능적인 서비스를 제공합니다.

예를 들면 센서나 스위치에 대해, 단순한 On/Off 만이 아닌 상세한 정보, 동작, 모드 설정 등이 가능합니다.

단일 케이블을 사용하여 배선에 드는 시간과 비용을 절감할 수 있고, 구성이 간단해져 유지보수에 유리합니다.

또한 일반적인 통신의 비결정적 응답 (Non-deterministic Response) 특성의 프로토콜과는 달리, 데이터 응답속도가 보장되어 임계시간 특성이 중요한 산업용도를 만족합니다.

![[그림 1.3.7-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/image_1.png>) 

<br>

1개의 필드버스 네트워크에는 1개의 마스터 (Master) 장치와 다수의 슬레이브(Slave) 장치가 연결됩니다.
마스터 장치는 네트워크 전체를 검색 / 관리하고 슬레이브 장치들과 데이터를 교환합니다.

일반적으로 PLC는 마스터 장치이고, 그 외에 센서나 버튼, 제어기등이 슬레이브 장치로 구성될 수 있습니다.
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/1-Specification-DeviceNet-Master.md)
# 1.3.7.1 DeviceNet Master 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>최대 연결 가능한 slave 수</td>
		<td>63개</td>
	</tr>
    <tr>
		<td>최대 입력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 입력 크기 (1 slave)</td>
		<td>255 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기 (1 slave)</td>
		<td>255 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td>Bit Strobe <br>Change of State <br>Cyclic <br>Poll</td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td> - </td>
	</tr>
   <tr>
		<td>통신 속도</td>
		<td>125 ~ 500 Kbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Auto Baudrate Detection</td>
		<td>미지원</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>CAN Frames</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Settings-DeviceNet-Master.md)
# 1.3.7.2 DeviceNet Master 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 및 "[**1.3.2 SYCON.NET 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      SYCON.net 이용 중 매뉴얼에 설명이 부족한 부분은  ""[**1.3.2 SYCON.NET 도움말**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" 기능을 참고해 주십시오.
{% endhint %}

<br>

{% hint style="info" %}
\.      DeviceNet Connector 연결은 아래를 참고해 주십시오.

\.      (“[**1.2.2 커넥터**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)”)
{% endhint %}

<br>

##### 1. PCI 슬롯 설정에서 DeviceNet Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.7.2-1 PCI 슬롯 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

<br>

{% hint style="info" %}
\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

<br>

![[그림 1.3.7.2-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_2.png>) 

<br>

##### 3. Sycon.net 을 이용하여 DeviceNet Master PCI 장치를 선택합니다.

![[그림 1.3.7.2-3 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_3.png>)
![[그림 1.3.7.2-4 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_4.png>) 

<br>

##### 4. PCI 장치를 Scan 하고 DeviceNet Master 적용(Apply)합니다.

![[그림 1.3.7.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_5.png>) 

<br>

##### 5. 통신 속도를 설정합니다.

{% hint style="warning" %}
\.      Master 와 Slave의 통신속도가 다르면 Network Scan이 정상적으로 이루어지지 않습니다.
{% endhint %}

![[그림 1.3.7.2-6 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_6.png>) 

<br>

##### 6. 설정을 다운로드 합니다.

![[그림 1.3.7.2-7 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_7.png>) 

<br>

##### 7. DeviceNet Master 에 연결할 Slave 모듈을 준비합니다.
   * 이번 예제에서는 Crevis 사의 NA-9211 DeviceNet Slave를 사용합니다.
   * 시스템 전원과 필드 전원을 공급해 주어 모듈을 활성화 시켜 주십시오.

![[그림 1.3.7.2-8 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_8.png>) 

<br>

##### 8. Slave 장치의 설정

{% hint style="info" %}
\.      DeviceNet Slave 장치의 MAC ID와 통신속도, 종단저항 설정합니다.
{% endhint %}

![[그림 1.3.7.2-9 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_9.png>) 

![[그림 1.3.7.2-10 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_10.png>)

{% hint style="info" %}
\.      [예제 설정]

\.      종단 저항 : Cable에 종단 저항 장착하여 사용 (종단 DIP Switch OFF)

\.      MAC ID (Station Number) : 4로 설정 (3번 DIP Switch만 ON)

\.      통신 속도 (Baudrate) : Auto 로 설정 (7번, 8번 DIP Switch ON)
{% endhint %}

<br>

##### 9. Slave 장치의 EDS 파일을 등록합니다.

{% hint style="info" %}
\.      Sycon.net에 등록되지 않은 Device를 사용하기 위해 EDS 파일이 필요합니다.

\.      NA-9211 Device의 EDS 파일은 Crevis 홈페이지에서 다운로드 할 수 있습니다.
{% endhint %}

![[그림 1.3.7.2-11 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_11.png>)

{% hint style="info" %}
\.      다운로드한 EDS 파일을 모두 Sycon.net 에 등록합니다.

\.      EDS File 등록시 산업용 통신 Protocol (DeviceNet)를 확인해 주십시오.
{% endhint %}

![[그림 1.3.7.2-12 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_12.png>)

<br>

![[그림 1.3.7.5-13 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_13.png>)



<br>

##### 10. Network Scan

{% hint style="warning" %}
\.      **Network Scan 시 아래 사항을 반드시 확인해 주십시오.**

\.      **(1) 케이블 연결 여부**  
\.      **(2) 종단저항 연결 또는 종단 DIP Switch 사용 여부**  
\.      **(3) Master - Slave 통신 속도 설정 여부**  

\.      **원활한 통신 연결을 위해 (“[**1.3.7.5 DeviceNet ERROR 조치**](../7-DeviceNet/5-Error-DeviceNet.md)”)을 반드시 확인해 주십시오.**
{% endhint %}

{% hint style="info" %}
\.      DeviceNet Master 는 Network Scan 기능을 지원합니다.
{% endhint %}

{% hint style="info" %}
\.      DeviceNet Master 장치에서 우클릭 후 Network Scan을 클릭합니다.
{% endhint %}

![[그림 1.3.7.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      EDS 파일이 등록되지 않은 경우 Network Scan을 하면 Slave 정보는 나타나지만 등록은 불가능합니다.
{% endhint %}

{% hint style="info" %}
\.      정상적으로 EDS 파일이 등록된 경우 Network Scan을 통해 Slave 장치를 추가할 수 있습니다.
{% endhint %}

![[그림 1.3.7.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_15.png>)

![[그림 1.3.7.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_16.png>)

<br>

##### 11. Slave 장치 Configuration

{% hint style="info" %}
\.      Slave 장치 Configuration을 위해 Master 장치의 Disconnect를 클릭합니다.
{% endhint %}

![[그림 1.3.7.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
\.      Slave 장치를 더블클릭합니다.
{% endhint %}

![[그림 1.3.7.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_18.png>)


<br>

{% hint style="info" %}
\.      Slave 장치의 연결 타입을 설정합니다.

\.      DeviceNet 통신을 연결을 위한 메세지 전송 방식을 선택합니다.

\.      ** UCMM 미 체크시 UCMM Group 2 기본 값으로 설정됨**   

\.      UCMM GROUP 1 : IO Message   
\.      UCMM GROUP 2 : Network 초기화 시 Master - Slave 연결 Message (기본 설정)   
\.      UCMM GROUP 3 : Explicit Message   

\.      특정 Device의 경우 UCMM Group 3을 사용할 수 있으니 제품 사양서를 확인 후 진행하십시오.
{% endhint %}

![[그림 1.3.7.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_19.png>)

<br>

{% hint style="info" %}
\.      Crevis NA-9211 은 UCMM 미체크 후 진행합니다. (Group2 기본 값 사용)
{% endhint %}

![[그림 1.3.7.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_20.png>)

<br>


{% hint style="info" %}
\.      DeviceNet Slave의 설정을 확인 합니다.

\.      Output : ST-2318 (1 Byte)  
\.      Input : ST-1218 (1 Byte)  
{% endhint %}

<br>

{% hint style="info" %}
\.      통신 방식 (Poll, Change of State, Cyclic, Bit-Strobe)에 따라 설정 필요  
{% endhint %}

<br>

![[그림 1.3.7.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_21.png>)

<br>

{% hint style="info" %}
\.      [Production Inhibit Time]

\.      슬레이브 장치의 IO 데이터 생성 주기 설정 (ms)  
\.  
\.      예시) 10ms  :  10ms 주기로 IO 데이터를 생성  
\.      예시) 0ms   :  Slave가 가능한 가장 빠른 시간 안에 IO 데이터 생성  

\.      주기가 짧을 수록 Slave 장치에 걸리는 부하가 커질 수 있습니다. (각 Slave 별 사양 확인 필요) 
{% endhint %}

<br>

{% hint style="info" %}
\.      [Expected Packet Rate]

\.      마스터와 슬레이브 간 IO 데이터 업데이트 시간 설정  
{% endhint %}

<br>

![[그림 1.3.7.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_22.png>)



<br>

##### 12. Master 장치 Configuration

{% hint style="info" %}
\.      Master 장치를 더블클릭합니다.
{% endhint %}

![[그림 1.3.7.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      DeviceNet 통신 속도를 설정합니다. (Slave 통신 속도와 동일하도록)
{% endhint %}

![[그림 1.3.7.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.      Address Table에서 각 Slave Slot의 할당된 IO 및 시작 주소를 확인 합니다.
{% endhint %}

![[그림 1.3.7.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      Quick Connect 기능 사용 유무를 설정합니다.
{% endhint %}

![[그림 1.3.7.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_26.png>)


{% hint style="info" %}
\.      설정을 완료 후 Download를 진행해 주십시오.
{% endhint %}

![[그림 1.3.7.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_27.png>)

<br>

##### 13. 통신 상태 확인

{% hint style="info" %}
\.        Sycon.net 과 TP 에서 통신 상태를 확인 합니다.

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      Connected 된 Master 장치를 더블클릭하여 통신 상태를 확인 할 수 있습니다.
{% endhint %}

![[그림 1.3.7.2-28 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_28.png>)

![[그림 1.3.7.2-29 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.        Sycon.net 의 Diagnosis 기능을 이용하여 통신 상태와 함게 IO 입출력 상태를 모니터링 할 수 있습니다.
{% endhint %}

![[그림 1.3.7.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_30.png>)

<br>

##### 14. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/3-Specification-DeviceNet-Slave.md)
# 1.3.7.3 DeviceNet Slave 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>최대 입력 크기</td>
		<td>255 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>255 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td>Bit Strobe <br>Change of State <br>Cyclic <br>Poll</td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td> - </td>
	</tr>
    <tr>
		<td>통신 속도</td>
		<td>125 ~ 500 Kbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Auto Baudrate Detection</td>
		<td>미지원</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>CAN Frames</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Settings-DeviceNet-Slave.md)
# 1.3.7.4 DeviceNet Slave 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      **[DeviceNet Slave EDS File 다운로드]**

\.      “[**5. Slave 장치 설명 파일**](../../../5-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

<br>

{% hint style="info" %}
\.      DeviceNet Connector 연결은 아래를 참고해 주십시오.

\.      (“[**1.2.2 커넥터**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)”)
{% endhint %}

<br>

##### 1. TP를 이용하여 산업용 통신 펌웨어 설정에서 DeviceNet Slave를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.7.4-1 펌웨어 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.

![[그림 1.3.7.4-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

##### 3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬레이브 슬롯 설정 >  DeviceNet Slave]**

![[그림 1.3.7.4-3 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_3.png>) 

![[그림 1.3.7.4-4 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_4.png>) 

<br>

##### 4. 각 항목별 설명

{% hint style="info" %}
\.      [Station Address = Mac ID]

\.      DeviceNet는 Station Address (MAC ID)을 통해 Slave를 식별합니다. (1 ~ 63)
{% endhint %}

{% hint style="info" %}
\.      [통신 속도(Baudrate)]

\.      125, 250, 500 Kbit/s 중 선택 가능합니다.
{% endhint %}

{% hint style="info" %}
\.      [입력 바이트 수 (Input Byte)]

\.      입력 바이트 수 : Master -> Slave 로 입력되는 데이터 크기를 설정합니다.
{% endhint %}

{% hint style="info" %}
\.      [출력 바이트 수 (Output Byte)]

\.      출력 바이트 수 : Slave -> Master 로 출력하는 데이터 크기를 설정합니다.
{% endhint %}


<br>

##### 5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[그림 1.3.7.4-5 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_5.png>) 

<br>

##### 6. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error-DeviceNet.md)
# 1.3.7.5 DeviceNet 에러 조치

<br>

"[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)" 참고해 주십시오.

<br>

##### 1. DeviceNet 종단 저항

{% hint style="info" %}
\.      DeviceNet Cable 연결 시 종단에는 저항을 추가해야합니다.

\.      Network Scan이 안되는 경우 종단 저항을 확인해 주십시오.

\.      DeviceNet 종단 저항 : 120옴
{% endhint %}

{% hint style="info" %}
\.      아래 그림과 같이 CIFX-50 DN PCI가 DeviceNet의 종단인 경우 종단 저항을 추가해 주십시오.
{% endhint %}

![[그림 1.3.7.5-1 DeviceNet 종단 저항]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_1.png>) 

{% hint style="info" %}
\.      아래 그림과 같이 DeviceNet Remote IO 가 종단인 경우 종단 저항을 추가하거나 DIP Switch를 조작해 주십시오.
{% endhint %}

![[그림 1.3.7.5-2 DeviceNet 종단 저항]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_2.png>) 

<br>

##### 2. 통신 속도

{% hint style="info" %}
\.      DeviceNet Master와 Slave 간 통신 속도가 다른 경우 Network Scan이 안될 수 있습니다.

\.      Network Scan이 안되는 경우 통신 속도를 확인해 주십시오.
{% endhint %}

![[그림 1.3.7.5-3 DeviceNet Baudrate]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_3.png>) 

<br>

##### 3. DeviceNet ERROR

{% hint style="info" %}
\.      DeviceNet Cable에 24V 전원 공급이 안되는 경우 아래와 같은 ERROR가 나타납니다.

\.      24V 전원 공급을 확인해 주십시오.
{% endhint %}

![[그림 1.3.7.5-4 DeviceNet Error]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/5-Error/image_4.png>) 
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-DeviceNet-Object.md)
# 1.3.7.6 DeviceNet Object


<br>

##### 1. Object


DeviceNet의 장치 내부에는 Object 의 집합체로 구성이 되어있습니다. 각 Object 는 장치 내부에의 특정한 구성요소를 표현합니다.

<br>

![[그림 1.3.7.6-1 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_1.png>) 


<br>

Object는 Class Code 를 이용하여 구분합니다.

<br>

![[그림 1.3.7.6-2 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_2.png>)

<br>

Object 내부에는 Instance 번호와 Attribute ID로 구성되어 있습니다.

<br>

DeviceNet Master 에서 Explicit Message를 통해 특정 Slave의 Object 에 접근할 수 있습니다.

<br>

{% hint style="info" %}
\.      EX) Crevis GN-9212 의 Object (해당 자료는 Crevis 매뉴얼에서 확인 하실 수 있습니다.)

\.      Identity Object (Class Code 0x01) 의 Vendor ID 값 읽기

\.      Instance : 1

\.      Attribute ID : 1

\.      권한 : Get (읽기만 가능)
{% endhint %}


![[그림 1.3.7.6-3 DeviceNet Object Crevis GN-9212]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_3.png>)


<br>

각 Object 와 내부의 Instance 및 Attribute 마다 모두 각기 다른 접근 권한을 가지고 있습니다.

<br>

{% hint style="info" %}
\.      접근 권한

\.      Get : 읽기 권한

\.      Set : 쓰기 권한 

\.      Attribute Single : 한번에 1개의 Attribute 항목만 접근 가능

\.      Attribute All : 한번에 Instance내의 모든 Attribute 접근 가능
{% endhint %}

<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/README.md)
# 1.3.8 CC-Link

이 장에서는 CC-Link Slave의 특성과 설정 방법에 대해 기술합니다. 


<br>

##### Fieldbus 개요

필드버스(Fieldbus)는 공장에서의 센서나 버튼, 모터 드라이버, 조작 인터페이스 등의 장치를 PLC(Programmable Logic Controller) 와 단일 케이블로 연결하여 동작시키기 위해 개방화된 산업표준입니다.

필드버스는 전체 네트워크의 상태를 중앙에서 모니터링 하거나 재구성하는 등의 지능적인 서비스를 제공합니다.

예를 들면 센서나 스위치에 대해, 단순한 On/Off 만이 아닌 상세한 정보, 동작, 모드 설정 등이 가능합니다.

단일 케이블을 사용하여 배선에 드는 시간과 비용을 절감할 수 있고, 구성이 간단해져 유지보수에 유리합니다.

또한 일반적인 통신의 비결정적 응답 (Non-deterministic Response) 특성의 프로토콜과는 달리, 데이터 응답속도가 보장되어 임계시간 특성이 중요한 산업용도를 만족합니다.

![[그림 1.3.8-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/image_1.png>) 

<br>

1개의 필드버스 네트워크에는 1개의 마스터 (Master) 장치와 다수의 슬레이브(Slave) 장치가 연결됩니다.
마스터 장치는 네트워크 전체를 검색 / 관리하고 슬레이브 장치들과 데이터를 교환합니다.

일반적으로 PLC는 마스터 장치이고, 그 외에 센서나 버튼, 제어기등이 슬레이브 장치로 구성될 수 있습니다.
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md)
# 1.3.8.1 CC-Link Slave 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=3, class='powderblued'>구분</th>
		<th class='powderblued'>사양 (Version 1.11)</th>
		<th class='powderblued'>사양 (Version 2.0)</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td colspan=3>최대 입력 크기</td>
		<td>48 bytes</td>
		<td>368 bytes</td>
	</tr>
    <tr>
		<td colspan=3>최대 출력 크기</td>
		<td>48 bytes</td>
		<td>368 bytes</td>
	</tr>
    <tr>
		<td rowspan=6>입출력 크기</td>
		<td rowspan=2>IO 스테이션</td>
        <td>RY</td>
		<td>4 bytes</td>
		<td>미지원</td>
	</tr>
    <tr>
        <td>RX</td>
		<td>4 bytes</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td rowspan=4>Remote Device</td>
        <td>RY</td>
		<td>16 bytes</td>
		<td>112 Bytes</td>
	</tr>
    <tr>
        <td>RX</td>
		<td>16 bytes</td>
		<td>112 Bytes</td>
	</tr>
    <tr>
        <td>RWw</td>
		<td>32 bytes</td>
		<td>256 Bytes</td>
	</tr>
    <tr>
        <td>RWr</td>
		<td>32 bytes</td>
		<td>256 Bytes</td>
	</tr>
    <tr>
        <td colspan=2, rowspan=2>점유 스테이션</td>
        <td>IO 스테이션</td>
		<td>1</td>
		<td> - </td>
	</tr>
    <tr>
        <td>Remote Device</td>
		<td>1 ~ 4</td>
		<td>1 ~ 4</td>
	</tr>
    <tr>
        <td colspan=3>Extension Cycle</td>
		<td>미지원</td>
		<td>1, 2, 4, 8</td>
	</tr>
   <tr>
		<td colspan=3>통신 속도</td>
		<td colspan=2>156 kbit/s ~ 10 Mbit/s</td>
	</tr>
</tbody>
</table>
<br>


##### CC-Link IO 맵핑

<br>

{% hint style="info" %}
\.        CC-Link Version 1
{% endhint %}

<br>

![[그림 1.3.8.1-1 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Single
{% endhint %}

<br>

![[그림 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Double
{% endhint %}

<br>

![[그림 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Quadruple
{% endhint %}

<br>

![[그림 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Octuple
{% endhint %}

<br>

![[그림 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_5.png>)

<br>
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/2-Settings-CC-Link-Slave.md)
# 1.3.8.2 CC-Link Slave 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      CC-Link Connector 연결은 아래를 참고해 주십시오.

\.      (“[**1.2.2 커넥터**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)”)
{% endhint %}

<br>

##### 1. TP를 이용하여 산업용 통신 펌웨어 설정에서 CC-Link Slave를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.8.4-1 펌웨어 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.

![[그림 1.3.8.4-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

##### 3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬레이브 슬롯 설정 >  CC-Link Slave]**

![[그림 1.3.8.4-3 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>) 

![[그림 1.3.8.4-4 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>) 

<br>

##### 4. 각 항목별 설명

{% hint style="info" %}
\.      [Station Address]

\.      CC-Link는 Station Address를 통해 Slave를 식별합니다. (1 ~ 64)
{% endhint %}

{% hint style="info" %}
\.      [통신 속도(Baudrate)]

\.      156, 625, 2500, 5000, 10000 Kbit/s  중 선택 가능합니다.
{% endhint %}

{% hint style="info" %}
\.      [CC-Link Version]

\.      Version 1 : IO Station 사용 가능, Extension Cycle 사용 불가

\.      Version 2 : IO Station 사용 불가, Extension Cycle 사용 가능
{% endhint %}

{% hint style="info" %}
\.      [점유 Station 수]

\.      IO Station : 1개 점유

\.      Remote Device : 1 ~ 4 개 선택 가능 

\.      점유하는 Station 수에 따라 할당되는 IO Byte 영역의 크기가 달라집니다.
{% endhint %}

{% hint style="info" %}
\.      [Extension Cycle]

\.      Version 2에서 사용 가능

\.      Remote Device : 1배(Single), 2배(Double), 4배(Quadruple), 8배(Octuple) 선택 가능 

\.      Extension Cycle에 따라 할당되는 IO Byte 영역의 크기가 달라집니다.
{% endhint %}

<br>

{% hint style="info" %}
\.      **IO Byte 영역에 대해서는 아래 링크를 참고해 주십시오.**

\.      **(“[**1.3.8.1 CC-Link Slave 사양**](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md)”)**
{% endhint %}

<br>

##### 5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

<br>

##### 6. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Error-CC-Link.md)
# 1.3.8.3 CC-Link Slave 에러 조치

<br>

"[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)" 참고해 주십시오.

<br>

##### 1. CC-Link 종단 저항

{% hint style="info" %}
\.      CC-Link Cable 연결 시 종단에는 저항을 추가해야합니다.

\.      통신 연결이 안되는 경우 종단 저항을 확인해 주십시오.

\.      CC-Link 종단 저항 : 110옴
{% endhint %}

{% hint style="info" %}
\.      아래 그림과 같이 CIFX-50 CC PCI가 CC-Link의 종단인 경우 종단 저항을 추가해 주십시오.
{% endhint %}

![[그림 1.3.8.5-1 CC-Link 종단 저항]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/5-Error/image_1.png>) 



##### 2. CC-Link ERROR

{% hint style="info" %}
\.      통신 연결을 위해 CC-Link Cable에 24V 전원 공급이 필요합니다.

\.      통신 연결이 안되는 경우 24V 전원 공급을 확인해 주십시오.
{% endhint %}

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/README.md)
# 1.3.9 CC-Link IE Field

이 장에서는 CC-Link IE Field Slave의 특성과 설정 방법에 대해 기술합니다. 


<br>

##### Fieldbus 개요

필드버스(Fieldbus)는 공장에서의 센서나 버튼, 모터 드라이버, 조작 인터페이스 등의 장치를 PLC(Programmable Logic Controller) 와 단일 케이블로 연결하여 동작시키기 위해 개방화된 산업표준입니다.

필드버스는 전체 네트워크의 상태를 중앙에서 모니터링 하거나 재구성하는 등의 지능적인 서비스를 제공합니다.

예를 들면 센서나 스위치에 대해, 단순한 On/Off 만이 아닌 상세한 정보, 동작, 모드 설정 등이 가능합니다.

단일 케이블을 사용하여 배선에 드는 시간과 비용을 절감할 수 있고, 구성이 간단해져 유지보수에 유리합니다.

또한 일반적인 통신의 비결정적 응답 (Non-deterministic Response) 특성의 프로토콜과는 달리, 데이터 응답속도가 보장되어 임계시간 특성이 중요한 산업용도를 만족합니다.

![[그림 1.3.9-1 Fieldbus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/image_1.png>) 

<br>

1개의 필드버스 네트워크에는 1개의 마스터 (Master) 장치와 다수의 슬레이브(Slave) 장치가 연결됩니다.
마스터 장치는 네트워크 전체를 검색 / 관리하고 슬레이브 장치들과 데이터를 교환합니다.

일반적으로 PLC는 마스터 장치이고, 그 외에 센서나 버튼, 제어기등이 슬레이브 장치로 구성될 수 있습니다.

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/1-Specification-CC-Link-IE-Field-Slave.md)
# 1.3.9.1 CC-Link IE Field Slave 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=2, class='powderblued'>구분</th>
		<th colspan=2, class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td colspan=2>Network Number</td>
		<td colspan=2>1~239</td>
	</tr>
    <tr>
		<td colspan=2>Station Number</td>
		<td colspan=2>1~120</td>
	</tr>
    <tr>
		<td colspan=2>통신 속도</td>
		<td colspan=2>1Gbps</td>
	</tr>
    <tr>
		<td colspan=2>Device Type</td>
		<td>Intelligent Device Station</td>
        <td>Remote Device Station</td>
	</tr>
    <tr>
		<td rowspan=4>IO Size</td>
        <td>RY data</td>
		<td>4 ~ 256 bytes (32 ~ 2048 bits)</td>
        <td>4 ~ 16 bytes (32 ~ 128 bits)</td>
	</tr>
    <tr>
        <td>RX data</td>
		<td>0 ~ 256 bytes (0 ~ 2048 bits)</td>
        <td>0 ~ 16 bytes (0 ~ 128 bits)</td>
	</tr>
    <tr>
        <td>RWw data</td>
		<td>0 ~ 1024 words</td>
        <td>0 ~ 64 words</td>
	</tr>
    <tr>
        <td>RWr data</td>
		<td>0 ~ 1024 words</td>
        <td>0 ~ 64 words</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>1000 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>Constantly On</td>
	</tr>
    <tr>
		<td>Auto-Crossover</td>
		<td>Constantly On</td>
	</tr>
</tbody>
</table>
<br>

##### 물리적 연결

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>케이블</td>
		<td>최소 Cat6 이상, STP 케이블</td>
	</tr>
	<tr>
		<td>길이</td>
		<td>Max. 100m</td>
	</tr>
	<tr>
		<td>결선</td>
		<td>8선 전체 결선</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/2-Settings-CC-Link-IE-Field-Slave.md)
# 1.3.9.2 CC-Link IE Field Slave 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.


<br>

##### 1. TP를 이용하여 산업용 통신 펌웨어 설정에서 CC-Link IE Field Slave를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.9.2-1 펌웨어 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.

![[그림 1.3.9.4-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

##### 3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬레이브 슬롯 설정 >  CC-Link IE Field Slave]**

![[그림 1.3.9.4-3 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>) 

![[그림 1.3.9.4-4 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>) 

<br>

##### 4. 각 항목별 설명

{% hint style="info" %}
\.      [Network Number]

\.      CC-Link IE Field network 번호 (1~239)
{% endhint %}

{% hint style="info" %}
\.      [Station Address]

\.      연결된 network 내에 장치 ID (1 ~ 120)
{% endhint %}

{% hint style="info" %}
\.      [IO Type]

\.      IO Type은 master 장치 설정에 의해 결정됨   
\.      - Mixed: 입력과 출력이 다른 인덱스 사용 (서로 다른 주소)   
\.      - Input: 입력 전용   
\.      - Output: 출력 전용   
\.      - FrontBackMixture: 입력과 출력이 같은 인덱스 사용 (동일한 주소)   
{% endhint %}

{% hint style="info" %}
\.      [Device Type]

\.      Device Type에 따라 설정 가능한 IO 최대 크기가 상이합니다.

\.      Intelligent Device Station   
\.      - RY, RX (max): 256 bytes   
\.      - RWw, RWr (max): 1024 words

\.      Remote Device Station   
\.      - RY, RX (max): 16 bytes   
\.      - RWw, RWr (max): 64 words
{% endhint %}

{% hint style="info" %}
\.      [IO Size]

\.      Master -> Slave   
\.      - RWw (word data)   
\.      - RY (bit data)   

\.      Slave -> Master   
\.      - RWr (word data)   
\.      - RX (bit data)  
{% endhint %}

<br>

##### 5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

<br>

##### 6. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}

<br>

![[그림 1.3.9.4-5 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>) 
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/3-Error-CC-Link-IE-Field.md)
# 1.3.9.3 CC-Link IE Field Slave 에러 조치

<br>

"[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)" 참고해 주십시오.

[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/README.md)
# 1.3.10 EtherNet/IP - 표준 Remote IO 연결

<br>

이 장에서는 EtherNet/IP Scanner (Master)를 이용하여 당사에서 선정한 몇가지의 표준 Remote IO Module을 연결하는 방법에 대해 설명합니다.

<br>

{% hint style="info" %}
\.      EtherNet/IP Scanner(Master) 는 CIFX-50 Real Time Ethernet PCI 를 사용합니다.


\.      Remote IO Module은 Crevis 사의 M9289 EtherNet/IP Network Adapter를 사용합니다.
{% endhint %}


[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)
# 1.3.10.1 EtherNet/IP - 표준 Remote IO 연결 설정

“[**1.3.1 CIFX PCI 슬롯 설정**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

##### 1. 산업용 통신 펌웨어 설정에서 EtherNet/IP Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 1.3.10.1-1 펌웨어 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

![[그림 1.3.10.1-2 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

##### 3. 통신을 위해 PCI와 Remote IO의 Cable 등을 연결하고 상태를 확인합니다.

![[그림 1.3.10.1-3 하드웨어 연결]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[그림 1.3.10.1-4 하드웨어 연결]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

<br>

{% hint style="info" %}
\.      PCI 와 Remote IO를 LAN Cable을 이용하여 연결해 주십시오.

\.      Remote IO 의 DIP Switch는 모두 OFF로 설정해 주십시오.

\.      Remote IO 전원과 Field Power를 모두 연결해 주십시오. (24V DC)
{% endhint %}

<br>

{% hint style="info" %}
\.      Remote IO Crevis M9289 의 공장 출하시 설정 IP는 192.168.100.99 입니다.

\.      Remote IO 의 IP가 192.168.100.99 로 설정되어 있어야 통신 연결이 가능합니다.

\.      “[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

##### 4. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: PCI 슬레이브 슬롯 설정 >  EtherNet/IP Remote IO Setting]**

![[그림 1.3.10.1-5 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>) 

![[그림 1.3.10.1-6 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>) 

<br>

{% hint style="info" %}
\.      IP는 고정값으로 설정되어 있습니다.

\.      Input, Output Byte 수를 확인합니다.

\.      선택한 Input, Output 수가 Remote IO Slot에 장착된 카드의 IO 수 보다 작거나 같아야 합니다.
{% endhint %}

<br>

{% hint style="info" %}
\.      Input Module  
\.      M12DF : Digital 16점  
\.      M3534 : Analog 4점  
{% endhint %}

{% hint style="info" %}
\.      Output Module  
\.      M225F : Digital 16점  
\.      M226F : Digital 16점  
\.      M2768 : Digital 8점   
\.      M4534 : Analog 4점  
{% endhint %}

{% hint style="info" %}
\.      Special Module  
\.      M5112 : Conveyer I/F 
{% endhint %}

<br>

##### 5. 설정 완료 후 제어기를 재부팅합니다.

![[그림 1.3.10.1-7 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>) 

![[그림 1.3.10.1-8 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
\.      설정 완료 후 제어기를 재부팅해 주십시오.
{% endhint %}

<br>

##### 6. 설정값이 반영되어있는지 확인 후, 통신 상태를 확인합니다.

![[그림 1.3.10.1-9 슬레이브 설정]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>) 

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**1.4 CIFX PCI 통신 모니터링**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[그림 1.3.10.1-10 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>) 

{% hint style="info" %}
\.      통신 연결이 안되는 경우 Remote IO의 IP를 확인해야합니다.

\.      아래를 따라 확인해 주십시오. (192.168.100.99 가 아닌 경우)

\.      “[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

![[그림 1.3.10.1-11 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>) 

![[그림 1.3.10.1-12 산업용 통신 모니터링]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>) 

<br>

##### 7. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)
# 1.3.10.2 Remote IO IP 주소 설정

Crevis M9289 EtherNet/IP Network Adpater 의 IP 주소 설정 방법입니다.

<br>

{% hint style="info" %}
\.      Remote IO Crevis M9289 의 공장 출하시 설정 IP는 192.168.100.99 입니다.

\.      Remote IO 의 IP를 알지 못하거나 변경이 필요한 경우 아래를 따라 주십시오.
{% endhint %}

<br>

##### 1. PC와 Remote IO를 LAN Cable을 이용해 직접 연결합니다.

![[그림 1.3.10.2-1 LAN 연결]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

##### 2. Remote IO Adapter의 9번 DIP Switch만 ON으로 변경합니다.

![[그림 1.3.10.2-2 DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

##### 3. Bootpsvr.exe 프로그램을 실행합니다.
   * 해당 프로그램은 Crevis 사에서 제공합니다. (홈페이지에서 IO Guide Pro 다운로드 후 설치)

![[그림 1.3.10.2-3 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[그림 1.3.10.2-4 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
\.      Start BootP를 누른 상태에서 M9289 모듈의 전원을 분리하고 다시 인가하여 재부팅합니다.
{% endhint %}

![[그림 1.3.10.2-5 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>


##### 4. Adapter 장치를 재부팅하면 BootpSvr.exe 프로그램에 Device 정보가 나타납니다.

![[그림 1.3.10.2-6 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

##### 5. Device를 선택하여 IP를 설정합니다.

![[그림 1.3.10.2-7 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[그림 1.3.10.2-8 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

##### 6. IP 설정이 끝난 Adapter의 DIP Switch를 모두 OFF로 변경한 후 장치를 재부팅합니다.

{% hint style="info" %}
\.      DIP Switch의 상태 Adapter 재부팅 여부를 반드시 확인해 주십시오.
{% endhint %}

![[그림 1.3.10.2-9 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

##### 7. PC 에서 Ping Test 등을 이용하여 IP를 확인합니다.

![[그림 1.3.10.2-10 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

##### 8. IP 주소가 정상적으로 변경이 되었다면 설정을 진행합니다.

{% hint style="info" %}
\.      "[**1.3.10.1 EtherNet/IP - 표준 Remote IO 연결 설정**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)" 절차를 따라 설정을 진행해 주십시오.
{% endhint %}

[__SOURCE](1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)
# 1.4 CIFX PCI 통신 모니터링

<br>

“[**1.2 CIFX PCI 통신 카드 장착 및 설정**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)” 및 “[**1.3  CIFX PCI 통신 설정**](../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)” 절차를 따라 통신 설정 이후 동작여부를 다음과 같은 화면에서 확인 가능합니다.

<br>

#### 1. 산업용 통신 모니터링

<br>

**\[서비스 > 19: 산업용 통신 모니터링]** 을 터치하여 들어갈 수 있으며, 해당 화면에서 설정한 펌웨어 정보, 통신 상태, 통신 구성 상태 등을 확인 가능합니다.

<br>

{% hint style="info" %}
\.      **\[재시작]** 버튼을 이용하여 해당 PCI 통신 카드의 산업용 통신을 재시작 시킬 수 있습니다.

\.      슬롯, 펌웨어, 장치 상태를 확인해 주십시오.

\.      Master의 경우 슬레이브 구성 및 활성 슬레이가 구성한 슬레이브 수와 동일한지 확인해 주십시오.
{% endhint %}

<br>

![[그림 1.4-1 산업용 통신 모니터터링]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_1.png>)

<br>

{% hint style="info" %}
\.      [상태 정보]   
\.       통신 상태 (Communication) : 통신 연결 및 IO 교환 중   
\.       동작 (Run) : 통신 카드 동작 중   
\.       준비 (Ready) : 통신 준비 상태   
\.       에러 (Error) : 통신 에러 상태   

\.       통신 에러 (Communication Error) : 통신 중 발생한 에러 코드   
\.       에러 횟수 (Error Count) : 에러 발생 누적 횟수   
\.       활성 슬레이브 (Active Slaves) : 통신 연결 및 IO 교환 중인 슬레이브 수   
\.       슬레이브 구성 (Configured Slaves) : 통신 연결 설정한 슬레이브 수   
\.       진단 슬레이브 (Diag Slave) : 통신 진단 중인 슬레이브 수   
\.       Watchdog time (ms) : 통신 프로그램 동작 감지 기능 Timeout 시간   
{% endhint %}

<br>

#### 2. 산업용 통신 노드 모니터링

<br> 

#### 지원 버전 미정

<br>

모니터링 화면 하단의 노드 상태(Node Status) 버튼을 클릭하여 마스터 프로토콜에 연결된 장치의 상태를 모니터링 합니다.

<br>

![[그림 1.4-2 산업용 통신 모니터터링]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_2.png>)

{% hint style="info" %}
\.      [노드 상태 정보]   
\.       초록색 : 통신 연결 및 IO 교환 중인 노드   
\.       빨간색 : 통신 설정은 했으나 연결 안된 노드   
{% endhint %}

<br>

{% hint style="info" %}
\.      DeviceNet Master의 경우 노드 정보 리스트를 스캔하여 모니터링 할 수 있습니다.
{% endhint %}

<br>

![[그림 1.4-3 산업용 통신 모니터터링]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_3.png>)
[__SOURCE](1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)
# 1.4.1 ERROR Code

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>

<br>

<table class="tg">
<thead>
	<tr>
		<th>Error Code</th>
		<th>Description</th>
		<th>Action</th>
	</tr>
</thead>

<tbody>
	<tr>
		<td>0x00000000</td>
		<td>정상</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xC000000C</td>
		<td>제어기와 PCI 사이의 Watchdog 시간 초과</td>
		<td>제어기와 장치의 상태를 확인해 주십시오. 통신 재시작을 통해 리셋할 수 있습니다.</td>
	</tr>
    <tr>
		<td>0xC0000123</td>
		<td>라이선스 없음</td>
		<td>마스터 라이선스의 유무를 확인하십시오</td>
	</tr>
    <tr>
		<td>0xC0000140</td>
		<td>통신 오류</td>
		<td>장치의 상태나 연결 여부를 확인해 주십시오.</td>
	</tr>
    <tr>
		<td>0xC0000141</td>
		<td>연결 끊김</td>
		<td>장치의 상태나 연결 여부를 확인해 주십시오.</td>
	</tr>
    <tr>
		<td>0xC0000142</td>
		<td>연결 대기 시간 초과</td>
		<td>장치의 상태나 연결 여부를 확인해 주십시오..</td>
	</tr>
    <tr>
		<td>0xC0000144</td>
		<td>중복된 IP 주소</td>
		<td>연결된 장치의 IP 주소를 확인하여 중복된 주소를 변경해 주십시오.</td>
	</tr>
    <tr>
		<td>0xC0000145</td>
		<td>케이블 연결 안됨</td>
		<td>통신 케이블의 연결 상태를 확인해 주십시오.</td>
	</tr>
    <tr>
		<td>0xC0000180</td>
		<td>통신 버스 Off 플래그 설정됨 <br> [발생 가능 원인] <br>  - 통신선 CAN High/Low 의 단락 감지 <br>  - 전원 전압 불안정 <br>  - 노이즈 등으로 인한 네트워크 에러 지속 발생</td>
		<td>통신 케이블 접촉 상태나 결선을 확인하고, 장치를 리셋해 주십시오.</td>
	</tr>
    <tr>
		<td>0xC0470298</td>
		<td>DeviceNet 24V 공급 안됨</td>
		<td>DeviceNet 24V 전원을 확인해 주십시오.</td>
	</tr>
	<tr>
		<td>0xC0620023</td>
		<td>DeviceNet Slave bus off 감지 <br> [발생 가능 원인] <br>  - 통신선 CAN High/Low 의 단락 감지 <br>  - 전원 전압 불안정 <br>  - 노이즈 등으로 인한 네트워크 에러 지속 발생</td>
		<td>통신 케이블 접촉 상태나 결선을 확인하고, 장치를 리셋해 주십시오. </td>
	</tr>
    <tr>
		<td>0xC062002C</td>
		<td>DeviceNet Slave 24V 공급 안됨</td>
		<td>DeviceNet 24V 전원을 확인해 주십시오.</td>
	</tr>
</tbody>
</table>


[__SOURCE](2-ethernet-ip/README.md)
# 2. EtherNet/IP

이 장에서는 내장형 EtherNet/IP Master(Scanner) 와 Slave(Adapter)의 특성과 설정 방법에 대해 기술합니다. 

<br>

##### EtherNet/IP 개요

EthetNet/IP 는 CI(ControlNet International)와 ODVA(Open DeviceNet Vendors Association)에 의해 개발된 이더넷 기반의 개방형 산업용 통신 프로토콜입니다.

공장에서 센서, 리모트 IO, 모터 드라이버, HMI, PLC, 로봇 제어기 등 다양한 장치가 제조사와 무관하게 하나의 EtherNet/IP 네트워크에 연결될 수 있습니다.

![[그림 2-1 EtherNet/IP]](<../_assets//2-ethernet-ip/image_1.png>)
 

<br>

EtherNet/IP 는 통신 기능에 따라 아래와 같이 구분합니다.

##### Scanner Class
   * 기존 필드버스 마스터(Master)에 해당되는 제품들로 EtherNet/IP Adapter 또는 Scanner 에게 I/O 데이터 연결을 요청할 수 있습니다.

<br>

##### Adapter Class
  * 기존 필드버스 슬레이브(Slave)에 해당되는 제품들로 EtherNet/IP Scanner 에 의해 요청되는 Real-Time I/O 데이터의 연결 타겟(Target)에 해당됩니다.
    
  * Adapter는 Scanner 에 의하지 않고서는 스스로 Real-Time I/O 데이터를 송수신 할 수 없습니다.

<br>

##### Messaging Class
   * 모든 Class 의 제품의 대해 Explicit 메세지 송수신이 가능한 제품들로 Real-Time I/O 데이터 송수신은 지원하지 않습니다.
   
   * 예를 들면 프로그램 업로드 / 다운로드용 컴퓨터 인터페이스 카드, 네트워크 설정 Tool 등이 해당 될 수 있습니다.


### 용어
|약어|설명|
|---------------|------------------------------|
|어댑터(Adapter)|EtherNet/IP 스캐너(Scanner)로 부터 Output Data를 수집하고 Input Data를 송신하는 장치|
|스캐너(Scanner)|말단 장치(EtherNet/IP 어댑터)로 Output Data를 보내고 그들로부터 Input Data를 수집하는 장치|
|LAN| Local Area Network|
|RPI|Requested Packet Interval(통신 주기)|
|PLC|Programmable logic controller|
|T2O|Target to Originator(어댑터 -> 스캐너)|
|O2T|Originator to Target(스캐너 -> 어댑터)|

[__SOURCE](2-ethernet-ip/1-network.md)
## 2.1 네트워크 설정

### 1. 제어기 메인 모듈
EtherNet/IP 통신을 사용할 수 있는 LAN Port는 LAN1/ LAN2/ LAN3 입니다.<br>

![그림 2.1-1 Main Module](../_assets/2-ethernet-ip/1-network/hi6com.png)<br>

### 2. 네트워크 설정
EtherNet/IP 통신을 연결할 LAN Port를 선택한 뒤 아래와 같이 TP화면을 통해 해당 LAN Port의 설정을 확인하고 필요에 따라 설정을 변경해야 합니다.<br>

![그림 2.1-2 Network configuration](../_assets/2-ethernet-ip/1-network/networkConfig.png)<br>

{% hint style="info" %}
\.      LAN1/LAN2/LAN3 각각의 IP주소는 서브넷 부분을 다르게 설정해야 합니다.

\.      설정을 변경한 후에는 로봇제어기를 재부팅 하십시오.
{% endhint %}

<br>

### 3. 연결 상태의 확인
랜 포트의 Link/Act Led로 물리적 연결 상태를 확인할 수 있습니다.<br>

LAN선을 연결 한 뒤 LED의 상태를 확인합니다. 좌측의 LED가 점등 또는 점멸하지 않는다면 케이블이나 어댑터 또는 스캐너 장치에 이상이 있다는 것을 의미합니다. 케이블이나 장치의 연결상태를 확인하십시오.<br>

![l그림 2.1-3 LAN Port](../_assets/2-ethernet-ip/1-network/lanPort.png)<br>


### 4. 네트워크 구성
EtherNet/IP Network와 Factory Network는 서로 분리된 네트워크로 구성하는 것이 좋습니다. 아래 그림과 같이 하나의 Network로 EtherNet/IP Network와 Factory Network를 구성하게 되면 하나의 전송 매체를 공유하게 되므로 네트워크 부하를 증가시키게 됩니다. 따라서 가능하면 EtherNet/IP Network는 별도로 구성한 네트워크를 사용하시는 것을 추천 드립니다.<br>

![그림 2.1-4 Network](../_assets/2-ethernet-ip/1-network/NG_Network.png)<br>

![그림 2.1-5 Network](../_assets/2-ethernet-ip/1-network/Good_Network.png)<br>

[__SOURCE](2-ethernet-ip/2-license.md)
## 2.2 라이선스 설정

### 1. 라이선스의 활성화
초기화면에서 “시스템” > “2 : 제어 파라미터” > “10: 옵션기능의 라이선스키 등록” 으로 이동<br>
![그림 2.2-1 license](../_assets/2-ethernet-ip/2-license/license.png)<br>
*[그림 2.5.1-1 라이선스 활성]*<br>

1. 라이선스 리스트 중 “EtherNet/IP 어댑터를 “유효”로 선택
2. 시스템 일련번호를 라이선스 관리자에게 전달
3. 관리자로부터 라이선스키를 얻어 입력 후 “확인”버튼을 누름
4. License Key [XXXXXX] ==>OK 확인
5. Ethernet/IP 어댑터 메뉴 진입시 라이런스 없다는 경고 메시지가 사라진 것을 확인<br>
~ 참고<br>
![그림 2.2-2 license](../_assets/2-ethernet-ip/2-license/license_ng.png)<br>
*[그림 2.5.1-2 라이선스 활성화 안될시 나오는 메시지]*<br>



[__SOURCE](2-ethernet-ip/3-adapter/README.md)
# 2.3 EtherNet/IP 어댑터 (슬레이브)

내장형 EtherNet/IP 어댑터 (슬레이브) 에 대한 설명입니다.<br>


[__SOURCE](2-ethernet-ip/3-adapter/1-specification.md)
## 2.3.1 EtherNet/IP 어댑터 사양 (슬레이브)


<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th colspan=2, class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
    <tr>
        <td>Connection</td>
        <td>O (Master) -> T (Slave)</td>
		<td>T (Slave) -> O (Master)</td>
	</tr>
    <tr>
        <td>최대 IO Size</td>
        <td>240 bytes</td>
		<td>240 bytes</td>
	</tr>
    <tr>
        <td>Instance No.</td>
        <td>112 (0x70)</td>
		<td>100 (0x64)</td>
	</tr>
    <tr>
        <td>Real-Time Transfer Format</td>
        <td>32-bit run/idle header</td>
		<td>None</td>
	</tr>
	<tr>
        <td>Connection Type</td>
        <td>Point to Point</td>
		<td>Point to Point</td>
	</tr>
	<tr>
        <td>Priority</td>
        <td>Scheduled</td>
		<td>Scheduled</td>
	</tr>
    <tr>
		<td>IO 최소 Cycle Time (RPI)</td>
		<td colspan=2>5ms</td>
	</tr>
    <tr>
		<td>장치 타입</td>
		<td colspan=2>General Purpose Discrete I/O</td>
	</tr>
    <tr>
		<td>통신 속도</td>
		<td colspan=2>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td colspan=2>미지원</td>
	</tr>
    <tr>
		<td >IP 할당 방식</td>
		<td colspan=2>고정 IP 주소</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>10 or 100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>사용 가능</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>사용 가능</td>
	</tr>
</tbody>
</table>
<br>

##### 물리적 연결

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>케이블</td>
		<td>최소 Cat5 이상, STP 케이블</td>
	</tr>
	<tr>
		<td>길이</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](2-ethernet-ip/3-adapter/2-settings.md)
## 2.3.2 EtherNet/IP 어댑터 (슬레이브) 설정

### 1. 티칭팬던트를 통한 EtherNet/IP 어댑터의 설정 및 모니터링
초기화면에서 “SYSTEM” > “Control Parameter” > “Industrial Communication” > ”Ethernet/IP 어댑터” 로 이동<br>
![Config.PNG](../../_assets/2-ethernet-ip/3-adapter/Config.png)<br>
*[그림 2.3.1 설정]*<br>

**[Network]**
-	기능사용 : Ethernet/IP 어댑터의 사용여부 선택
-	이더넷 포트 선택 : Ethernet/IP Scanner와 연결할 LAN Port 선택 (선택된 LAN Port의 정보는 바로 아래 줄에 표시 됨)<br>

**[I/O Size]**
-	입력 바이트 수 : 0 ~ 240 설정 가능
-	출력 바이트 수 : 0 ~ 240 설정 가능<br>

**[Monitoring]**
- 동작(Run) : Ethernet/IP의 I/O Data 교환의 상태를 나타냄 (On : 정상 통신 중 , Off : 통신 중 아님)
- 준비(Ready) : Ethernet/IP 어댑터의 초기화 상태를 나타냄 (On : 초기화 정상, Off : 초기화 비정상)
- 에러(Error) : Ethernet/IP 어댑터의 알람 또는 경고 상태 표시 (On : 알람/경고 상태, Off : 정상)
- 버전 : Ethernet/IP 어댑터 S/W 버전 정보 표시
- 에러코드: 알람 또는 경고가 발생했을 경우 알람/경고 코드 표시 

[__SOURCE](2-ethernet-ip/3-adapter/3-connect-scanner/README.md)
## 2.3.3 외부 Scanner 장치 연결

이 장에서는 EtherNet/IP 어댑터와의 외부 스캐너 장치 연결 방법을 설명합니다.  <br>
[__SOURCE](2-ethernet-ip/3-adapter/3-connect-scanner/1-connect-ls-plc.md)
### 2.3.3.1 LS ELECTRIC PLC와의 연결

LS ELECTRIC PLC와 EtherNet/IP와의 연결 방법을 설명합니다.  
아래에서 사용되는 PLC와 통신모듈은 다음과 같습니다.  
(PLC : XGI-CPUS, 통신모듈 : XGL-EFMTB)

#### 1. XG5000 실행
![xg5000.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/xg5000.png) <br>
*[그림 2.6.1.1 XG5000의 실행]*<br>
XG5000 프로그램의 다운로드 및 자세한 사용방법은 LS ELECTRIC 홈페이지를 참고 하십시오.

#### 2. EDS File의 등록
메뉴 > 도구 > EDS(D) > EDS파일 등록 클릭 > “Hi6_EIP_240402.eds” 선택<br>
아래 그림과 같이 EDS 파일 등록 확인<br>
![eds.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/eds.png)<br>
*[그림 2.6.1.2 EDS File의 등록]*<br>


#### 3. 장치 연결
[1] 프로젝트 생성<br>
![newProject_1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_1.png)<br>
*[그림 2.6.1.3 새프로젝트 생성]*<br>

[2] 통신 모듈 추가<br>
![newProject_2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_2.png)<br>
*[그림 2.6.1.4 통신 모듈 추가1]*<br>

![newProject_3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_3.png)<br>
*[그림 2.6.1.5 통신 모듈 추가2]*<br>

![newProject_4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_4.png)<br>
*[그림 2.6.1.6 통신 모듈 추가3]*<br>

[3] 통신 모듈의 설정 <br>
아래 그림에서 좌측 탭에 보이는 XGL-EFMT를 더블 클릭<br>
![newProject_6.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_6.png)<br>
*[그림 2.6.1.7 통신 모듈 설정]*<br>
- IP주소, 서브넷마스크, 게이트웨이 등을 설정합니다.  
- PLC의 2개의 LAN Port를 릴레이 기능으로 사용하려면 "Relay" 체크 박스를 선택해 줍니다.  
- RAPIEnet설정은 Disable로 변경합니다.

#### 4. 온라인 접속 설정
[1] USB 케이블로 PLC와 연결합니다.<br>
![newProject_7.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_7.png)<br>
*[그림 2.6.1.8 온라인 접속 설정1]*<br>

[2] 아래 그림 좌측에 표시된 버튼을 눌러 전체 설정을 다운로드 합니다.<br>
![newProject_8.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_8.png)<br>
*[그림 2.6.1.9 온라인 접속 설정2]*<br>

#### 5. 오토 스캔
[1] 오토 스캔은 PLC와 연결된 상태에서 가능합니다.<br>
현재 온라인 상태가 아니라면 메뉴 > 온라인 > 접속 을 클릭하여 온라인 상태로 변경합니다.<br>

[2] XGL-EFMT 에서 마우스 우측클릭 > 항목 추가 > 스마트 증설 클릭<br>
![auto1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto1.png)<br>
*[그림 2.6.1.10 오토 스캔1]*<br>

[3] Next 클릭  <br>
![auto2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto2.png)<br>
*[그림 2.6.1.11 오토 스캔2]*<br>

[4] 오토 스캔 클릭  <br>
![auto3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto3.png)<br>
*[그림 2.6.1.12 오토 스캔3]*<br>

![auto4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto4.png)<br>
*[그림 2.6.1.13 오토 스캔4]*<br>

[5] 자동 스캔된 장치 확인  
![auto5.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto5.png)<br>
*[그림 2.6.1.14 오토 스캔5]*<br>

![auto6.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto6.png)<br>
*[그림 2.6.1.15 오토 스캔6]*<br>

아래 그림과 같이 Hi6 EtherNet/IP 어댑터 장치가 리스트에 나타납니다.  <br>
![auto7.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto7.png)<br>
*[그림 2.6.1.16 오토 스캔7]*<br>

#### 6. 프로그램 변수 등록
[1] 스캔프로그램 > NewProgram > 로컬변수(더블클릭)<br>
![variable1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/variable1.png)<br>
*[그림 2.6.1.17 변수 등록1]*<br>

[2] 통신에서 사용할 Input/Output Data를 설정합니다.<br>
![variable2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/variable2.png)<br>
*[그림 2.6.1.18 변수 등록2]*<br>

#### 7. EtherNet/IP Adapter 설정
[1] 좌측 리스트에서 EB01(Hi6 EtherNet/IP 어댑터)를 더블 클릭 합니다.<br>

[2] EIP 상세 설정 버튼을 누릅니다.<br>
![AdapterSetting1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting1.png)<br>
*[그림 2.6.1.19 EtherNet/IP Adapter 설정1]*<br>

[3] 아래 그림을 참고하여 EtherNet/IP 어댑터의 설정값을 선택해 줍니다. <br> 
- 접속 형태
- T2O RPI Range, O2T RPI Range
- T2O Input, O2T Output size
- 송신 주기
- 타임 아웃
- 로컬태크, 리모트태그 <br>
![AdapterSetting2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting2.png) <br>
*[그림 2.6.1.20 EtherNet/IP Adapter 설정2]*<br>

[4] 온라인 > 통신 모듈 설정 및 진단 > 서비스 인에블 클릭<br>
![AdapterSetting3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting3.png)<br>
*[그림 2.6.1.21 EtherNet/IP Adapter 설정3]*<br>

[5] FEnet의 I/O서비스 체크 확인<br>
![AdapterSetting4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting4.png)<br>
*[그림 2.6.1.22 EtherNet/IP Adapter 설정4]*<br>

<br>

##### 8. 통신 설정 완료 후 IO Block 을 할당

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**5. 산업용 통신 IO Block 할당**](../../../5-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](2-ethernet-ip/3-adapter/4-error_code.md)
## 2.3.4 EtherNet/IP 어댑터 (슬레이브) 알람코드

|코드|메시지|
|------|---|
|W23101|EtherNet/IP 초기화 실패|
|W23102|EtherNet/IP 통신 타임아웃 발생|
|W23103|EIP 어댑터 CPF O2T 초기화 실패|
|W23104|EIP 어댑터 CPF T2O 초기화 실패|
|W23105|EIP 어댑터 IO MSG O2T 초기화 실패|
|W23106|EIP 어댑터 IO MSG T2O 초기화 실패|
|W23107|EIP 어댑터 PIT 초기화 실패|
|W23108|EIP 어댑터 Socket 통신 초기화 실패|
|W23109|EIP 어댑터 Socket 통신 (UDP 0) 초기화 실패|
|W23110|EIP 어댑터 Socket 통신 (UDP 1) 초기화 실패|
|W23111|EIP 어댑터 Socket 통신 (UDP 2) 초기화 실패|
|W23112|EIP 어댑터 Socket 통신 (UDP 3) 초기화 실패|
|W23113|EIP 어댑터 Socket 통신 (TCP 0) 초기화 실패|
|W23114|EIP 어댑터 Socket 통신 (TCP 1) 초기화 실패|
|W23115|EIP 어댑터 Socket 통신 (TCP 2) 초기화 실패|
|W23116|EIP 어댑터 Socket 통신 (TCP 3) 초기화 실패|
|W23117|EIP 어댑터 내부 통신1(IO Write) 문제|
|W23118|EIP 어댑터 내부 통신1(IO Read) 문제|
|W23119|EIP 어댑터 내부 통신1(Status Write) 문제|
|W23120|EIP 어댑터 내부 통신1(Config Read) 문제|
|W23150|EIP 어댑터 내부 통신2(IO Read) 문제|
|W23151|EIP 어댑터 내부 통신2(IO Write) 문제|
|W23152|EIP 어댑터 내부 통신2(Status Read) 문제|
|W23153|EIP 어댑터 내부 통신2(Config Write) 문제|




[__SOURCE](2-ethernet-ip/4-scanner/README.md)
# 2.4 EtherNet/IP 스캐너 (마스터)

<br>

#### 지원 버전 미정

<br>

내장형 EtherNet/IP 스캐너 (마스터) 에 대한 설명입니다.<br>

[__SOURCE](2-ethernet-ip/4-scanner/1-specification.md)
## 2.4.1 EtherNet/IP 스캐너 (마스터) 사양

<br>

#### 지원 버전 미정

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=2, class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td colspan=2>최대 연결 가능한 slave 수</td>
		<td>20개</td>
	</tr>
    <tr>
		<td rowspan=2>IO Size</td>
        <td>전체 입출력</td>
		<td>Max 1200 bytes</td>
	</tr>
    <tr>
        <td>Slave 장치당 입출력</td>
		<td>Max 240 bytes</td>
	</tr>
    <tr>
		<td colspan=2>IO 연결</td>
		<td>Cyclic</td>
	</tr>
    <tr>
		<td colspan=2>IO 최소 Cycle Time</td>
		<td>5ms</td>
	</tr>
    <tr>
		<td colspan=2>통신 속도</td>
		<td>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td colspan=2>Quick Connect</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td colspan=2>Topology</td>
		<td>Tree, Line</td>
	</tr>
    <tr>
		<td colspan=2>IP 할당 방식</td>
		<td>고정 IP 주소</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>10 or 100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>사용 가능</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>사용 가능</td>
	</tr>
</tbody>
</table>
<br>

##### 물리적 연결

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>케이블</td>
		<td>최소 Cat5 이상, STP 케이블</td>
	</tr>
	<tr>
		<td>길이</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](2-ethernet-ip/4-scanner/2-settings.md)
## 2.4.2 EtherNet/IP 스캐너 (마스터) 설정

<br>

#### 지원 버전 미정

<br>

“[**2.1 네트워크 설정**](../../2-ethernet-ip/1-network.md)" 및 "[**2.2 라이선스 설정**](../../2-ethernet-ip/2-license.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

##### 1. 메뉴를 터치하여 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 3: EtherNet/IP 설정]**

<br>

![[그림 2.4.2-1 스캐너 설정]](<../../_assets/2-ethernet-ip/4-scanner/img_1.png>) 

<br>

![[그림 2.4.2-2 스캐너 설정]](<../../_assets/2-ethernet-ip/4-scanner/img_2.png>) 

<br>

{% hint style="info" %}
\.      [Protocol 설정]

\.      * OFF : EtherNet/IP 사용 안함   
\.      * Adapter : EtherNet/IP Adapter 모드   
\.      * Scanner : EtherNet/IP Scanner 모드   
\.      * Adapter + Scanner : EtherNet/IP Adapter + Scanner 동시 사용 모드    (같은 LAN Port)
{% endhint %}

{% hint style="info" %}
\.      [Port 설정]

\.      * 제어기 범용 LAN1 ~ 3 사용 가능 (상태 OK 확인 필요)
{% endhint %}

<br>

##### 2. Scanner 모드를 선택하고 "장치 추가(Add Device)" 버튼을 눌러 다음 화면으로 진입합니다.

<br>

![[그림 2.4.2-3 스캐너 장치 추가]](<../../_assets/2-ethernet-ip/4-scanner/img_3.png>) 

<br>

##### 3. 연결할 장치와 동일하게 설정을 입력하고 저장합니다.

<br>

{% hint style="info" %}
\.      [장치 설정]

\.      * Device No. : 장치 연결 순서 (IO 데이터 배치 순서)   
\.      * IP Address : 장치의 IP 주소   
\.      * Device Name : 장치 이름 (통신 연결과는 무관, 단순 식별용)   
\.      * RPI (ms) : IO 데이터 갱신 주기   
\.      * Connection Type   
\.          - Exclusive Owner (I/O) : Scanner - Adapter 입출력 연결   
\.          - Input Only : Adapter의 입력 신호만 연결   
\.          - Listen Only : Adapter 가 다른 Scanner와 I/O 연결 되어있는 상태에서 입력 신호만 연결   

\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      * Run/Idle Header : IO 데이터 헤더 유무 선택   
\.      * Instance No. : IO 데이터 교환을 위한 Input / Output Assembly의 Instance 번호   
\.      * IO Size : IO 데이터 크기 (bytes 단위)   
{% endhint %}

<br>

{% hint style="info" %}
\.      연결 예시는 아래 매뉴얼을 참고해주십시오.    
\.      “[**2.3.3.1 외부 Adapter 장치 연결 - Crevis Remote IO**](3-connect-adapter/1-crevis.md)"

\.      “[**2.3.3.2 외부 Adapter 장치 연결 - Wago Remote IO**](3-connect-adapter/2-wago.md)"

\.      “[**2.3.3.3 외부 Adapter 장치 연결 - Hilscher CIFX PCI EtherNet/IP Adapter**](3-connect-adapter/3-pci.md)"

\.      “[**2.3.3.4 외부 Adapter 장치 연결 - Baumer OM-70**](3-connect-adapter/4-baumer.md)"  
{% endhint %}

<br>

![[그림 2.4.2-4 스캐너 장치 추가]](<../../_assets/2-ethernet-ip/4-scanner/img_4.png>) 

<br>

##### 4. OK 버튼을 눌러 통신 설정을 전송합니다.

<br>

![[그림 2.4.2-5 스캐너 설정]](<../../_assets/2-ethernet-ip/4-scanner/img_5.png>) 

<br>

##### 5. 통신이 정상적으로 연결되었는지 상태를 확인합니다.

<br>

![[그림 2.4.2-6 통신 상태 모니터링]](<../../_assets/2-ethernet-ip/4-scanner/img_6.png>) 

<br>

{% hint style="info" %}
\.      [통신 상태 확인]   
\.       - License: 현재 라이선스 상태   
\.       - Run: EtherNet/IP 기능 동작 상태 표시   
\.       - Communication: EtherNet/IP 통신 연결 상태 표시   
\.       - Error: EtherNet/IP 오류 상태 표시   

\.      장치 번호 색상   
\.       - 초록색 : 통신 연결 OK   
\.       - 빨간색 : 통신 연결 NG   
{% endhint %}

<br>

![[그림 2.4.2-7 통신 상태 모니터링]](<../../_assets/2-ethernet-ip/4-scanner/img_7.png>) 

<br>

##### 6. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../../5-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/README.md)
## 2.4.3 외부 Adapter 장치 연결

<br>

#### 지원 버전 미정

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### 외부 Adapter 장치 연결 시 설정 값

<br>

{% hint style="info" %}
\.      IO size는 외부 장치에 연결된 Input / Output 크기와 일치하게 설정해 주십시오.   
{% endhint %}

<br>

{% hint style="info" %}
\.      자세한 사양은 장치 Maker에서 제공하는 매뉴얼을 참고해주십시오.    
{% endhint %}

<br>

<table class="tg">
<thead>
	<tr>
    	<th rowspan=2, class='powderblued'>Maker</th>
		<th rowspan=2, class='powderblued'>제품</th>
		<th rowspan=2, class='powderblued'>연결 방식</th>
        <th colspan=2, class='powderblued'>T -> O</th>
        <th colspan=2, class='powderblued'>O -> T</th>
        <th colspan=5, class='powderblued'>Additional Configuration</th>
	</tr>
    <tr>
        <th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Run Idle Header</th>
        <th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Run Idle Header</th>
		<th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Total Size</th>
		<th class='powderblued'>Data Size</th>
        <th class='powderblued'>Data Type</th>
		<th class='powderblued'>Data</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Crevis</td>
		<td>M9289</td>
        <td>Exclusive Owner</td>
		<td>1</td>
		<td>No</td>
        <td>2</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Wago</td>
		<td>750-366</td>
        <td>Exclusive Owner</td>
		<td>104: Status + AI + DI<br>105: Status + DI<br>106: Status + AI<br>107: AI + DI<br>108: DI<br>109: AI</td>
		<td>No</td>
        <td>101: AO + DO<br>102: DO<br>103: AO</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Hilscher</td>
		<td>CIFX PCI EtherNet/IP Adapter</td>
        <td>Exclusive Owner</td>
		<td>101</td>
		<td>Yes</td>
        <td>100</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Baumer</td>
		<td>OM-70 EtherNet/IP</td>
        <td>Input Only</td>
		<td>100</td>
		<td>No</td>
        <td>238</td>
		<td>-</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Beckhoff</td>
		<td>EK-9500</td>
        <td>Exclusive Owner</td>
		<td>129</td>
		<td>No</td>
        <td>130</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
	<tr>
		<td rowspan=6>Rockwell Automation (AB)</td>
		<td rowspan=6>Point I/O 1734-AENTR</td>
        <td rowspan=6>Exclusive Owner</td>
		<td rowspan=6>101</td>
		<td rowspan=6>No</td>
        <td rowspan=6>100</td>
		<td rowspan=6>Yes</td>
		<td rowspan=6>102</td>
		<td rowspan=6>10</td>
		<td>4byte</td>
		<td>unsigned int</td>
		<td>1</td>
	</tr>
	<tr>
		<td>2byte</td>
		<td>unsigned int</td>
		<td>IO slot + 1</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(T -> O) Alignment<br>0: bytes<br>2: word<br>4: Dword<br>255: Fixed</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(T -> O) Fixed Size per Slot</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(O -> T) Alignment<br>0: bytes<br>2: word<br>4: Dword<br>255: Fixed</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(O -> T) Fixed Size per Slot</td>
	</tr>
</tbody>
</table>
<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis.md)
## 2.4.3.1 외부 Adapter 장치 연결 - Crevis Remote IO

<br>

#### 지원 버전 미정

<br>

{% hint style="info" %}
\.      EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

\.      “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
\.      예시의 Remote IO의 IP 설정은 아래 매뉴얼 링크를 참조하여 진행해 주십시오.

\.      “[**1.3.10.2 Remote IO IP Setting**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

##### 1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.

![[그림 2.4.3.1-1 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_1.png>) 

<br>

![[그림 2.4.3.1-2 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_2.png>) 

<br>

![[그림 2.4.3.1-3 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_3.png>) 

<br>

##### 2. EZ-EDS 프로그램으로 EDS 파일을 열어 장치 정보를 확인합니다.

<br>

![[그림 2.4.3.1-4 EDS 파일 정보]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_4.png>) 

<br>

{% hint style="info" %}
\.      Connection Manager에서 연결 타입 확인   
\.      * 예시에서는 Exclusive Owner

\.      Real Time Transfer Format에서 헤더 여부 확인   
\.      * Input (T > O) : 헤더 없음   
\.      * Output (O > T) : 32-bit run/idle header   

\.      Create / Decode path 를 눌러 Instance ID 확인   
{% endhint %}

<br>

![[그림 2.4.3.1-5 EDS 파일 정보]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_5.png>) 

<br>

{% hint style="info" %}
\.      * Input (T > O) : 1   
\.      * Output (O > T) : 2   
{% endhint %}

<br>

##### 3. 장치 매뉴얼에서 IO size를 확인합니다.

<br>

{% hint style="info" %}
\.      현재 연결할 장치의 IO 구성 확인 
{% endhint %}

<br>

![[그림 2.4.3.1-6 Remote IO 구성]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_6.png>) 

<br>

{% hint style="info" %}
\.      슬롯 구성별 매뉴얼을 참고하여 IO size 확인
{% endhint %}

<br>

![[그림 2.4.3.1-7 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_7.png>) 

<br>

![[그림 2.4.3.1-8 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_8.png>) 

<br>

##### 4. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.

<br>

![[그림 2.4.3.1-8 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_9.png>)

<br>

{% hint style="info" %}
\.      연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      [Adapter 구성]   
\.      Crevis M9289   
\.      - M7002 : None   
\.      - M2768 : 1byte (O > T)   
\.      - M2768 : 1byte (O > T)   
\.      - M12DF : 2bytes (T > O)   
\.      - M12DF : 2bytes (T > O)   
\.      - M2768 : 1byte (O > T)   
\.      - M2768 : 1byte (O > T)   

\.      [IO Assembly 정보]   
\.      [T > O]   
\.      - Size: 4bytes   
\.      - Instance: 1   
\.      - Run/Idle Header: No   

\.      [O > T]    
\.      - Size: 4bytes   
\.      - Instance: 2   
\.      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/2-wago.md)
## 2.4.3.2 외부 Adapter 장치 연결 - Wago Remote IO

<br>

#### 지원 버전 미정

<br>

{% hint style="info" %}
\.      EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

\.      “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
\.      해당 장치의 IP 설정은 Wago 매뉴얼을 참조하여 진행해 주십시오.
{% endhint %}

<br>

##### 1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.

![[그림 2.4.3.2-1 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_1.png>) 

<br>

##### 2. 장치 매뉴얼에서 Instance ID를 확인합니다.

<br>

![[그림 2.4.3.2-2 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_2.png>) 

<br>

{% hint style="info" %}
\.      Input (T > O)   
\.      * 104: Status  + Analog  + Digital   
\.      * 105: Status  + Digital   
\.      * 106: Status  + Analog   
\.      * 107: Analog  + Digital   
\.      * 108: Digital   
\.      * 109: Analog   

\.      Output (O > T)   
\.      * 101: Analog + Digital   
\.      * 102: Digital   
\.      * 103: Analog   
{% endhint %}

<br>

##### 2. EZ-EDS 프로그램으로 EDS 파일을 열어 장치 정보를 확인합니다.

<br>

![[그림 2.4.3.2-3 EDS 파일 정보]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_3.png>) 

<br>

{% hint style="info" %}
\.      Connection Manager에서 연결 타입 확인   
\.      * 예시에서는 Exclusive Owner

\.      Real Time Transfer Format에서 헤더 여부 확인   
\.      * Input (T > O) : 헤더 없음   
\.      * Output (O > T) : 32-bit run/idle header   
{% endhint %}

<br>

##### 3. 장치 매뉴얼에서 IO size를 확인합니다.

<br>

{% hint style="info" %}
\.      현재 연결할 장치의 IO 구성 확인 
{% endhint %}

<br>

![[그림 2.4.3.2-4 Remote IO 구성]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_4.png>) 

<br>

{% hint style="info" %}
\.      슬롯 구성별 매뉴얼을 참고하여 IO size 확인
{% endhint %}

<br>

![[그림 2.4.3.2-5 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_5.png>) 

<br>

![[그림 2.4.3.2-6 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_6.png>) 

<br>

##### 4. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.

<br>

![[그림 2.4.3.2-7 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_7.png>)

<br>

{% hint style="info" %}
\.      연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      [Adapter 구성]   
\.      Wago 750-366   
\.      - Status 1byte (T > O) (Instance ID 104, 105, 106 선택시)   
\.      - 753-436 : 1byte (T > O)   
\.      - 753-536 : 1byte (O > T)   

\.      [IO Assembly 정보]   
\.      [T > O]   
\.      - Size: 2bytes   
\.      - Instance: 105   
\.      - Run/Idle Header: No   

\.      [O > T]    
\.      - Size: 1bytes   
\.      - Instance: 101   
\.      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/3-pci.md)
## 2.4.3.3 외부 Adapter 장치 연결 - Hilscher CIFX PCI EtherNet/IP Adapter

<br>

#### 지원 버전 미정

<br>

{% hint style="info" %}
\.      EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

\.      “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
\.      해당 장치의 IP 설정은 Hilscher 매뉴얼을 참조하여 진행해 주십시오.
{% endhint %}

<br>

##### 1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.

![[그림 2.4.3.3-1 CIFX PCI]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_1.png>) 

<br>

##### 2. EZ-EDS 프로그램으로 EDS 파일을 열어 장치 정보를 확인합니다.

<br>

![[그림 2.4.3.3-2 EDS 파일 정보]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_2.png>) 

<br>

{% hint style="info" %}
\.      Connection Manager에서 연결 타입 확인   
\.      * 예시에서는 Exclusive Owner

\.      Real Time Transfer Format에서 헤더 여부 확인   
\.      * Input (T > O) : 32-bit run/idle header   
\.      * Output (O > T) : 32-bit run/idle header   
{% endhint %}

<br>

![[그림 2.4.3.3-3 EDS 파일 정보]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_3.png>) 

<br>

{% hint style="info" %}
\.      Param에서 Instance ID 확인   
\.      * Input (T > O) : 101   
\.      * Output (O > T) : 100   
{% endhint %}

<br>

##### 3. 장치에 설정된 IO size를 확인합니다.

<br>

{% hint style="info" %}
\.      현재 연결할 장치의 IO Size 확인 (해당 PCI 장치 설정 참조)   
{% endhint %}

<br>

##### 4. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.

<br>

![[그림 2.4.3.3-4 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_4.png>)

<br>

{% hint style="info" %}
\.      연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      [IO Assembly 정보]   
\.      [T > O]   
\.      - Size: 240 bytes (PCI 장치에 설정된 값)   
\.      - Instance: 101   
\.      - Run/Idle Header: 32Bit   

\.      [O > T]    
\.      - Size: 240 bytes (PCI 장치에 설정된 값)   
\.      - Instance: 100   
\.      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer.md)
## 2.4.3.4 외부 Adapter 장치 연결 - Baumer OM-70

<br>

#### 지원 버전 미정

<br>

{% hint style="info" %}
\.      EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

\.      “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
\.      해당 장치의 IP 설정은 Baumer 매뉴얼을 참조하여 진행해 주십시오.
{% endhint %}

<br>

##### 1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.

![[그림 2.4.3.4-1 Baumer OM-70]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_1.png>) 

<br>

##### 2. 장치 매뉴얼에서 Instance ID 및 IO Size를 확인합니다.

<br>

![[그림 2.4.3.4-2 Baumer OM-70]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_2.png>) 

<br>

{% hint style="info" %}
\.      [Input Only Connection]   

\.      Input (T > O)   
\.      * Instance ID: 100   
\.      * Size : 34 bytes   

\.      Output (O > T)   
\.      * Instance ID: 238   
\.      * Size : 0 byte    
{% endhint %}

<br>

##### 3. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.

<br>

![[그림 2.4.3.4-3 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_3.png>)

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff.md)
## 2.4.3.5 외부 Adapter 장치 연결 - Beckhoff Remote IO

<br>

#### 지원 버전 미정

<br>

{% hint style="info" %}
\.      EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

\.      “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
\.      해당 장치의 IP 설정은 Beckhoff 매뉴얼을 참조하여 진행해 주십시오.
{% endhint %}

<br>

##### 1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.

![[그림 2.4.3.5-1 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_1.png>) 

<br>

##### 2. 장치 웹페이지에 접속하여 IP 주소를 설정합니다.

<br>

{% hint style="info" %}
\.      예시에서 초기 IP 설정은 192.168.1.2 로 되어있습니다. (DIP 스위치 2번 ON)
{% endhint %}

<br>

![[그림 2.4.3.5-2 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_2.png>) 

<br>

![[그림 2.4.3.5-3 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_3.png>) 

<br>

{% hint style="info" %}
\.      예시에서는 IP를 192.168.10.95로 설정합니다. 

\.      IP 주소 입력 후 체크 버튼을 눌러 저장합니다. 
{% endhint %}

<br>

![[그림 2.4.3.5-4 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_4.png>) 

<br>

{% hint style="info" %}
\.      DIP 스위치를 아래와 같이 설정한 후 장치를 재부팅합니다.   
\.      * 1 ~ 8번  : ON   
\.      * 9 ~ 10번 : OFF   
{% endhint %}

<br>

![[그림 2.4.3.5-5 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_5.png>) 

<br>

![[그림 2.4.3.5-6 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_6.png>) 

<br>

##### 3. 장치 웹페이지에 접속하여 EtherNet/IP 설정 정보를 확인합니다.

<br>

{% hint style="info" %}
\.      설정한 IP 주소로 다시 접속하여 IP 주소 및 EtherNet/IP 구성 정보를 확인합니다.
{% endhint %}

<br>

![[그림 2.4.3.5-7 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_7.png>) 

<br>

![[그림 2.4.3.5-8 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_8.png>) 

<br>

{% hint style="info" %}
\.      Input (T > O)   
\.      * Instance ID: 129   
\.      * Byte Size: 6      

\.      Output (O > T)   
\.      * Instance ID: 130   
\.      * Byte Size: 6   
{% endhint %}

<br>

##### 4. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.

<br>

![[그림 2.4.3.5-9 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_9.png>)

<br>

{% hint style="info" %}
\.      연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      [Adapter 구성]   
\.      Beckhoff EK-9500   
\.      - EK-1008 : 1byte (T > O)   
\.      - EK-2008 : 1byte (O > T)   

\.      [IO Assembly 정보]   
\.      [T > O]   
\.      - Size: 6bytes   
\.      - Instance: 129   
\.      - Run/Idle Header: No   

\.      [O > T]    
\.      - Size: 6bytes   
\.      - Instance: 130   
\.      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell.md)
## 2.4.3.6 외부 Adapter 장치 연결 - Rockwell Automation (AB) Remote IO

<br>

#### 지원 버전 미정

<br>

{% hint style="info" %}
\.      EZ-EDS 프로그램을 통해 EtherNet/IP Adapter 장치의 설정 정보를 쉽게 확인할 수 있습니다.

\.      “[**EDS 파일 도구 (EZ-EDS) 다운로드**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
\.      해당 장치의 IP 설정은 Rockwell Automation (AB) Point I/O 1734-AENTR 매뉴얼을 참조하여 진행해 주십시오.
{% endhint %}

<br>

##### 1. Adapter 장치의 매뉴얼과 EDS 파일을 준비합니다.

<br>

![[그림 2.4.3.6-1 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_1.png>) 

<br>

![[그림 2.4.3.6-2 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_2.png>) 

<br>

##### 2. EZ-EDS 프로그램으로 EDS 파일을 열어 장치 정보를 확인합니다.

<br>

![[그림 2.4.3.6-3 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_3.png>) 

<br>

![[그림 2.4.3.6-4 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_4.png>) 

<br>

{% hint style="info" %}
\.      Connection Manager에서 연결 타입 확인   
\.      * 예시에서는 Exclusive Owner

\.      Real Time Transfer Format에서 헤더 여부 확인   
\.      * Input (T > O) : 헤더 없음   
\.      * Output (O > T) : 32-bit run/idle header   

\.      Create / Decode path 를 눌러 Instance ID 확인   
\.      * Input (T > O) : 101   
\.      * Output (O > T) : 100   
\.      * Configuration : 102   
{% endhint %}

<br>

##### 3. 장치 매뉴얼에서 IO size를 확인합니다.

<br>

{% hint style="info" %}
\.      현재 연결할 장치의 IO 구성 확인 
{% endhint %}

<br>

![[그림 2.4.3.6-5 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_5.png>) 

<br>

{% hint style="info" %}
\.      슬롯 구성별 매뉴얼을 참고하여 IO size 확인
{% endhint %}

<br>

![[그림 2.4.3.6-6 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_6.png>) 

<br>

![[그림 2.4.3.6-7 Remote IO 연결]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_7.png>) 

<br>

##### 4. Adapter 장치 정보에 따라 통신 설정값을 입력합니다.

<br>

![[그림 2.4.3.6-8 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_8.png>)

<br>

{% hint style="info" %}
\.      연결할 장치의 매뉴얼을 확인하여 설정값을 올바르게 입력해 주십시오.   
\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      [Adapter 구성]   
\.      Point I/O 1734-AENTR    
\.      - 상태 값 : 8byte (T > O)    
\.      - 1734-IB8 : 1byte (T > O)   
\.      - 1734-OB8E : 1byte (O > T) + 1byte (T > O, 상태 값)   

\.      [IO Assembly 정보]   
\.      [T > O]   
\.      - Size: 10bytes   
\.      - Instance: 101   
\.      - Run/Idle Header: No   

\.      [O > T]    
\.      - Size: 1byte   
\.      - Instance: 100   
\.      - Run/Idle Header: 32Bit   
{% endhint %}

<br>

![[그림 2.4.3.6-9 EtherNet/IP Adapter 설정]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_9.png>)

<br>

{% hint style="info" %}
\.      연결할 장치의 매뉴얼을 확인하여 부가 설정값을 올바르게 입력해 주십시오.   
\.      * Input (T > O) : Slave > Master 연결   
\.      * Output (O > T) : Master > Slave 연결   

\.      [부가 설정 값]   
\.      - Config Segment : ON   
\.      - Instance: 102   
\.      - Size: 10bytes    

\.      [Config Segment 정보]    
\.      - (4bytes) 1 : 헤더    
\.      - (2bytes) 3 : 연결된 슬롯 + 1   
\.      - (1byte)  0 : T > O Alignment (byte 단위)      
\.      - (1byte)  1 : T > O 슬롯별 데이터 크기      
\.      - (1byte)  0 : O > T Alignment (byte 단위)      
\.      - (1byte)  1 : O > T 슬롯별 데이터 크기      
{% endhint %}

<br>
[__SOURCE](2-ethernet-ip/4-scanner/4-error.md)
## 2.4.4 EtherNet/IP 스캐너 (마스터) 에러 코드

<br>

#### 지원 버전 미정

<br>

{% hint style="info" %}
\.      각 장치별 통신 상태를 CIP 표준 General Status 코드로 표시하여 실시간 진단 기능을 제공합니다.
{% endhint %}

<br>

![[그림 2.4.4-1 스캐너 설정]](<../../_assets/2-ethernet-ip/4-scanner/img_8.png>) 

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### General Status Codes

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>상태 값 (16진수)</th>
		<th class='powderblued'>명칭</th>
		<th class='powderblued'>설명</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>-</td>
		<td>통신 설정 안됨 또는 변경됨</td>
		<td>통신 설정이 반영되지 않았거나 변경 중</td>
	</tr>
	<tr>
		<td>0x00</td>
		<td>Success</td>
		<td>서비스가 성공적으로 수행됨</td>
	</tr>
	<tr>
		<td>0x00 (에러 상태인 경우)</td>
		<td>No reponse</td>
		<td>통신 응답 없음 (케이블 연결 안됨, 유효하지 않은 IP 주소 등)</td>
	</tr>
	<tr>
		<td>0x01</td>
		<td>Connection failed</td>
		<td>연결 시도 실패 (설정 값 또는 경로 문제)</td>
	</tr>
	<tr>
		<td>0x02</td>
		<td>Resource unavailable</td>
		<td>장치 자원 부족 (연결 개수 초과 등)</td>
	</tr>
	<tr>
		<td>0x03</td>
		<td>Invalid parameter value</td>
		<td>파라미터 값 오류 (주로 데이터 크기 불일치)</td>
	</tr>
	<tr>
		<td>0x04</td>
		<td>Path segment error</td>
		<td>경로 세그먼트 오류 (Class, Instance 등 식별 불가)</td>
	</tr>
	<tr>
		<td>0x05</td>
		<td>Path destination unknown</td>
		<td>대상 객체(Object)를 찾을 수 없음</td>
	</tr>
	<tr>
		<td>0x06</td>
		<td>Partial transfer</td>
		<td>데이터의 일부만 전송됨</td>
	</tr>
	<tr>
		<td>0x07</td>
		<td>Connection lost</td>
		<td>통신 중 연결이 끊어짐 (Timeout 등)</td>
	</tr>
	<tr>
		<td>0x08</td>
		<td>Service not supported</td>
		<td>객체가 요청한 서비스(Get/Set 등)를 지원 안 함</td>
	</tr>
	<tr>
		<td>0x09</td>
		<td>Invalid attribute value</td>
		<td>설정하려는 속성값이 유효 범위를 벗어남</td>
	</tr>
	<tr>
		<td>0x0A</td>
		<td>Attribute list error</td>
		<td>속성 리스트 서비스 수행 중 오류 발생</td>
	</tr>
	<tr>
		<td>0x0B</td>
		<td>Already in requested state</td>
		<td>객체가 이미 요청한 상태에 있음</td>
	</tr>
	<tr>
		<td>0x0C</td>
		<td>Object state conflict</td>
		<td>객체의 현재 상태에서 허용되지 않는 서비스 요청</td>
	</tr>
	<tr>
		<td>0x0D</td>
		<td>Object already exists</td>
		<td>이미 존재하는 객체를 생성하려고 시도함</td>
	</tr>
	<tr>
		<td>0x0E</td>
		<td>Attribute not settable</td>
		<td>쓰기가 불가능한(Read-only) 속성에 쓰기 시도</td>
	</tr>
	<tr>
		<td>0x0F</td>
		<td>Privilege violation</td>
		<td>권한 부족 (보안이나 접근 레벨 문제)</td>
	</tr>
	<tr>
		<td>0x10</td>
		<td>Device state conflict</td>
		<td>장치의 현재 모드 또는 상태에서 요청된 서비스 실행 할 수 없음</td>
	</tr>
	<tr>
		<td>0x11</td>
		<td>Reply data too large</td>
		<td>응답 데이터가 할당된 버퍼보다 커서 전송 실패</td>
	</tr>
	<tr>
		<td>0x12</td>
		<td>Fragmentation of primitive value</td>
		<td>데이터 분할 전송 중 오류</td>
	</tr>
	<tr>
		<td>0x13</td>
		<td>Not enough data</td>
		<td>요청을 수행하기에 데이터 양이 부족함</td>
	</tr>
	<tr>
		<td>0x14</td>
		<td>Attribute not supported</td>
		<td>요청한 속성(Attribute) 번호가 존재하지 않음</td>
	</tr>
	<tr>
		<td>0x15</td>
		<td>Too much data</td>
		<td>요청에 포함된 데이터가 너무 많음</td>
	</tr>
	<tr>
		<td>0x16</td>
		<td>Object does not exist</td>
		<td>대상 객체가 존재 하지 않음</td>
	</tr>
	<tr>
		<td>0x17</td>
		<td>Service fragmentation sequence erroruccess</td>
		<td>서비스 분할 전송 순서가 잘못됨</td>
	</tr>
	<tr>
		<td>0x18</td>
		<td>No stored attribute data</td>
		<td>저장된 속성 데이터가 없음</td>
	</tr>
	<tr>
		<td>0x19</td>
		<td>Store operation failure</td>
		<td>데이터 저장 작업 실패</td>
	</tr>
	<tr>
		<td>0x1A</td>
		<td>Routing failure, request packet too large</td>
		<td>요청 데이터의 용량이 제한치를 초과하여 라우팅 서비스 중단</td>
	</tr>
	<tr>
		<td>0x1B</td>
		<td>Routing failure, response packet too large</td>
		<td>응답 데이터의 용량이 제한치를 초과하여 라우팅 서비스 중단</td>
	</tr>
	<tr>
		<td>0x1C</td>
		<td>Missing attribute list entry data</td>
		<td>요청된 동작을 수행하는데 필요한 속성이 누락됨</td>
	</tr>
	<tr>
		<td>0x1D</td>
		<td>Invalid attribute value list</td>
		<td>유효하지 않은 속성들에 대한 상태 정보 반환</td>
	</tr>
	<tr>
		<td>0x1E</td>
		<td>Embedded service error</td>
		<td>장치 내장 서비스 오류</td>
	</tr>
	<tr>
		<td>0x1F</td>
		<td>Vendor specific error</td>
		<td>장치 제조사가 직접 정의한 에러</td>
	</tr>
	<tr>
		<td>0x20</td>
		<td>Invalid parameter</td>
		<td>요청된 파라미터가 CIP 규격 또는 정의된 규격과 맞지 않음</td>
	</tr>
	<tr>
		<td>0x21</td>
		<td>Write-once value already written</td>
		<td>한 번만 쓰기 가능한 값을 이미 썼음</td>
	</tr>
	<tr>
		<td>0x22</td>
		<td>Invalid reply received</td>
		<td>잘못된 응답이 수신됨</td>
	</tr>
	<tr>
		<td>0x23</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0x24</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0x25</td>
		<td>Key failure in path</td>
		<td>경로 내 키(Key) 일치 확인 실패</td>
	</tr>
	<tr>
		<td>0x26</td>
		<td>Path size invalid</td>
		<td>경로 데이터 크기가 유효하지 않음</td>
	</tr>
	<tr>
		<td>0x27</td>
		<td>Unexpected attribute in list</td>
		<td>현재 상태에서 설정할 수 없는 항목 설정 시도</td>
	</tr>
	<tr>
		<td>0x28</td>
		<td>Invalid member ID</td>
		<td>지정된 클래스 / 인스턴스 또는 속성에 해당 항목이 존재하지 않음</td>
	</tr>
	<tr>
		<td>0x29</td>
		<td>Member cannot be set</td>
		<td>수정할 수 없는 항목 수정 요청</td>
	</tr>
	<tr>
		<td>0x2A</td>
		<td>Group 2 only server general failure</td>
		<td>DeviceNet Error (EtherNet/IP 에서 미사용)</td>
	</tr>
	<tr>
		<td>0x2B - 0xCF</td>
		<td>Reserved</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xD0 - 0xFF</td>
		<td>Vendor specific Codes</td>
		<td>장치 제조사가 직접 정의한 에러</td>
	</tr>
</tbody>
</table>
<br>

[__SOURCE](3-ethercat-master-io/README.md)
# 3. EtherCAT Master IO

<br>

이 장에서는 EtherCAT Master 를 이용하여 당사에서 선정한 몇가지의 표준 Remote IO Module을 연결하는 방법에 대해 설명합니다.

<br>

##### EtherCAT 개요

EtherCAT은 Beckhoff Automation 에서 개발된 이더넷 기반의 Fieldbus 시스템입니다.

EtherCAT 프로토콜은 매우빠른 IO Data 업데이트와 정확한 동기화를 위한 기능을 제공합니다. 

<br>

##### EtherCAT Master IO
   * 기존 필드버스 마스터(Master)에 해당되는 제품으로 EtherCAT 슬레이브(Slave) 장치들에게 IO 데이터 연결을 요청할 수 있습니다.

<br>

{% hint style="info" %}
\.      EtherCAT Master 는 제어기의 범용 LAN Port 를 사용합니다.


\.      Remote IO Module은 Crevis 사의 M9386 EtherCAT Network Adapter를 사용합니다.
{% endhint %}



[__SOURCE](3-ethercat-master-io/1-Settings-EtherCAT-Master.md)
# 3.1 EtherCAT Master IO 설정

<br>

##### 1. 메뉴를 터치하여 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 4: EtherCAT Master 설정]**

<br>

![[그림 3.1-1 EtherCAT Master 설정]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_1.png>) 

<br>

{% hint style="info" %}
\.      EtherCAT Master 설정 화면에서 선택된 제어기 LAN Port 번호를 확인합니다. 
{% endhint %}

##### 2. 통신을 위해 제어기 LAN 포트와 Remote IO의 Cable 등을 연결하고 상태를 확인합니다.

<br>

![[그림 3.1-2 하드웨어 연결]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_2.png>) 
![[그림 3.1-3 하드웨어 연결]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_3.png>) 

<br>

{% hint style="info" %}
\.      제어기 와 Remote IO를 LAN Cable을 이용하여 연결해 주십시오.

\.      Remote IO 의 DIP Switch는 모두 OFF로 설정해 주십시오.

\.      Remote IO 전원과 Field Power를 모두 연결해 주십시오. (24V DC)
{% endhint %}

<br>

##### 3. 설정 메뉴에서 EtherCAT Master 사용을 "ON" 으로 선택합니다. 

<br>

![[그림 3.1-4 EtherCAT Master 설정]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_4.png>) 

<br>

{% hint style="info" %}
\.      사용하는 환경에 맞게 통신 주기를 설정합니다.

\.      통신 주기는 1ms, 2ms, 5ms 를 지원합니다.
{% endhint %}

<br>

##### 4. 설정 메뉴의 슬레이브 리스트에서 연결한 Remote IO 모듈과 동일한 구성을 선택합니다. 

<br>

![[그림 3.1-5 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_5.png>)

<br>

{% hint style="info" %}
\.      Input, Output Byte 수를 확인합니다.
{% endhint %}

<br>

{% hint style="info" %}
\.      Input Module  
\.      M12DF : Digital 16점  
\.      M3534 : Analog 4점  
{% endhint %}

{% hint style="info" %}
\.      Output Module  
\.      M225F : Digital 16점  
\.      M226F : Digital 16점  
\.      M2768 : Digital 8점   
\.      M4534 : Analog 4점  
{% endhint %}

{% hint style="info" %}
\.      Special Module  
\.      M5112 : Conveyer I/F 
{% endhint %}

<br>

![[그림 3.1-6 EtherCAT Master 설정]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_6.png>) 

<br>

##### 5. 설정 완료 후 제어기를 재부팅합니다.

![[그림 3.1-7 EtherCAT Master 설정]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_7.png>) 

<br>

![[그림 3.1-8 EtherCAT Master 설정]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_8.png>) 

<br>

{% hint style="info" %}
\.      설정 완료 후 제어기를 재부팅해 주십시오.
{% endhint %}

<br>

##### 6. 설정값이 반영되어있는지 확인 후, 통신 상태를 확인합니다.

![[그림 3.1-9 EtherCAT Master 설정]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_9.png>) 

<br>

{% hint style="info" %}
\.      통신 연결 상태와 Error 여부를 확인해 주십시오.
{% endhint %}

<br>

![[그림 3.1-10 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_10.png>)

<br>

{% hint style="info" %}
\.      Remote IO Module 에서 LED를 이용해 정상적으로 통신이 개통되어 있는지 확인해 주십시오.
{% endhint %}

<br>

{% hint style="info" %}
\.      **통신 상태에서 ERROR 발생시 (“[**3.2 EtherCAT Master IO 에러 조치**](../3-ethercat-master-io/2-Error-EtherCAT-Master.md)”)를 확인해 주십시오.**
{% endhint %}

<br>

##### 7. 통신 설정 완료 후 IO Block 을 할당합니다.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**4. 산업용 통신 IO Block 할당**](../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}


[__SOURCE](3-ethercat-master-io/2-Error-EtherCAT-Master.md)
# 3.2 EtherCAT Master IO 에러 조치

EtherCAT Master IO 설정 중 발생할 수 있는 주요 Error 를 해결하기 위한 방법입니다.

<br>

![[그림 3.2-1 EtherCAT Master 상태]](<../_assets/3-ethercat-master-io/2-Error/image_1.png>) 

{% hint style="info" %}
\.      LAN Cable 의 연결 상태를 확인해 주십시오.

\.      Adapter Device 의 전원이 켜져 있는지 확인해 주십시오.

\.      Remote IO Module 의 IO 조합과 동일하게 설정이 되었는지 확인해 주십시오.
{% endhint %}

<br>

[__SOURCE](4-pnio/README.md)
# 4. PROFINET I/O (Hi7)

<br>

이 장에서는 PROFINET I/O 장치(BD671)를 활용한 로봇 제어기 내부 입출력 신호와의 연결 방법을 설명합니다. <br>

<br>


{% hint style="info" %}
PROFINET I/O (BD671)의 기능은 Hi7 로봇제어기에서 지원합니다.<br>
PROFIsafe 메뉴얼은 SafeSpace 2.0 메뉴얼을 참고하세요 ([SafeSpace 2.0 링크](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/korean/3-safety-function/3-safety-function/4-safety-io/4-profisafe))
{% endhint %}
[__SOURCE](4-pnio/1-pnio.md)

## 1. PROFINET ?
- PROFINET은 산업 자동화를 위한 이더넷 기반 통신 표준입니다.
- 컨트롤러(PLC, 로봇제어기 등)와 분산 I/O 장치(드라이브, 센서, 모듈 등) 간의 실시간 데이터 교환을 지원합니다.

## 2. PROFINET 사양
- 디지털 입력 : 50 , 120, 240 bytes (1개 선택) 
- 디지털 출력 : 50 , 120, 240 bytes (1개 선택) 
- 안전 입출력 : 8/8 bytes (활성 or 비활성화) 
- 최소 통신 주기 : 1 msec
- 지원 통신 속도 : 10 or 100 Mbps
- Conformance Class : B
- Netload Class : II
- Optional Feature : Legacy, MRP

## 3. PROFINET 설정 절차

1) BD671과 PROFINET 컨트롤러 & Hi7 Com의 연결
2) GSDML 파일 등록 (TIA Portal)
3) PROFINET 컨트롤러 설정 (TIA Portal)
4) Hi7 설정 (TP UI)
5) PROFINET 통신의 확인
6) PROFINET I/O 신호의 할당(FB Block Settings)

### 3.1 BD671과 F-Host & Hi7 Com의 연결

#### 3.1.1 랜선 연결
1) PROFINET 컨트롤러와 BD671를 랜선으로 연결한다.
2) Link LED가 점멸하는지 확인한다.
3) Hi7 COM의 LAN3 커넥터와 BD671를 랜선으로 연결한다.
4) Link LED가 점멸하는지 확인한다.

![](../_assets/4-pnio/profisafe_connect.png)

#### 3.1.2 Hi7 Com의 연결 설정
1) 다음과 같이 메뉴를 이동 시스템 -> 제어 파라미터 -> 산업용 통신-> EtherCAT Master 설정
2) 아래와 같이 설정
- EtherCAT Master : ON
- Port : LAN3
3) 슬레이브 리스트에서 "OptionBD – PROFINET_IO"를 선택하고 적용 버튼을 누른다.
4) Hi7 로봇제어기를 재부팅한다.
5) 재부팅후 Run & Communication & Error LED 점등 상태를 확인한다.

![](../_assets/4-pnio/EC_master_setting1.png)
<br> <br>
![](../_assets/4-pnio/EC_master_setting2.png)


### 3.2 GSDML 파일 등록 (TIA Portal)
1) TIA Portal을 실행
2) 메뉴에서 우측과 같이 이동 [Options] → [Manage general station description file (GSD)].
3) “…” 버튼 클릭 후 and GSDML file이 있는 디렉토리를 설정한다.
4) 화면에 표시된 리스트에서 “GSDML-V2.43-Hyundai-Robotics-HI6-20251127.xml”를 선택하고 [Install] 버튼을 누른다.
5) 하드웨어 카탈로그에 새로운 장치로 등록되었는지 확인한다. <br>
![](../_assets/4-pnio/profisafe_gsdmal.png)

### 3.3 PROFINET 컨트롤러 설정 (TIA Portal)
1) TIA Portal을 실행시키고 새 프로젝트를 생성한다.
2) Device & Network 부분을 더블클릭하여 오픈한다.<br>
![](../_assets/4-pnio/profisafe_device_network.png)

3) PROFINET 통신을 지원하는 컨트롤러(예 CPU 1511F-1 PN)를 선택하여 네트워크 뷰쪽으로 끌어다 놓는다.
4) 하드웨어 카탈로그에서 이전 단계에서 추가한 장치(HRC, PROFINET I/O DAP)를 추가하고 네트워크 뷰쪽으로 끌어다 놓는다.
5) 두 장치 그림에서 랜포트를 마우스 드래그&드랍으로 서로 연결한다.<br>
![](../_assets/4-pnio/profisafe_device_network2.png)

6) “Device & Network”화면에서 HRC-IO 장치를 더블 클릭
7) 원하는 슬롯을 선택한다.
8) 오른쪽 카탈로그에서 원하는 모듈을(DI, DO, or PROFIsafe I/O) 드래그하여 "Device Overview window"로 이동시킨다.<br>
![](../_assets/4-pnio/profisafe_device_network3.png)

9) “Device & Network”화면에서 HRC-IO 장치를 더블 클릭
10) HRC-IO장치를 다시 클릭하여 Setting화면을 오픈
11) 아래에서 General 탭으로 이동
12) 왼쪽 메뉴에서 Ethernet addresses 선택
13) “Generate PROFINET device name automatically.” 부분 체크 해제
14) "PROFINET device name"을 "hd-hrc-hi7"로 설정하고 저장함.<br>
![](../_assets/4-pnio/profisafe_device_network4.png)

### 3.4 Hi7 설정 (TP UI)
1) PNIO 컨트롤러에서 설정했던 값과 같은 아래의 값으로 파라미터 설정
- PROFINET IO Device Name : hd-hrc-hi7
- Slot 1 : Digital Input : 240
- Slot 2 : Digital Output : 240
- Slot 3 : Safety I/O : No

2) "전체 적용" 버튼을 누른다.<br>
![](../_assets/4-pnio/4_1_profinet_config.png)

### 3.5 PROFINET 통신의 확인
### 3.5.1 래더 프로그램 (Tia Portal)
1) Device Overview 탭 에서, 아래와 같이 래더 프로그램을 만들고 컨트롤러로 다운로드 한다.<br>
![](../_assets/4-pnio/5_1_Safety_Ladder.png)
2) 다운로드 후, Distribution I/O 화면에서 녹색 체크 박스가 표시되었는지 확인한다.<br>
![](../_assets/4-pnio/5_1_Safety_Ladder2.png)

### 3.5.2 TP 화면
메뉴에서 시스템 -> 안전시스템 -> 모니터링 -> PROFINET 상태로 이동한다.<br>
![](../_assets/4-pnio/5_2_pnio_status.png)
- 각 슬롯의 상태 정보를 확인
- Counter가 지속 증가하는지 확인


### 3.6 PROFINET I/O 신호의 할당(FB Block Settings)
1) 시스템 → 제어 파라미터 → 입출력 신호 설정 → FB 블럭 할당으로 이동
2) 2개 이하로 필요한 만큼 블럭 설정을 PROFINET I/O로 변경한다.
 (최대 PROFINET I/O 사이즈는 240바이트이고 개별 FB 블럭의 사이즈는 120바이트 입니다. 따라서 **2개를 초과하는 설정은 무시됩니다.**)<br>
![](../_assets/4-pnio/6_fb_block.png)

3) 추가로 조건 설정 메뉴로 이동하여 PLC 동작 모드가 OFF되어 있는지 확인합니다.<br>
![](../_assets/4-pnio/6_1_condition.png)
4) TIA Portal과 범용 I/O 화면에서 입출력 신호 확인<br>
![](../_assets/4-pnio/6_3_public_io.png)

[__SOURCE](4-pnio/2-pnio-status.md)
# 5.3 PROFINET 모니터링

**\[시스템 > 8: 안전 시스템 > 3: 모니터링 > 4: PROFINET 상태]** 메뉴를 선택하여 PROFINET 상태를 슬롯별로 모니터링 할 수 있습니다.

<p align="center">
<img src="../_assets/4-pnio/5_2_pnio_status.png"></img>
<em><p align="center">PROFINET 상태 모니터링 화면</p></em>
</p>

- 크기 : 설정된 I/O Size를 의미(단위 : 바이트)
- 상태 : BAD(사용안함 or 통신이상), GOOD(통신 정상)
- 카운터 : I/O 갱신 횟수(지속 증가시 통신 정상)

<p align="center">
<img src="../_assets/4-pnio/profinet_LED.png"></img>
<em><p align="center">BD671(PROFINET) </p></em>
</p>

[__SOURCE](5-io-block-allocation.md)
# 5. 산업용 통신 IO 읽기 및 쓰기

산업용 통신 설정 완료 후 제어기와의 통신을 위한 IO Block 할당 방법 입니다.

산업용 통신 IO를 사용하기 위해 fb0 \~ fb9 영역에 할당해야 합니다.

<br>

{% hint style="info" %}
\.      fb 블록의 IO 읽기/쓰기 방법은 아래 매뉴얼을 참조해 주십시오.

\.   **\[제어기 조작설명서 : 범용 입력]**   
\.   **\[제어기 조작설명서 : 범용 출력]**   
{% endhint %}

<br>

##### 1. IO 블록 할당 메뉴를 선택
   **\[시스템 > 2: 제어 파라미터 > 2: 입출력 신호 설정 > 6: FB 블록 할당]** 메뉴를 터치하십시오.

<br>

##### 2. 원하는 fb 영역에 산업용 통신 종류 지정
   지정 후 **\[OK]** 버튼을 터치하십시오.

![[그림 5-1]](<_assets/4-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[주의]**: 내장 PLC와 함께 사용하는 경우 IO 속성, DI/DO - X/Y 를 확인해 주십시오. 
{% endhint %}

{% hint style="warning" %}
**\[주의]**: EtherNet/IP 어댑터의 경우 최대 블록사이즈는 120 Bytes 이며 최대 2개까지 선택할 수 있습니다. 2개를 초과하는 선택은 무시 됩니다. 
{% endhint %}

[__SOURCE](6-slave-config-file.md)
# 6. Slave 장치 설명 파일

산업용 통신 Master에서 Slave 통신 구성을 위해 각 Protocol 별 Slave 장치의 대한 설명 파일을 사용합니다.

<br>

Slave 장치 설명 파일은 당사 홈페이지에 다운로드 받을 수 있습니다.
[www.hd-hyundairobotics.com](https://hd-hyundairobotics.com/) -> 산업용 로봇 홈페이지 -> 고객지원 -> 응용소프트웨어에서 "Hi7 Fieldbus Config"을 다운로드 합니다.

<br>

{% hint style="info" %}
\.      EtherNet/IP : EDS 파일

\.      PROFINET IO : GSDML (.XML) 파일

\.      EtherCAT : ESI (.XML) 파일

\.      PROFIBUS-DP : GSD 파일

\.      DeviceNet : EDS 파일

\.      CC-Link IE Field : CSPP 파일

\.      CC-Link IE Basic : CSPP 파일
{% endhint %}

<br>

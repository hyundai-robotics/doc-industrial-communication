# 3.3 EtherNet/IP

이 장에서는 EtherNet/IP Master(Scanner) 와 Slave(Adapter)의 특성과 설정 방법에 대해 기술합니다. 

<br>

##### EtherNet/IP 개요

EthetNet/IP 는 CI(ControlNet International)와 ODVA(Open DeviceNet Vendors Association)에 의해 개발된 이더넷 기반의 개방형 산업용 통신 프로토콜입니다.

공장에서 센서, 리모트 IO, 모터 드라이버, HMI, PLC, 로봇 제어기 등 다양한 장치가 제조사와 무관하게 하나의 EtherNet/IP 네트워크에 연결될 수 있습니다.

![[그림 3.3-1 EtherNet/IP]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/image_1.png>) 

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
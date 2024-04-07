# 3.4 PROFINET IO

이 장에서는 PROFINET IO Master(Controller) 와 Slave(Device)의 특성과 설정 방법에 대해 기술합니다. 

<br>

##### PROFINET IO 개요

PROFINET IO 는 PROFIBUS-DP와 산업용 이더넷으로부터 진보적으로 발전된 이더넷 기반의 개방형 산업용 통신 프로토콜입니다.

![[그림 3.4-1 PROFINET IO]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/image_1.png>) 

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

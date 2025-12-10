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
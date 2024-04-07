# 3.5.5 EtherCAT 케이블 결선 (Topology)

<br>

EtherCAT 기존 산업용 통신들과 달리 Cable 결선과 사용할 수 있는 Ethernet Port에 제약이 있습니다.

##### 1. Ethernet Port

{% hint style="info" %}
\.      EthreCAT Master와 Slave를 연결하는 경우 Port 0번을 사용해야 합니다.
{% endhint %}

![[그림 3.5.5-1 EtherCAT Topology]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
\.      Master에 Slave 가 1개 연결되는 경우
{% endhint %}

![[그림 3.5.5-2 EtherCAT Topology]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
\.      Master에 Slave 가 2개 이상 연결되는 경우

\.      Slave Port 1번에서 다음 Slave Port 0번으로 연결합니다.
{% endhint %}

![[그림 3.5.5-3 EtherCAT Topology]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_3.png>) 

<br>

##### 2. Redundancy 

{% hint style="info" %}
\.      Master에서 Redundancy 기능을 사용하는 경우 

\.      마지막 Slave의 Port 1번과 Master의 Port 1번을 연결하여 Ring 구조를 형성합니다.
{% endhint %}

![[그림 3.5.5-4 EtherCAT Topology]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_4.png>) 


<br>

##### 3. Cable 결선 ERROR


"[**4.1 ERROR Code**](../../4-monitoring-industrial-communication/4-1-error-code.md)" 참고해 주십시오.

<br>

{% hint style="info" %}
\.      Network Scan 이 안되는 경우

\.      Master에 연결된 Port와 Cable을 확인해 주십시오.
{% endhint %}

![[그림 3.5.5-5 EtherCAT ERROR]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
\.      Topology Error (Configuration 에서 Error)

\.      Master와 Slave 간 Cable 결선을 확인해 주십시오.
{% endhint %}

![[그림 3.5.5-6 EtherCAT ERROR]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
\.      Topology Error 2 (Configuration 에서는 정상이나 진단시 Error)

\.      Master와 Slave 간 Cable 결선을 확인해 주십시오.

\.      Slave와 Slave 간 Cable 결선을 확인해 주십시오.
{% endhint %}

![[그림 3.5.5-7 EtherCAT ERROR]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_7.png>)

![[그림 3.5.5-8 EtherCAT ERROR]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
\.      Mandatory Slave Missing Error

\.      Slave와 Slave 간 Cable 결선을 확인해 주십시오.
{% endhint %}

![[그림 3.5.5-9 EtherCAT ERROR]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_9.png>)
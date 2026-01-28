# 3. EtherCAT Master IO

<br>

이 장에서는 EtherCAT Master 를 이용하여 당사에서 선정한 몇가지의 표준 Remote IO Module을 연결하는 방법에 대해 설명합니다.

<br>

**EtherCAT 개요**

EtherCAT은 Beckhoff Automation 에서 개발된 이더넷 기반의 Fieldbus 시스템입니다.

EtherCAT 프로토콜은 매우빠른 IO Data 업데이트와 정확한 동기화를 위한 기능을 제공합니다. 

<br>

**EtherCAT Master IO**
   * 기존 필드버스 마스터(Master)에 해당되는 제품으로 EtherCAT 슬레이브(Slave) 장치들에게 IO 데이터 연결을 요청할 수 있습니다.

<br>

{% hint style="info" %}
\.      EtherCAT Master 는 제어기의 범용 LAN Port 를 사용합니다.


\.      Remote IO Module은 Crevis 사의 M9386 EtherCAT Network Adapter를 사용합니다.
{% endhint %}



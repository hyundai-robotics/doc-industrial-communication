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


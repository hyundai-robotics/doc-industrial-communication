# 3.4.4 PROFINET IO Device 설정

“[**3.1 산업용 통신 펌웨어 설정**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      **[PROFINET IO Device GSDML File 다운로드]**

\.      “[**6. Slave 장치 설명 파일**](../../6-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

<br>

##### 1. TP를 이용하여 산업용 통신 펌웨어 설정에서 PROFINET IO Slave를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 3.4.4-1 펌웨어 설정]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 현재 선택되어 있는 통신 Protocol 준비 상태를 확인합니다.

![[그림 3.4.4-2 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[주의]**: Sycon.net 으로 설정한 Configuration 파일이 해당 PCI 슬롯에 Download 되어 있는 경우 TP의 설정 값을 무시하게 됩니다.
{% endhint %}

<br>

##### 3. 메뉴를 터치하여 슬레이브 설정 화면으로 진입 합니다. 
**\[시스템 > 2: 제어 파라미터 > 11: 산업용 통신 > 2: 슬레이브 구성 >  PROFINET IO Slave]**

![[그림 3.4.4-3 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_3.png>) 

![[그림 3.4.4-4 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_4.png>) 

<br>

##### 4. 각 항목 별 설명

{% hint style="info" %}
\.      [Station Name]

\.      PROFINET IO는 Station Name을 통해 Slave를 식별합니다.

\.      Naming Rule
\.       > PROFINET IO 로 연결된 Device들의 이름이 중복될 수 없습니다.  
\.       > 최대 240자로 이름을 설정할 수 있습니다.  
\.       > 특수 문자는 "." , "-" 를 사용할 수 있습니다.  
\.       > 문자는 영문과 숫자를 사용할 수 있습니다.  
\.       > 이름 시작과 끝은 영문 또는 숫자로 시작해야 합니다.  
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
\.      Master 에서 Slot 설정 시

\.      설정한 바이트 수와 일치하도록 Master에서 Slot을 지정해 주어야합니다.

\.      4, 8, 16, 32, 64 Bytes -> 각 Bytes 에 맞는 Slot 지정  
\.      128, 256 Bytes -> 64 Bytes Slot 다수 지정 (2개, 4개)

\.      입력 Slot이 출력 Slot 보다 앞에 위치 합니다.
{% endhint %}

![[그림 3.4.4-5 슬레이브 설정]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_5.png>) 


<br>

##### 5. 설정 완료 후 아래 절차에 따라 통신 상태를 확인하여 주십시오.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**4 산업용 통신 모니터링**](../../4-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[그림 3.4.4-6 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/4-Slave_setting/image_6.png>) 
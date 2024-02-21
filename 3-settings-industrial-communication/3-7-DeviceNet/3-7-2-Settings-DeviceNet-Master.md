# 3.7.2 DeviceNet Master 설정

“[**3.1 산업용 통신 펌웨어 설정**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)" 및 "[**3.2 SYCON.NET 설정**](../../3-settings-industrial-communication/3-2-Settings-SYCON.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      DeviceNet Connector 연결은 아래를 참고해 주십시오.

\.      (“[**2.2 커넥터**](../../2-mounting-settings-industrial-communication-card/2-2-Connector.md)”)
{% endhint %}

<br>

##### 1. 산업용 통신 펌웨어 설정에서 DeviceNet Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 3.7.2-1 펌웨어 설정]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

![[그림 3.7.2-2 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_2.png>) 

<br>

##### 3. Sycon.net 을 이용하여 DeviceNet Master PCI 장치를 선택합니다.

![[그림 3.7.2-3 DeviceNet Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_3.png>)
![[그림 3.7.2-4 DeviceNet Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_4.png>) 

<br>

##### 4. PCI 장치를 Scan 하고 DeviceNet Master 적용(Apply)합니다.

![[그림 3.7.2-5 Sycon.net Scan]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_5.png>) 

<br>

##### 5. 통신 속도를 설정합니다.

{% hint style="warning" %}
\.      Master 와 Slave의 통신속도가 다르면 Network Scan이 정상적으로 이루어지지 않습니다.
{% endhint %}

![[그림 3.7.2-6 DeviceNet Master Download]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_6.png>) 

<br>

##### 6. 설정을 다운로드 합니다.

![[그림 3.7.2-7 DeviceNet Master Download]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_7.png>) 

<br>

##### 7. DeviceNet Master 에 연결할 Slave 모듈을 준비합니다.
   * 이번 예제에서는 Crevis 사의 NA-9211 DeviceNet Slave를 사용합니다.
   * 시스템 전원과 필드 전원을 공급해 주어 모듈을 활성화 시켜 주십시오.

![[그림 3.7.2-8 Crevis NA-9211]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_8.png>) 

<br>

##### 8. Slave 장치의 설정

{% hint style="info" %}
\.      DeviceNet Slave 장치의 MAC ID와 통신속도, 종단저항 설정합니다.
{% endhint %}

![[그림 3.7.2-9 Crevis NA-9211]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_9.png>) 

![[그림 3.7.2-10 Crevis NA-9211]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_10.png>)

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

![[그림 3.7.2-11 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_11.png>)

{% hint style="info" %}
\.      다운로드한 EDS 파일을 모두 Sycon.net 에 등록합니다.

\.      EDS File 등록시 산업용 통신 Protocol (DeviceNet)를 확인해 주십시오.
{% endhint %}

![[그림 3.7.2-12 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_12.png>)

<br>

![[그림 3.7.5-13 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_13.png>)



<br>

##### 10. Network Scan

{% hint style="warning" %}
\.      **Network Scan 시 아래 사항을 반드시 확인해 주십시오.**

\.      **(1) 케이블 연결 여부**  
\.      **(2) 종단저항 연결 또는 종단 DIP Switch 사용 여부**  
\.      **(3) Master - Slave 통신 속도 설정 여부**  

\.      **원활한 통신 연결을 위해 (“[**3.7.5 DeviceNet ERROR 조치**](../3-7-DeviceNet/3-7-5-Error-DeviceNet.md)”)을 반드시 확인해 주십시오.**
{% endhint %}

{% hint style="info" %}
\.      DeviceNet Master 는 Network Scan 기능을 지원합니다.
{% endhint %}

{% hint style="info" %}
\.      DeviceNet Master 장치에서 우클릭 후 Network Scan을 클릭합니다.
{% endhint %}

![[그림 3.7.2-14 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      EDS 파일이 등록되지 않은 경우 Network Scan을 하면 Slave 정보는 나타나지만 등록은 불가능합니다.
{% endhint %}

{% hint style="info" %}
\.      정상적으로 EDS 파일이 등록된 경우 Network Scan을 통해 Slave 장치를 추가할 수 있습니다.
{% endhint %}

![[그림 3.7.2-15 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_15.png>)

![[그림 3.7.2-16 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_16.png>)

<br>

##### 11. Slave 장치 Configuration

{% hint style="info" %}
\.      Slave 장치 Configuration을 위해 Master 장치의 Disconnect를 클릭합니다.
{% endhint %}

![[그림 3.7.2-17 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
\.      Slave 장치를 더블클릭합니다.
{% endhint %}

![[그림 3.7.2-18 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_18.png>)


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

![[그림 3.7.2-19 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_19.png>)

<br>

{% hint style="info" %}
\.      Crevis NA-9211 은 UCMM 미체크 후 진행합니다. (Group2 기본 값 사용)
{% endhint %}

![[그림 3.7.2-20 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_20.png>)

<br>


{% hint style="info" %}
\.      DeviceNet Slave의 설정을 확인 합니다.

\.      Output : ST-2318 (1 Byte)  
\.      Input : ST-1218 (1 Byte)  
{% endhint %}

![[그림 3.7.2-21 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_21.png>)



<br>

##### 12. Master 장치 Configuration

{% hint style="info" %}
\.      Master 장치를 더블클릭합니다.
{% endhint %}

![[그림 3.7.2-22 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_22.png>)


{% hint style="info" %}
\.      DeviceNet 통신 속도를 설정합니다. (Slave 통신 속도와 동일하도록)
{% endhint %}

![[그림 3.7.2-23 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      Address Table에서 각 Slave Slot의 할당된 IO 및 시작 주소를 확인 합니다.
{% endhint %}

![[그림 3.7.2-24 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.      Quick Connect 기능 사용 유무를 설정합니다.
{% endhint %}

![[그림 3.7.2-25 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_25.png>)


{% hint style="info" %}
\.      설정을 완료 후 Download를 진행해 주십시오.
{% endhint %}

![[그림 3.7.2-26 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_26.png>)

<br>

##### 13. 통신 상태 확인

{% hint style="info" %}
\.        Sycon.net 과 TP 에서 통신 상태를 확인 합니다.

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**4 산업용 통신 모니터링**](../../4-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      Connected 된 Master 장치를 더블클릭하여 통신 상태를 확인 할 수 있습니다.
{% endhint %}

![[그림 3.7.2-27 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_27.png>)

![[그림 3.7.2-28 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.        Sycon.net 의 Diagnosis 기능을 이용하여 통신 상태와 함게 IO 입출력 상태를 모니터링 할 수 있습니다.
{% endhint %}

![[그림 3.7.2-29 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_29.png>)


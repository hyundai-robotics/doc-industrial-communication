# 3.4.2 PROFINET IO Controller 설정

“[**3.1 산업용 통신 펌웨어 설정**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)" 및 "[**3.2 SYCON.NET 설정**](../../3-settings-industrial-communication/3-2-Settings-SYCON.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.


<br>

##### 1. 산업용 통신 펌웨어 설정에서 PROFINET IO Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 3.4.2-1 펌웨어 설정]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

![[그림 3.4.2-2 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

##### 3. Sycon.net 을 이용하여 PROFINET IO Controller PCI 장치를 선택합니다.

![[그림 3.4.2-3 PROFINET IO Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_3.png>)
![[그림 3.4.2-4 PROFINET IO Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

##### 4. PCI 장치를 Scan 하고 PROFINET IO Controller 적용(Apply)합니다.

![[그림 3.4.2-5 Sycon.net Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

##### 5. 설정을 다운로드 합니다.

![[그림 3.4.2-6 PROFINET IO Controller Download]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

##### 6. PROFINET IO Controller 에 연결할 Device(Slave) 모듈을 준비합니다.
   * 이번 예제에서는 Crevis 사의 M9287 PROFINET IO Device를 사용합니다.
   * 시스템 전원과 필드 전원을 공급해 주어 모듈을 활성화 시켜 주십시오.

![[그림 3.4.2-7 Crevis M9287]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
\.      DIP Switch 을 이용한 PROFINET IO Device 이름 설정 방법

\.      M9287-XX : Dip Switch 로 설정한 번호

\.      이번 예제에서는 1번 Dip Switch를 이용해 이름을 M9287-01 로 설정하였습니다.
{% endhint %}

<br>

##### 7. (Dip Switch 예제) DIP Switch를 이용하여 Slave 장치의 이름을 설정합니다.
   * 1번 DIP Switch만 ON으로 변경합니다.


![[그림 3.4.2-8 Crevis M9287 Dip Swicth]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      DIP Switch 설정 후 장치를 재부팅 해주십시오.
{% endhint %}

<br>

##### 8. Slave 장치의 GSDML 파일을 등록합니다.

{% hint style="info" %}
\.      Sycon.net에 등록되지 않은 Device를 사용하기 위해 GSDML 파일이 필요합니다.

\.      M9287 Device의 GSDML 파일은 Crevis 홈페이지에서 다운로드 할 수 있습니다.
{% endhint %}

![[그림 3.4.2-9 Crevis GSDML File]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      다운로드한 GSDML 파일을 Sycon.net 에 등록합니다.

\.      GSDML File 등록시 산업용 통신 Protocol (PROFINET IO)를 확인해 주십시오.
{% endhint %}

![[그림 3.4.2-10 Crevis GSDML File]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_10.png>)![[그림 3.4.2-11 Crevis GSDML File]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_11.png>)
![[그림 3.4.2-12 Crevis GSDML File]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_12.png>)

![[그림 3.4.2-13 Crevis GSDML File]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_13.png>)


<br>

##### 9. Network Scan

{% hint style="info" %}
\.      PROFINET IO Controller 는 Network Scan 기능을 지원합니다.
{% endhint %}

{% hint style="info" %}
\.      PROFINET IO Master 장치에서 우클릭 후 Network Scan을 클릭합니다.
{% endhint %}

![[그림 3.4.2-14 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      GSDML 파일이 등록되지 않은 경우 Network Scan을 하면 Slave 정보는 나타나지만 등록은 불가능합니다.
{% endhint %}

![[그림 3.4.2-15 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      정상적으로 GSDML 파일이 등록된 경우 Network Scan을 통해 Slave 장치를 추가할 수 있습니다.
{% endhint %}

![[그림 3.4.2-16 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_16.png>)

![[그림 3.4.2-17 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_17.png>)

![[그림 3.4.2-18 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

##### 10. Slave(Device) 장치 Configuration

{% hint style="info" %}
\.      Slave 장치 Configuration을 위해 Master 장치의 Disconnect를 클릭합니다.
{% endhint %}

![[그림 3.4.2-19 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      Slave 장치를 더블클릭합니다.
{% endhint %}

![[그림 3.4.2-20 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      PROFINET IO Slave(Device) 설정을 위해 M9287에 연결되어 있는 Slot을 추가합니다.

\.      Slot 1 : M7001  
\.      Slot 2 : M12DF  
\.      Slot 3 : M225F  
{% endhint %}

![[그림 3.4.2-21 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_21.png>)

![[그림 3.4.2-22 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

##### 11. Master(Controller) 장치 Configuration

{% hint style="info" %}
\.      Master 장치를 더블클릭합니다.
{% endhint %}

![[그림 3.4.2-23 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      Master 장치와 Slave 장치의 IP 주소를 설정해줍니다.

\.      PROFINET IO Device의 Slave IP 주소는 Master 에서 설정합니다.

\.      IP 주소는 Master와 Slave가 같은 대역안에서 서로 중복되지 않도록 해주십시오.
{% endhint %}

![[그림 3.4.2-24 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_24.png>)

![[그림 3.4.2-25 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      Master 장치에서 Slave 장치의 Slot 정보가 올바른지 확인해주십시오.
{% endhint %}

![[그림 3.4.2-26 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.      Address Table에서 각 Slave Slot의 할당된 IO 및 시작 주소를 확인 합니다.
{% endhint %}

![[그림 3.4.2-27 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.      PROFINET IO의 IO 통신속도를 설정합니다.
{% endhint %}

![[그림 3.4.2-28 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.      설정을 완료 후 Download를 진행해 주십시오.
{% endhint %}

![[그림 3.4.2-29 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

##### 12. 통신 상태 확인

{% hint style="info" %}
\.        Sycon.net 과 TP 에서 통신 상태를 확인 합니다.

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**4 산업용 통신 모니터링**](../../4-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      Connected 된 Master 장치를 더블클릭하여 통신 상태를 확인 할 수 있습니다.
{% endhint %}

![[그림 3.4.2-30 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_30.png>)

![[그림 3.4.2-31 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
\.        Sycon.net 의 Diagnosis 기능을 이용하여 통신 상태와 함게 IO 입출력 상태를 모니터링 할 수 있습니다.
{% endhint %}

![[그림 3.4.2-32 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_32.png>)
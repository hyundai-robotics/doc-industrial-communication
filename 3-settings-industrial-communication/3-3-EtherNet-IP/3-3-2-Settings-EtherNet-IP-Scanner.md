# 3.3.2 EtherNet/IP Scanner 설정

“[**3.1 산업용 통신 펌웨어 설정**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)" 및 "[**3.2 SYCON.NET 설정**](../../3-settings-industrial-communication/3-2-Settings-SYCON.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.


<br>

##### 1. 산업용 통신 펌웨어 설정에서 EtherNet/IP Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 3.3.2-1 펌웨어 설정]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

![[그림 3.3.2-2 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

##### 3. Sycon.net 을 이용하여 EtherNet/IP Scanner PCI 장치를 선택합니다.

![[그림 3.3.2-3 EtherNet/IP Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_3.png>)
![[그림 3.3.2-4 EtherNet/IP Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

##### 4. PCI 장치를 Scan 하고 EtherNet/IP Scanner 적용(Apply)합니다.

![[그림 3.3.2-5 Sycon.net Scan]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

##### 5. 설정을 다운로드 합니다.

![[그림 3.3.2-6 EtherNet/IP Scanner Download]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

##### 6. EtherNet/IP Scanner 에 연결할 Adapter(Slave) 모듈을 준비합니다.
   * 이번 예제에서는 Crevis 사의 M9289 EtherNet/IP Adapter를 사용합니다.
   * 시스템 전원과 필드 전원을 공급해 주어 모듈을 활성화 시켜 주십시오.

![[그림 3.3.2-7 Crevis M9289]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

##### 7. EtherNet/IP 통신 연결을 위해 Apdapter(Slave) 의 IP Address를 설정합니다.

{% hint style="info" %}
\.      Dip Switch 를 이용한 IP Address 설정
{% endhint %}

![[그림 3.3.2-8 Crevis M9289 Dip Swicth]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
\.      BootpSvr.exe 을 이용한 IP Address 설정 방법
{% endhint %}

<br>

##### 8. (Bootp 예제) Bootp를 이용하여 Slave 장치의 IP Address를 설정합니다.
   * 9번 DIP Switch만 ON으로 변경합니다.

![[그림 3.3.2-9 Crevis M9289 Dip Swicth]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_9.png>)

   * M9289 Adapter LAN 포트에 PC를 연결합니다.

![[그림 3.3.2-10 Crevis M9289 LAN Port]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

##### 9. PC 에서 BootpSvr.exe 를 실행합니다.
   * 해당 프로그램은 Crevis 사에서 제공합니다. (홈페이지에서 IO Guide Pro 다운로드)

![[그림 3.3.2-11 Crevis IO Guide Pro]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_11.png>)

![[그림 3.3.2-12 Crevis Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
\.      Start BootP를 누른 상태에서 M9289 모듈의 전원을 분리하고 다시 인가하여 재부팅합니다.
{% endhint %}

![[그림 3.3.2-13 Crevis Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

##### 10. Adapter 장치를 재부팅하면 BootpSvr.exe 프로그램에 Device 정보가 나타납니다.

![[그림 3.3.2-14 Crevis Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

##### 11. Device를 선택하여 IP를 설정합니다.

![[그림 3.3.2-15 Crevis Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_15.png>)![[그림 3.3.2-16 Crevis Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

##### 12. IP 설정이 끝난 Adapter의 DIP Switch를 모두 OFF로 변경한 후 장치를 재부팅합니다.

{% hint style="info" %}
\.      DIP Switch의 상태 Adapter 재부팅 여부를 반드시 확인해 주십시오.
{% endhint %}

![[그림 3.3.2-17 Crevis DIP Switch]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

##### 13. Slave 장치의 EDS 파일을 등록합니다.

{% hint style="info" %}
\.      Sycon.net에 등록되지 않은 Device를 사용하기 위해 EDS 파일이 필요합니다.

\.      M9289 Adapter의 EDS 파일은 Crevis 홈페이지에서 다운로드 할 수 있습니다.
{% endhint %}

![[그림 3.3.2-18 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
\.      다운로드한 EDS 파일을 Sycon.net 에 등록합니다.

\.      EDS File 등록시 산업용 통신 Protocol (EtherNet/IP)를 확인해 주십시오.
{% endhint %}

![[그림 3.3.2-19 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_19.png>)![[그림 3.3.2-20 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_20.png>)
![[그림 3.3.2-21 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_21.png>)

![[그림 3.3.2-22 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_22.png>)

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

![[그림 3.3.2-23 Sycon.net Bus]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      해당 Device (Adapter)를 더블클릭하여 설정을 진행합니다.

\.      해당 Device에 장착된 IO 장치에 알맞게 Input / Output Byte 수를 설정합니다.

\.      이 예제에서는 아래와 같이 설정했습니다.
{% endhint %}

{% hint style="info" %}
\.        O -> T : Originator(Master) -> Target (Slave)

\.        Output : EtherNet/IP Scanner (OUT) -> M9289 (INPUT Module M225F) : 2Byte
{% endhint %}

![[그림 3.3.2-24 Adapter Device Settings]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.        T -> O : Target (Slave) -> Originator(Master)

\.        Input : M9289 (OUTPUT Module M12DF) -> EtherNet/IP Scanner (IN)

\.        **System Status(Default) 1Byte + M12DF 2Byte => 3Byte**
{% endhint %}

![[그림 3.3.2-25 Adapter Device Settings]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_25.png>)

<br>

##### 16. Master(Scanner) 장치 Configuration
    

{% hint style="info" %}
\.        Master Device를 우클릭하여 Disconnect 합니다.
{% endhint %}

![[그림 3.3.2-26 Adapter Device Settings]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Master Device를 더블클릭합니다.

\.        Master Device의 IP Address를 설정합니다. 
{% endhint %}

![[그림 3.3.2-27 Adapter Device Settings]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.        Slave Device의 IP Address를 설정합니다. 
{% endhint %}

![[그림 3.3.2-28 Scanner Device Settings]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.        Slave Device의 Scan Time을 설정합니다. 

\.        해당 값을 조절하여 적절한 통신 속도를 설정해 주십시오.
{% endhint %}

![[그림 3.3.2-29 Scanner Device Settings]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.        Address Table에서 Slave 장치의 설정을 확인해 주십시오.

\.        Input / Output IO Byte 수와 시작 Address 를 확인해 주십시오.
{% endhint %}

![[그림 3.3.2-30 Scanner Device Settings]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_30.png>)

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

![[그림 3.3.2-31 Scanner Device Settings]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

##### 17. 통신 상태 확인

{% hint style="info" %}
\.        Sycon.net 과 TP 에서 통신 상태를 확인 합니다.

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**4 산업용 통신 모니터링**](../../4-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      Connected 된 Master 장치를 더블클릭하여 통신 상태를 확인 할 수 있습니다.
{% endhint %}

![[그림 3.3.2-32 Communication State]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_32.png>)

![[그림 3.3.2-33 Communication State]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
\.        Sycon.net 의 Diagnosis 기능을 이용하여 통신 상태와 함게 IO 입출력 상태를 모니터링 할 수 있습니다.
{% endhint %}

![[그림 3.3.2-34 Communication State]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_34.png>)
# 3.6.2 PROFIBUS-DP Master 설정


“[**3.1 산업용 통신 펌웨어 설정**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)" 및 "[**3.2 SYCON.NET 설정**](../../3-settings-industrial-communication/3-2-Settings-SYCON.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.


<br>

##### 1. 산업용 통신 펌웨어 설정에서 PROFIBUS-DP Master를 선택하고 로봇 제어기를 재부팅합니다.

![[그림 3.6.2-1 펌웨어 설정]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

##### 2. 산업용 통신 모니터링에서 선택한 Protocol의 준비 상태를 확인합니다.

![[그림 3.6.2-2 산업용 통신 모니터링]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_2.png>) 

<br>

##### 3. Sycon.net 을 이용하여 PROFIBUS-DP Master PCI 장치를 선택합니다.

![[그림 3.6.2-3 PROFIBUS-DP Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[그림 3.6.2-4 PROFIBUS-DP Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

##### 4. PCI 장치를 Scan 하고 PROFIBUS-DP Master 적용(Apply)합니다.

![[그림 3.6.2-5 Sycon.net Scan]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>


##### 5. 설정을 다운로드 합니다.

![[그림 3.6.2-6 PROFIBUS-DP Master Download]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

##### 6. PROFIBUS-DP Master 에 연결할 Slave 모듈을 준비합니다.
   * 이번 예제에서는 Crevis 사의 GN-9222 PROFIBUS-DP Slave를 사용합니다.
   * 시스템 전원과 필드 전원을 공급해 주어 모듈을 활성화 시켜 주십시오.

![[그림 3.6.2-7 Crevis GN-9222]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_7.png>) 


<br>

##### 7. Slave 장치의 설정

{% hint style="info" %}
\.      PROFIBUS-DP Slave 장치의 Node 번호와 종단을 설정합니다.
{% endhint %}

![[그림 3.6.2-8 Crevis GN-9222]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_8.png>) 


{% hint style="info" %}
\.      종단 : DIP Switch를 사용하여 종단 설정 (예제 : 종단 처리 ON)

\.      Node ID (Station Number) : DIP Switch를 사용하여 설정 (예제 : Node 3번)
{% endhint %}

<br>

##### 8. Slave 장치의 GSD 파일을 등록합니다.

{% hint style="info" %}
\.      Sycon.net에 등록되지 않은 Device를 사용하기 위해 GSD 파일이 필요합니다.

\.      GN-9222 Device의 GSD 파일은 Crevis 홈페이지에서 다운로드 할 수 있습니다.
{% endhint %}

![[그림 3.6.2-9 Crevis GSD File]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      다운로드한 GSD 파일을 Sycon.net 에 등록합니다.

\.      GSD File 등록시 산업용 통신 Protocol (PROFIBUS-DP)를 확인해 주십시오.
{% endhint %}

![[그림 3.6.2-10 Crevis GSD File]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_10.png>)

<br>

![[그림 3.6.5-11 Crevis GSD File]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_11.png>)

![[그림 3.6.5-12 Crevis GSD File]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_12.png>)



<br>

##### 9. Network Scan

{% hint style="warning" %}
\.      **Network Scan 시 아래 사항을 반드시 확인해 주십시오.**

\.      **(1) 케이블 연결 여부**  
\.      **(2) 종단 DIP Switch 사용 여부**  
{% endhint %}

{% hint style="info" %}
\.      PROFIBUS-DP Master 는 Network Scan 기능을 지원합니다.
{% endhint %}

{% hint style="info" %}
\.      PROFIBUS-DP Master 장치에서 우클릭 후 Network Scan을 클릭합니다.
{% endhint %}

![[그림 3.6.2-13 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      GSD 파일이 등록되지 않은 경우 Network Scan을 하면 Slave 정보는 나타나지만 등록은 불가능합니다.
{% endhint %}

{% hint style="info" %}
\.      정상적으로 GSD 파일이 등록된 경우 Network Scan을 통해 Slave 장치를 추가할 수 있습니다.
{% endhint %}

![[그림 3.6.2-14 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

##### 10. Slave 장치 Configuration

{% hint style="info" %}
\.      Slave 장치 Configuration을 위해 Master 장치의 Disconnect를 클릭합니다.
{% endhint %}

![[그림 3.6.2-15 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Slave 장치를 더블클릭합니다.
{% endhint %}

![[그림 3.6.2-16 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      PROFIBUS-DP Slave의 설정을 확인 합니다.

\.      Slot 1 : GN-9222  
\.      Slot 2 : GT-12DF (Input 2 Byte)  
\.      Slot 3 : GT-227F (Output 2 Byte)  
\.      Slot 4 : GT-3154 (Input 8 Byte)  
\.      Slot 5 : GT-4254 (Output 8 Byte)  
{% endhint %}

![[그림 3.6.2-17 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_17.png>)

<br>

![[그림 3.6.2-18 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_18.png>)


<br>

##### 11. Master 장치 Configuration

{% hint style="info" %}
\.      Master 장치를 더블클릭합니다.
{% endhint %}

![[그림 3.6.2-19 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_19.png>)


{% hint style="info" %}
\.      PROFIBUS-DP 통신 속도를 설정합니다.

\.      9.6 ~ 12000 Kbit/s 
{% endhint %}

![[그림 3.6.2-20 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Master 장치에서 Slave 장치의 Slot 정보가 올바른지 확인해주십시오.
{% endhint %}

![[그림 3.6.2-21 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
\.      Address Table에서 각 Slave Slot의 할당된 IO 및 시작 주소를 확인 합니다.
{% endhint %}

![[그림 3.6.2-22 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
\.      Station Table 에서 각 장치가 활성 상태인지 확인합니다.
{% endhint %}

![[그림 3.6.2-23 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      설정을 완료 후 Download를 진행해 주십시오.
{% endhint %}

![[그림 3.6.2-24 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

##### 12. 통신 상태 확인

{% hint style="info" %}
\.        Sycon.net 과 TP 에서 통신 상태를 확인 합니다.

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[**4 산업용 통신 모니터링**](../../4-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      Connected 된 Master 장치를 더블클릭하여 통신 상태를 확인 할 수 있습니다.
{% endhint %}

![[그림 3.6.2-25 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[그림 3.6.2-26 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Sycon.net 의 Diagnosis 기능을 이용하여 통신 상태와 함게 IO 입출력 상태를 모니터링 할 수 있습니다.
{% endhint %}

![[그림 3.6.2-27 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_27.png>)



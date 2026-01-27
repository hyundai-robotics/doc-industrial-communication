## 2.3.3.1 LS ELECTRIC PLC와의 연결

LS ELECTRIC PLC와 EtherNet/IP와의 연결 방법을 설명합니다.  
아래에서 사용되는 PLC와 통신모듈은 다음과 같습니다.  
(PLC : XGI-CPUS, 통신모듈 : XGL-EFMTB)

**1. XG5000 실행**
![xg5000.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/xg5000.png) <br>
*[그림 2.6.1.1 XG5000의 실행]*<br>
XG5000 프로그램의 다운로드 및 자세한 사용방법은 LS ELECTRIC 홈페이지를 참고 하십시오.

**2. EDS File의 등록**
메뉴 > 도구 > EDS(D) > EDS파일 등록 클릭 > “Hi6_EIP_240402.eds” 선택<br>
아래 그림과 같이 EDS 파일 등록 확인<br>
![eds.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/eds.png)<br>
*[그림 2.6.1.2 EDS File의 등록]*<br>


**3. 장치 연결**
[1] 프로젝트 생성<br>
![newProject_1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_1.png)<br>
*[그림 2.6.1.3 새프로젝트 생성]*<br>

[2] 통신 모듈 추가<br>
![newProject_2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_2.png)<br>
*[그림 2.6.1.4 통신 모듈 추가1]*<br>

![newProject_3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_3.png)<br>
*[그림 2.6.1.5 통신 모듈 추가2]*<br>

![newProject_4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_4.png)<br>
*[그림 2.6.1.6 통신 모듈 추가3]*<br>

[3] 통신 모듈의 설정 <br>
아래 그림에서 좌측 탭에 보이는 XGL-EFMT를 더블 클릭<br>
![newProject_6.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_6.png)<br>
*[그림 2.6.1.7 통신 모듈 설정]*<br>
- IP주소, 서브넷마스크, 게이트웨이 등을 설정합니다.  
- PLC의 2개의 LAN Port를 릴레이 기능으로 사용하려면 "Relay" 체크 박스를 선택해 줍니다.  
- RAPIEnet설정은 Disable로 변경합니다.

**4. 온라인 접속 설정**
[1] USB 케이블로 PLC와 연결합니다.<br>
![newProject_7.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_7.png)<br>
*[그림 2.6.1.8 온라인 접속 설정1]*<br>

[2] 아래 그림 좌측에 표시된 버튼을 눌러 전체 설정을 다운로드 합니다.<br>
![newProject_8.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_8.png)<br>
*[그림 2.6.1.9 온라인 접속 설정2]*<br>

**5. 오토 스캔**
[1] 오토 스캔은 PLC와 연결된 상태에서 가능합니다.<br>
현재 온라인 상태가 아니라면 메뉴 > 온라인 > 접속 을 클릭하여 온라인 상태로 변경합니다.<br>

[2] XGL-EFMT 에서 마우스 우측클릭 > 항목 추가 > 스마트 증설 클릭<br>
![auto1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto1.png)<br>
*[그림 2.6.1.10 오토 스캔1]*<br>

[3] Next 클릭  <br>
![auto2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto2.png)<br>
*[그림 2.6.1.11 오토 스캔2]*<br>

[4] 오토 스캔 클릭  <br>
![auto3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto3.png)<br>
*[그림 2.6.1.12 오토 스캔3]*<br>

![auto4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto4.png)<br>
*[그림 2.6.1.13 오토 스캔4]*<br>

[5] 자동 스캔된 장치 확인  
![auto5.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto5.png)<br>
*[그림 2.6.1.14 오토 스캔5]*<br>

![auto6.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto6.png)<br>
*[그림 2.6.1.15 오토 스캔6]*<br>

아래 그림과 같이 Hi6 EtherNet/IP 어댑터 장치가 리스트에 나타납니다.  <br>
![auto7.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto7.png)<br>
*[그림 2.6.1.16 오토 스캔7]*<br>

**6. 프로그램 변수 등록**
[1] 스캔프로그램 > NewProgram > 로컬변수(더블클릭)<br>
![variable1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/variable1.png)<br>
*[그림 2.6.1.17 변수 등록1]*<br>

[2] 통신에서 사용할 Input/Output Data를 설정합니다.<br>
![variable2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/variable2.png)<br>
*[그림 2.6.1.18 변수 등록2]*<br>

**7. EtherNet/IP Adapter 설정**
[1] 좌측 리스트에서 EB01(Hi6 EtherNet/IP 어댑터)를 더블 클릭 합니다.<br>

[2] EIP 상세 설정 버튼을 누릅니다.<br>
![AdapterSetting1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting1.png)<br>
*[그림 2.6.1.19 EtherNet/IP Adapter 설정1]*<br>

[3] 아래 그림을 참고하여 EtherNet/IP 어댑터의 설정값을 선택해 줍니다. <br> 
- 접속 형태
- T2O RPI Range, O2T RPI Range
- T2O Input, O2T Output size
- 송신 주기
- 타임 아웃
- 로컬태크, 리모트태그 <br>
![AdapterSetting2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting2.png) <br>
*[그림 2.6.1.20 EtherNet/IP Adapter 설정2]*<br>

[4] 온라인 > 통신 모듈 설정 및 진단 > 서비스 인에블 클릭<br>
![AdapterSetting3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting3.png)<br>
*[그림 2.6.1.21 EtherNet/IP Adapter 설정3]*<br>

[5] FEnet의 I/O서비스 체크 확인<br>
![AdapterSetting4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting4.png)<br>
*[그림 2.6.1.22 EtherNet/IP Adapter 설정4]*<br>

<br>

**8. 통신 설정 완료 후 IO Block 을 할당**

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[**5. 산업용 통신 IO Block 할당**](../../../5-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
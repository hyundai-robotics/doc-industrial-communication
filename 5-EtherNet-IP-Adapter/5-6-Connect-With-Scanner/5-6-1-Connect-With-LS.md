### 5.6.1 LS ELECTRIC PLC와의 연결

LS ELECTRIC PLC와 Hi6 EtherNet/IP와의 연결 방법을 설명합니다.  
아래에서 사용되는 PLC와 통신모듈은 다음과 같습니다.  
(PLC : XGI-CPUS, 통신모듈 : XGL-EFMTB)

#### 5.6.1.1 XG5000 실행
![[그림 10.1 XG5000]](../../_assets/EIP-ADAPTER/ConnectWithScanner/xg5000.png) <br>
XG5000 프로그램의 다운로드 및 자세한 사용방법은 LS ELECTRIC 홈페이지를 참고 하십시오.

#### 5.6.1.2 EDS File의 등록
메뉴 > 도구 > EDS(D) > EDS파일 등록 클릭 > “Hi6_EIP_240402.eds” 선택<br>
![[그림 10.2 EDS File]](../../_assets/EIP-ADAPTER/ConnectWithScanner/eds.png)<br>
위 그림과 같이 EDS 파일 등록 확인

#### 5.6.1.3 장치 연결
[1] 프로젝트 생성<br>
![[그림 10.3 EDS File]](../../_assets/EIP-ADAPTER/ConnectWithScanner/newProject_1.png)

[2] 통신 모듈 추가<br>
![[그림 10.4 통신 모듈 추가1]](../../_assets/EIP-ADAPTER/ConnectWithScanner/newProject_2.png)<br><br>
![[그림 10.5 통신 모듈 추가2]](../../_assets/EIP-ADAPTER/ConnectWithScanner/newProject_3.png)<br><br>
![[그림 10.6 통신 모듈 추가3]](../../_assets/EIP-ADAPTER/ConnectWithScanner/newProject_4.png)

[3] 통신 모듈의 설정 <br>
아래 그림에서 좌측 탭에 보이는 XGL-EFMT를 더블 클릭<br>
![[그림 10.7 통신 모듈 설정]](../../_assets/EIP-ADAPTER/ConnectWithScanner/newProject_6.png)<br>
- IP주소, 서브넷마스크, 게이트웨이 등을 설정합니다.  
- PLC의 2개의 LAN Port를 릴레이 기능으로 사용하려면 "Relay" 체크 박스를 선택해 줍니다.  
- RAPIEnet설정은 Disable로 변경합니다.

#### 5.6.1.4 온라인 접속 설정
[1] USB 케이블로 PLC와 연결합니다.<br>
![[그림 10.8 온라인 접속 설정1]](../../_assets/EIP-ADAPTER/ConnectWithScanner/newProject_7.png)<br><br>
[2] 아래 그림 좌측에 표시된 버튼을 눌러 전체 설정을 다운로드 합니다.  <br>
![[그림 10.9 온라인 접속 설정2]](../../_assets/EIP-ADAPTER/ConnectWithScanner/newProject_8.png)

#### 5.6.1.5 오토 스캔
[1] 오토 스캔은 PLC와 연결된 상태에서 가능합니다.  <br>
현재 온라인 상태가 아니라면 메뉴 > 온라인 > 접속 을 클릭하여 온라인 상태로 변경합니다.  <br>
[2] XGL-EFMT 에서 마우스 우측클릭 > 항목 추가 > 스마트 증설 클릭<br>
![[그림 10.10 오토 스캔1]](../../_assets/EIP-ADAPTER/ConnectWithScanner/auto1.png) <br>
[3] Next 클릭  <br>
![[그림 10.11 오토 스캔2]](../../_assets/EIP-ADAPTER/ConnectWithScanner/auto2.png)  <br>
[4] 오토 스캔 클릭  <br>
![[그림 10.12 오토 스캔3]](../../_assets/EIP-ADAPTER/ConnectWithScanner/auto3.png)<br><br>
![[그림 10.13 오토 스캔4]](../../_assets/EIP-ADAPTER/ConnectWithScanner/auto4.png) <br><br>
[5] 자동 스캔된 장치 확인  
![[그림 10.14 오토 스캔5]](../../_assets/EIP-ADAPTER/ConnectWithScanner/auto5.png)<br><br>
![[그림 10.15 오토 스캔6]](../../_assets/EIP-ADAPTER/ConnectWithScanner/auto6.png) <br><br> 
아래 그림과 같이 Hi6 EtherNet/IP 어댑터 장치가 리스트에 나타납니다.  <br>
![[그림 10.16 오토 스캔7]](../../_assets/EIP-ADAPTER/ConnectWithScanner/auto7.png)

#### 5.6.1.6 프로그램 변수 등록
[1] 스캔프로그램 > NewProgram > 로컬변수(더블클릭)<br>
![[그림 10.17 변수 등록1]](../../_assets/EIP-ADAPTER/ConnectWithScanner/variable1.png)<br>
[2] 통신에서 사용할 Input/Output Data를 설정합니다.<br>
![[그림 10.18 변수 등록2]](../../_assets/EIP-ADAPTER/ConnectWithScanner/variable2.png)

#### 5.6.1.7 EtherNet/IP Adapter 설정
[1] 좌측 리스트에서 EB01(Hi6 EtherNet/IP 어댑터)를 더블 클릭 합니다.  <br>
[2] EIP 상세 설정 버튼을 누릅니다.  <br>
![[그림 10.19 EtherNet/IP Adapter 설정1]](../../_assets/EIP-ADAPTER/ConnectWithScanner/AdapterSetting1.png)  <br>
[3] 아래 그림을 참고하여 EtherNet/IP 어댑터의 설정값을 선택해 줍니다. <br> 
- 접속 형태
- T2O RPI Range, O2T RPI Range
- T2O Input, O2T Output size
- 송신 주기
- 타임 아웃
- 로컬태크, 리모트태그 <br><br>
![[그림 10.20 EtherNet/IP Adapter 설정2]](../../_assets/EIP-ADAPTER/ConnectWithScanner/AdapterSetting2.png) <br><br>

[4] 온라인 > 통신 모듈 설정 및 진단 > 서비스 인에블 클릭  <br>
![[그림 10.21 EtherNet/IP Adapter 설정3]](../../_assets/EIP-ADAPTER/ConnectWithScanner/AdapterSetting3.png)  <br><br>
[5] FEnet의 I/O서비스 체크 확인  <br>
![[그림 10.22 EtherNet/IP Adapter 설정4]](../../_assets/EIP-ADAPTER/ConnectWithScanner/AdapterSetting4.png)  
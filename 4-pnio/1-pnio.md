
## 4.1 PROFINET ?

 **1. PROFINET**
- PROFINET은 산업 자동화를 위한 이더넷 기반 통신 표준입니다.
- 컨트롤러(PLC, 로봇제어기 등)와 분산 I/O 장치(드라이브, 센서, 모듈 등) 간의 실시간 데이터 교환을 지원합니다.

 **2. PROFINET 사양**
- 디지털 입력 : 50 , 120, 240 bytes (1개 선택) 
- 디지털 출력 : 50 , 120, 240 bytes (1개 선택) 
- 안전 입출력 : 8/8 bytes (활성 or 비활성화) 
- 최소 통신 주기 : 1 msec
- 지원 통신 속도 : 10 or 100 Mbps
- Conformance Class : B
- Netload Class : II
- Optional Feature : Legacy, MRP

 **3. PROFINET 설정 절차**

1) BD671과 PROFINET 컨트롤러 & Hi7 Com의 연결
2) GSDML 파일 등록 (TIA Portal)
3) PROFINET 컨트롤러 설정 (TIA Portal)
4) Hi7 설정 (TP UI)
5) PROFINET 통신의 확인
6) PROFINET I/O 신호의 할당(FB Block Settings)

 **3.1 BD671과 F-Host & Hi7 Com의 연결**

 **3.1.1 랜선 연결**
1) PROFINET 컨트롤러와 BD671를 랜선으로 연결한다.
2) Link LED가 점멸하는지 확인한다.
3) Hi7 COM의 LAN3 커넥터와 BD671를 랜선으로 연결한다.
4) Link LED가 점멸하는지 확인한다.

![](../_assets/4-pnio/profisafe_connect.png)

**3.1.2 Hi7 Com의 연결 설정**
1) 다음과 같이 메뉴를 이동 시스템 -> 제어 파라미터 -> 산업용 통신-> EtherCAT Master 설정
2) 아래와 같이 설정
- EtherCAT Master : ON
- Port : LAN3
3) 슬레이브 리스트에서 "OptionBD - PROFINET_IO"를 선택하고 적용 버튼을 누른다.
4) Hi7 로봇제어기를 재부팅한다.
5) 재부팅후 Run & Communication & Error LED 점등 상태를 확인한다.

![](../_assets/4-pnio/EC_master_setting1.png)
<br> <br>
![](../_assets/4-pnio/EC_master_setting2.png)


**3.2 GSDML 파일 등록 (TIA Portal)**
1) TIA Portal을 실행
2) 메뉴에서 우측과 같이 이동 [Options] → [Manage general station description file (GSD)].
3) "..." 버튼 클릭 후 and GSDML file이 있는 디렉토리를 설정한다.
4) 화면에 표시된 리스트에서 "GSDML-V2.43-Hyundai-Robotics-HI6-20251127.xml"를 선택하고 [Install] 버튼을 누른다.
5) 하드웨어 카탈로그에 새로운 장치로 등록되었는지 확인한다. <br>
![](../_assets/4-pnio/profisafe_gsdmal.png)

**3.3 PROFINET 컨트롤러 설정 (TIA Portal)**
1) TIA Portal을 실행시키고 새 프로젝트를 생성한다.
2) Device & Network 부분을 더블클릭하여 오픈한다.<br>
![](../_assets/4-pnio/profisafe_device_network.png)

3) PROFINET 통신을 지원하는 컨트롤러(예 CPU 1511F-1 PN)를 선택하여 네트워크 뷰쪽으로 끌어다 놓는다.
4) 하드웨어 카탈로그에서 이전 단계에서 추가한 장치(HRC, PROFINET I/O DAP)를 추가하고 네트워크 뷰쪽으로 끌어다 놓는다.
5) 두 장치 그림에서 랜포트를 마우스 드래그&드랍으로 서로 연결한다.<br>
![](../_assets/4-pnio/profisafe_device_network2.png)

6) "Device & Network"화면에서 HRC-IO 장치를 더블 클릭
7) 원하는 슬롯을 선택한다.
8) 오른쪽 카탈로그에서 원하는 모듈을(DI, DO, or PROFIsafe I/O) 드래그하여 "Device Overview window"로 이동시킨다.<br>
![](../_assets/4-pnio/profisafe_device_network3.png)

9) "Device & Network"화면에서 HRC-IO 장치를 더블 클릭
10) HRC-IO장치를 다시 클릭하여 Setting화면을 오픈
11) 아래에서 General 탭으로 이동
12) 왼쪽 메뉴에서 Ethernet addresses 선택
13) "Generate PROFINET device name automatically." 부분 체크 해제
14) "PROFINET device name"을 "hd-hrc-hi7"로 설정하고 저장함.<br>
![](../_assets/4-pnio/profisafe_device_network4.png)

**3.4 Hi7 설정 (TP UI)**
1) PNIO 컨트롤러에서 설정했던 값과 같은 아래의 값으로 파라미터 설정
- PROFINET IO Device Name : hd-hrc-hi7
- Slot 1 : Digital Input : 240
- Slot 2 : Digital Output : 240
- Slot 3 : Safety I/O : No

2) "전체 적용" 버튼을 누른다.<br>
![](../_assets/4-pnio/4_1_profinet_config.png)

**3.5 PROFINET 통신의 확인**
**3.5.1 래더 프로그램 (Tia Portal)**
1) Device Overview 탭 에서, 아래와 같이 래더 프로그램을 만들고 컨트롤러로 다운로드 한다.<br>
![](../_assets/4-pnio/5_1_Safety_Ladder.png)
2) 다운로드 후, Distribution I/O 화면에서 녹색 체크 박스가 표시되었는지 확인한다.<br>
![](../_assets/4-pnio/5_1_Safety_Ladder2.png)

**3.5.2 TP 화면**
메뉴에서 시스템 -> 안전시스템 -> 모니터링 -> PROFINET 상태로 이동한다.<br>
![](../_assets/4-pnio/5_2_pnio_status.png)
- 각 슬롯의 상태 정보를 확인
- Counter가 지속 증가하는지 확인


**3.6 PROFINET I/O 신호의 할당(FB Block Settings)**
1) 시스템 → 제어 파라미터 → 입출력 신호 설정 → FB 블럭 할당으로 이동
2) 2개 이하로 필요한 만큼 블럭 설정을 PROFINET I/O로 변경한다.
 (최대 PROFINET I/O 사이즈는 240바이트이고 개별 FB 블럭의 사이즈는 120바이트 입니다. 따라서 **2개를 초과하는 설정은 무시됩니다.**)<br>
![](../_assets/4-pnio/6_fb_block.png)

3) 추가로 조건 설정 메뉴로 이동하여 PLC 동작 모드가 OFF되어 있는지 확인합니다.<br>
![](../_assets/4-pnio/6_1_condition.png)
4) TIA Portal과 범용 I/O 화면에서 입출력 신호 확인<br>
![](../_assets/4-pnio/6_3_public_io.png)

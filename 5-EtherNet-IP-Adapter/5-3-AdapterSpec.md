## 5.3 EtherNet/IP 어댑터

### 5.3.1 EtherNet/IP 어댑터 사양
|항목|설명|
|------|---|
|장치 타입|General Purpose Discrete I/O (7)|
|Input Assembly Instance|100|
|Output Assembly Instance|112|
|Input Size Range(bytes)|0 - 240|
|Output Size Range(bytes)|0 - 240|
|RPI Range (ms)|5 – 3000|<br>

### 5.3.2 티칭팬던트를 통한 EtherNet/IP 어댑터의 설정 및 모니터링
초기화면에서 “SYSTEM” > “Control Parameter” > “Industrial Communication” > ”Ethernet/IP 어댑터” 로 이동<br>
![[그림 7.2.1 설정]](../_assets/EIP-ADAPTER/Spec/Config.PNG)<br>

**[Network]**
-	Function Enable : 내장형 Ethernet/IP 기능을 사용여부 선택
-	Port Select : Ethernet/IP Scanner와 연결할 LAN Port 선택 (선택된 LAN Port의 정보는 바로 아래 줄에 표시 됨)<br>

**[I/O Size]**
-	Input Bytes : 0 ~ 240 설정 가능
-	Output Bytes : 0 ~ 240 설정 가능<br>

**[Monitoring]**
- Run : Ethernet/IP의 I/O Data 교환의 상태를 나타냄 (On : 정상 통신 중 , Off : 통신 중 아님)
- Ready : Ethernet/IP 어댑터의 초기화 상태를 나타냄 (On : 초기화 정상, Off : 초기화 비정상)
- Error : Ethernet/IP 어댑터의 알람 또는 경고 상태 표시 (On : 알람/경고 상태, Off : 정상)
- Version : Ethernet/IP 어댑터 S/W 버전 정보 표시
- Error Code: 알람 또는 경고가 발생했을 경우 알람/경고 코드 표시 

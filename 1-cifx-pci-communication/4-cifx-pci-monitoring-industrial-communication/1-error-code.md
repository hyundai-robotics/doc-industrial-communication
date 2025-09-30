# 1.4.1 ERROR Code

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>

<br>

<table class="tg">
<thead>
	<tr>
		<th>Error Code</th>
		<th>Description</th>
		<th>Action</th>
	</tr>
</thead>

<tbody>
	<tr>
		<td>0x00000000</td>
		<td>정상</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xC000000C</td>
		<td>제어기와 PCI 사이의 Watchdog 시간 초과</td>
		<td>제어기와 장치의 상태를 확인해 주십시오. 통신 재시작을 통해 리셋할 수 있습니다.</td>
	</tr>
    <tr>
		<td>0xC0000123</td>
		<td>라이선스 없음</td>
		<td>마스터 라이선스의 유무를 확인하십시오</td>
	</tr>
    <tr>
		<td>0xC0000140</td>
		<td>통신 오류</td>
		<td>장치의 상태나 연결 여부를 확인해 주십시오.</td>
	</tr>
    <tr>
		<td>0xC0000141</td>
		<td>연결 끊김</td>
		<td>장치의 상태나 연결 여부를 확인해 주십시오.</td>
	</tr>
    <tr>
		<td>0xC0000142</td>
		<td>연결 대기 시간 초과</td>
		<td>장치의 상태나 연결 여부를 확인해 주십시오..</td>
	</tr>
    <tr>
		<td>0xC0000144</td>
		<td>중복된 IP 주소</td>
		<td>연결된 장치의 IP 주소를 확인하여 중복된 주소를 변경해 주십시오.</td>
	</tr>
    <tr>
		<td>0xC0000145</td>
		<td>케이블 연결 안됨</td>
		<td>통신 케이블의 연결 상태를 확인해 주십시오.</td>
	</tr>
    <tr>
		<td>0xC0000180</td>
		<td>통신 버스 Off 플래그 설정됨 <br> [발생 가능 원인] <br>  - 통신선 CAN High/Low 의 단락 감지 <br>  - 전원 전압 불안정 <br>  - 노이즈 등으로 인한 네트워크 에러 지속 발생</td>
		<td>통신 케이블 접촉 상태나 결선을 확인하고, 장치를 리셋해 주십시오.</td>
	</tr>
    <tr>
		<td>0xC0470298</td>
		<td>DeviceNet 24V 공급 안됨</td>
		<td>DeviceNet 24V 전원을 확인해 주십시오.</td>
	</tr>
	<tr>
		<td>0xC0620023</td>
		<td>DeviceNet Slave bus off 감지 <br> [발생 가능 원인] <br>  - 통신선 CAN High/Low 의 단락 감지 <br>  - 전원 전압 불안정 <br>  - 노이즈 등으로 인한 네트워크 에러 지속 발생</td>
		<td>통신 케이블 접촉 상태나 결선을 확인하고, 장치를 리셋해 주십시오. </td>
	</tr>
    <tr>
		<td>0xC062002C</td>
		<td>DeviceNet Slave 24V 공급 안됨</td>
		<td>DeviceNet 24V 전원을 확인해 주십시오.</td>
	</tr>
</tbody>
</table>


# 1.3.7.1 DeviceNet Master 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>최대 연결 가능한 slave 수</td>
		<td>63개</td>
	</tr>
    <tr>
		<td>최대 입력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>최대 입력 크기 (1 slave)</td>
		<td>255 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기 (1 slave)</td>
		<td>255 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td>Bit Strobe, Change of State, Cyclic, Poll</td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td> - </td>
	</tr>
   <tr>
		<td>통신 속도</td>
		<td>125 ~ 500 Kbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td> - </td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Auto Baudrate Detection</td>
		<td>미지원</td>
	</tr>
</tbody>
</table>
<br>

##### Network 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Data Transport Layer</td>
		<td>CAN Frames</td>
	</tr>
</tbody>
</table>
<br>

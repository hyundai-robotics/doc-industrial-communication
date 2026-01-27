## 1.3.3.1 EtherNet/IP Scanner 사양

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol 특성**

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
		<td>64개</td>
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
		<td>504 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기 (1 slave)</td>
		<td>504 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td>Cyclic</td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td>최소 1ms</td>
	</tr>
    <tr>
		<td>통신 속도</td>
		<td>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Tree, Line, Ring</td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>DLR (Device Level Ring)</td>
		<td>Beacon based 'Ring Node'</td>
	</tr>
    <tr>
		<td>부가 기능</td>
		<td>DHCP, BOOTP, ACD 지원</td>
	</tr>
</tbody>
</table>
<br>

**Network 특성**

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
		<td>Ethernet II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>Interface Type</td>
		<td>10 or 100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>지원</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>사용 가능</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>사용 가능</td>
	</tr>
</tbody>
</table>
<br>

**물리적 연결**

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
		<td>케이블</td>
		<td>최소 Cat5 이상, STP 케이블</td>
	</tr>
	<tr>
		<td>길이</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>

## 1.3.5.3 EtherCAT Slave 사양

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
		<td>최대 입력 크기</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>최대 출력 크기</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>IO 연결</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 업데이트 주기</td>
		<td>최소 250us (1ms 이상 권장)</td>
	</tr>
    <tr>
		<td>통신 속도</td>
		<td>100 Mbit/s (Full-Duplex)</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Line, Ring</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>동기화</td>
		<td>DC (Distributed Clocks)</td>
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
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>Auto-Negotiation</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>사용 불가능</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>제한 사용 가능 (Master와 1번째 Slave 사이)</td>
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

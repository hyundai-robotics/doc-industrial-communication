### 2.3.1 EtherNet/IP 어댑터 사양 (슬레이브)


<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol 특성**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>구분</th>
		<th colspan=2, class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
    <tr>
        <td>Connection</td>
        <td>O (Master) -> T (Slave)</td>
		<td>T (Slave) -> O (Master)</td>
	</tr>
    <tr>
        <td>최대 IO Size</td>
        <td>240 bytes</td>
		<td>240 bytes</td>
	</tr>
    <tr>
        <td>Instance No.</td>
        <td>112 (0x70)</td>
		<td>100 (0x64)</td>
	</tr>
    <tr>
        <td>Real-Time Transfer Format</td>
        <td>32-bit run/idle header</td>
		<td>None</td>
	</tr>
	<tr>
        <td>Connection Type</td>
        <td>Point to Point</td>
		<td>Point to Point</td>
	</tr>
	<tr>
        <td>Priority</td>
        <td>Scheduled</td>
		<td>Scheduled</td>
	</tr>
    <tr>
		<td>IO 최소 Cycle Time (RPI)</td>
		<td colspan=2>5ms</td>
	</tr>
    <tr>
		<td>장치 타입</td>
		<td colspan=2>General Purpose Discrete I/O</td>
	</tr>
    <tr>
		<td>통신 속도</td>
		<td colspan=2>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td colspan=2>미지원</td>
	</tr>
    <tr>
		<td >IP 할당 방식</td>
		<td colspan=2>고정 IP 주소</td>
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
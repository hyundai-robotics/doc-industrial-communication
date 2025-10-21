## 2.3.1 EtherNet/IP 스캐너 사양 (마스터)

<br>

#### 지원 버전 미정

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

##### Protocol 특성

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=2, class='powderblued'>구분</th>
		<th class='powderblued'>사양</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td colspan=2>최대 연결 가능한 slave 수</td>
		<td>20개</td>
	</tr>
    <tr>
		<td rowspan=2>IO Size</td>
        <td>전체 입출력</td>
		<td>Max 1200 bytes</td>
	</tr>
    <tr>
        <td>Slave 장치당 입출력</td>
		<td>Max 240 bytes</td>
	</tr>
    <tr>
		<td colspan=2>IO 연결</td>
		<td>Cyclic</td>
	</tr>
    <tr>
		<td colspan=2>IO 최소 Cycle Time</td>
		<td>5ms</td>
	</tr>
    <tr>
		<td colspan=2>통신 속도</td>
		<td>10 or 100 Mbit/s</td>
	</tr>
    <tr>
		<td colspan=2>Auto Negotiation</td>
		<td>지원</td>
	</tr>
    <tr>
		<td colspan=2>Quick Connect</td>
		<td>미지원</td>
	</tr>
    <tr>
		<td colspan=2>Topology</td>
		<td>Tree, Line</td>
	</tr>
    <tr>
		<td colspan=2>IP 할당 방식</td>
		<td>고정 IP 주소</td>
	</tr>
</tbody>
</table>
<br>
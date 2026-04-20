### 2.4.3 외부 Adapter 장치 연결

<br>

<style type="text/css">
table  {border-collapse:collapse;}
.sm-font-table th, .sm-font-table td {font-size:9px;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**외부 Adapter 장치 연결 시 설정 값**

<br>

{% hint style="info" %}
   - IO size는 외부 장치에 연결된 Input / Output 크기와 일치하게 설정해 주십시오.   
{% endhint %}

<br>

{% hint style="info" %}
   - 자세한 사양은 장치 Maker에서 제공하는 매뉴얼을 참고해주십시오.    
{% endhint %}

<br>

<table class="tg sm-font-table">
<thead>
	<tr>
    	<th rowspan=2, class='powderblued'>Maker</th>
		<th rowspan=2, class='powderblued'>제품</th>
		<th rowspan=2, class='powderblued'>연결 방식</th>
        <th colspan=2, class='powderblued'>T -> O</th>
        <th colspan=2, class='powderblued'>O -> T</th>
        <th colspan=5, class='powderblued'>Additional Configuration</th>
	</tr>
    <tr>
        <th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Run Idle Header</th>
        <th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Run Idle Header</th>
		<th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Total Size</th>
		<th class='powderblued'>Data Size</th>
        <th class='powderblued'>Data Type</th>
		<th class='powderblued'>Data</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Crevis</td>
		<td>M9289</td>
        <td>Exclusive Owner</td>
		<td>1</td>
		<td>No</td>
        <td>2</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Wago</td>
		<td>750-366</td>
        <td>Exclusive Owner</td>
		<td>104: Status + AI + DI<br>105: Status + DI<br>106: Status + AI<br>107: AI + DI<br>108: DI<br>109: AI</td>
		<td>No</td>
        <td>101: AO + DO<br>102: DO<br>103: AO</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Hilscher</td>
		<td>CIFX PCI EtherNet/IP Adapter</td>
        <td>Exclusive Owner</td>
		<td>101</td>
		<td>Yes</td>
        <td>100</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Baumer</td>
		<td>OM-70 EtherNet/IP</td>
        <td>Input Only</td>
		<td>100</td>
		<td>No</td>
        <td>238</td>
		<td>-</td>
		<td colspan=5>-</td>
	</tr>
    <tr>
		<td>Beckhoff</td>
		<td>EK-9500</td>
        <td>Exclusive Owner</td>
		<td>129</td>
		<td>No</td>
        <td>130</td>
		<td>Yes</td>
		<td colspan=5>-</td>
	</tr>
	<tr>
		<td rowspan=6>Rockwell Automation (AB)</td>
		<td rowspan=6>Point I/O 1734-AENTR</td>
        <td rowspan=6>Exclusive Owner</td>
		<td rowspan=6>101</td>
		<td rowspan=6>No</td>
        <td rowspan=6>100</td>
		<td rowspan=6>Yes</td>
		<td rowspan=6>102</td>
		<td rowspan=6>10</td>
		<td>4byte</td>
		<td>unsigned int</td>
		<td>1</td>
	</tr>
	<tr>
		<td>2byte</td>
		<td>unsigned int</td>
		<td>IO slot + 1</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(T -> O) Alignment<br>0: bytes<br>2: word<br>4: Dword<br>255: Fixed</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(T -> O) Fixed Size per Slot</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(O -> T) Alignment<br>0: bytes<br>2: word<br>4: Dword<br>255: Fixed</td>
	</tr>
	<tr>
		<td>1byte</td>
		<td>unsigned int</td>
		<td>(O -> T) Fixed Size per Slot</td>
	</tr>
</tbody>
</table>
<br>
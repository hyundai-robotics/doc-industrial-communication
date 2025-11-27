## 2.3.3 외부 Adapter 장치 연결

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

##### 외부 Adapter 장치 연결 시 설정 값

<br>

{% hint style="info" %}
\.      IO size는 외부 장치에 연결된 Input / Output 크기와 일치하게 설정해 주십시오.   
{% endhint %}

<br>

{% hint style="info" %}
\.      자세한 사양은 장치 Maker에서 제공하는 매뉴얼을 참고해주십시오.    
{% endhint %}

<br>

<table class="tg">
<thead>
	<tr>
    	<th rowspan=2, class='powderblued'>Maker</th>
		<th rowspan=2, class='powderblued'>제품</th>
		<th rowspan=2, class='powderblued'>연결 방식</th>
        <th colspan=2, class='powderblued'>T -> O</th>
        <th colspan=2, class='powderblued'>O -> T</th>
        <th rowspan=2, class='powderblued'>Additional Configuration</th>
	</tr>
    <tr>
        <th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Run Idle Header</th>
        <th class='powderblued'>Instance ID</th>
        <th class='powderblued'>Run Idle Header</th>
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
		<td>-</td>
	</tr>
    <tr>
		<td>Wago</td>
		<td>750-366</td>
        <td>Exclusive Owner</td>
		<td>104: DI + AI + Status<br>105: DI + Status<br>106: AI + Status<br>107: AI + DI<br>108: DI<br>109: AI</td>
		<td>No</td>
        <td>101: AO + DO<br>102: DO<br>103: AO</td>
		<td>Yes</td>
		<td>-</td>
	</tr>
    <tr>
		<td>Hilscher</td>
		<td>CIFX PCI EtherNet/IP Adapter</td>
        <td>Exclusive Owner</td>
		<td>101</td>
		<td>Yes</td>
        <td>100</td>
		<td>Yes</td>
		<td>-</td>
	</tr>
    <tr>
		<td>Baumer</td>
		<td>OM-70 EtherNet/IP</td>
        <td>Input Only</td>
		<td>100</td>
		<td>No</td>
        <td>238</td>
		<td>-</td>
		<td>-</td>
	</tr>
</tbody>
</table>
<br>
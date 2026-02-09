### 2.4.3 Connecting External Adapter Devices

<br>

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Configuration Values for Connecting External Adapter Devices**

<br>

{% hint style="info" %}
   - Please set the IO size to match the Input/Output size configured on the external device.   
{% endhint %}

<br>

{% hint style="info" %}
   - For detailed specifications, please refer to the manual provided by the device manufacturer    
{% endhint %}

<br>

<table class="tg">
<thead>
	<tr>
    	<th rowspan=2, class='powderblued'>Maker</th>
		<th rowspan=2, class='powderblued'>Product</th>
		<th rowspan=2, class='powderblued'>Connection Type</th>
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
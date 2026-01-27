## 1.3.5.1 EtherCAT Master Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Maximum Connectable Slave Count</td>
		<td>200</td>
	</tr>
    <tr>
		<td>Maximum Input Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size</td>
		<td>1200 bytes</td>
	</tr>
    <tr>
		<td>Maximum Input Size (1 slave)</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>Maximum Output Size (1 slave)</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>IO Connection</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO update Cycle</td>
		<td>Min. 250us (1ms Recommended)</td>
	</tr>
    <tr>
		<td>Communication Speed</td>
		<td>100 Mbit/s (Full-duplex)</td>
	</tr>
    <tr>
		<td>Topology</td>
		<td>Line, Ring</td>
	</tr>
    <tr>
		<td>Network Slave Scan</td>
		<td>Supported</td>
	</tr>
    <tr>
		<td>Quick Connect</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Redendance</td>
		<td>Supported (Cannot be applied simultaneously with synchronization)</td>
	</tr>
    <tr>
		<td>Synchronization</td>
		<td>DC (Distributed Clocks)</td>
	</tr>
</tbody>
</table>
<br>

**Network Characteristics**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
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
		<td>Not supported</td>
	</tr>
    <tr>
		<td>Hub</td>
		<td>Forbidden</td>
	</tr>
    <tr>
		<td>Switch</td>
		<td>Only allowed between Master and 1st Slave</td>
	</tr>
</tbody>
</table>
<br>

**Connection**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>Category</th>
		<th class='powderblued'>Specifications</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>Cable</td>
		<td>Minimum of Cat5, STP</td>
	</tr>
	<tr>
		<td>length</td>
		<td>Max. 100m</td>
	</tr>
</tbody>
</table>
<br>
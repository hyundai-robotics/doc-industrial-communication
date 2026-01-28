### 1.4.1 ERROR Code

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
		<td>Normal</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xC000000C</td>
		<td>Watchdog timeout between controller and PCI</td>
		<td>Please check the status of the controller and device. They can be reset by restarting communication.</td>
	</tr>
    <tr>
		<td>0xC0000123</td>
		<td>No license</td>
		<td>Please check if you have a license for master. </td>
	</tr>
    <tr>
		<td>0xC0000140</td>
		<td>Communication error</td>
		<td>Please check the status or connection of the device.</td>
	</tr>
    <tr>
		<td>0xC0000141</td>
		<td>Connection lost</td>
		<td>Please check the status or connection of the device.</td>
	</tr>
    <tr>
		<td>0xC0000142</td>
		<td>Connection waiting timeout</td>
		<td>Please check the status or connection of the device.</td>
	</tr>
    <tr>
		<td>0xC0000144</td>
		<td>Duplicate IP address</td>
		<td>Check the IP addresses of connected devices and change the duplicate addresses.</td>
	</tr>
    <tr>
		<td>0xC0000145</td>
		<td>Cable not connected</td>
		<td>Please check the connection status of the communication cable.</td>
	</tr>
    <tr>
		<td>0xC0000180</td>
		<td>Communication bus off flag set <br> [Possible causes] <br> - CAN High/Low communication line short circuit detected <br> - Unstable power supply voltage <br> - Continuous network errors due to noise, etc.</td>
		<td>Check the contact status or wiring of the communication cable, and reset the device.</td>
	</tr>
    <tr>
		<td>0xC0470298</td>
		<td>DeviceNet 24V not supplied</td>
		<td>Please check the DeviceNet 24V power supply.</td>
	</tr>
	<tr>
		<td>0xC0620023</td>
		<td>DeviceNet slave bus off detected <br> [Possible causes] <br>  - CAN High/Low communication line short circuit detected <br>  - Unstable power supply voltage <br>  - Continuous network errors due to noise, etc.</td>
		<td>Check the contact status or wiring of the communication cable, and reset the device. </td>
	</tr>
    <tr>
		<td>0xC062002C</td>
		<td>DeviceNet slave 24V not supplied</td>
		<td>Please check the DeviceNet 24V power supply.</td>
	</tr>
</tbody>
</table>


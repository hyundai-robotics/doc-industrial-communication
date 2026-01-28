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
		<td>正常</td>
		<td>-</td>
	</tr>
	<tr>
		<td>0xC000000C</td>
		<td>控制器与PCI之间的Watchdog超时</td>
		<td>请确认控制器及设备的状态。可以通过通信重启进行复位。</td>
	</tr>
    <tr>
		<td>0xC0000123</td>
		<td>无许可证</td>
		<td>请确认主许可证是否存在</td>
	</tr>
    <tr>
		<td>0xC0000140</td>
		<td>通信错误</td>
		<td>请确认设备的状态或连接情况。</td>
	</tr>
    <tr>
		<td>0xC0000141</td>
		<td>连接断开</td>
		<td>请确认设备的状态或连接情况。</td>
	</tr>
    <tr>
		<td>0xC0000142</td>
		<td>连接等待超时</td>
		<td>请确认设备的状态或连接情况。</td>
	</tr>
    <tr>
		<td>0xC0000144</td>
		<td>重复的IP地址</td>
		<td>请确认已连接设备的IP地址并更改重复的地址。</td>
	</tr>
    <tr>
		<td>0xC0000145</td>
		<td>电缆未连接</td>
		<td>请确认通信电缆的连接状态。</td>
	</tr>
    <tr>
		<td>0xC0000180</td>
		<td>通信总线Off标志已设置 <br> 【可能发生原因】 <br>  - 检测到通信线CAN High/Low短路 <br>  - 电源电压不稳定 <br>  - 因噪声等原因持续发生网络错误</td>
		<td>请检查通信电缆的接触状态或接线，并复位设备。</td>
	</tr>
    <tr>
		<td>0xC0470298</td>
		<td>DeviceNet 24V未供电</td>
		<td>请确认DeviceNet 24V电源。</td>
	</tr>
	<tr>
		<td>0xC0620023</td>
		<td>检测到DeviceNet Slave bus off <br> [可能发生原因] <br>  - 检测到通信线CAN High/Low短路 <br>  - 电源电压不稳定 <br>  - 因噪声等原因持续发生网络错误</td>
		<td>请检查通信电缆的接触状态或接线，并复位设备。 </td>
	</tr>
    <tr>
		<td>0xC062002C</td>
		<td>DeviceNet Slave 24V未供电</td>
		<td>请确认DeviceNet 24V电源。</td>
	</tr>
</tbody>
</table>


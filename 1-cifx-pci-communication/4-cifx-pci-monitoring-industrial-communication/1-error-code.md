### 1.4.1 错误代码

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
		<th>错误代码</th>
		<th>描述</th>
		<th>操作</th>
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
		<td>控制器和PCI之间的看门狗超时</td>
		<td>请检查控制器和设备的状态。可以通过重新启动通信来重置它们。</td>
	</tr>
    <tr>
		<td>0xC0000123</td>
		<td>无许可证</td>
		<td>请检查您是否拥有主控的许可证。</td>
	</tr>
    <tr>
		<td>0xC0000140</td>
		<td>通信错误</td>
		<td>请检查设备的状态或连接。</td>
	</tr>
    <tr>
		<td>0xC0000141</td>
		<td>连接丢失</td>
		<td>请检查设备的状态或连接。</td>
	</tr>
    <tr>
		<td>0xC0000142</td>
		<td>连接等待超时</td>
		<td>请检查设备的状态或连接。</td>
	</tr>
    <tr>
		<td>0xC0000144</td>
		<td>重复IP地址</td>
		<td>检查连接设备的IP地址并更改重复的地址。</td>
	</tr>
    <tr>
		<td>0xC0000145</td>
		<td>电缆未连接</td>
		<td>请检查通讯电缆的连接状态。</td>
	</tr>
    <tr>
		<td>0xC0000180</td>
		<td>通信总线关闭标志已设置 <br> [可能的原因] <br> - 检测到CAN高/低通信线路短路 <br> - 不稳定的电源电压 <br> - 由于噪声等原因导致的持续网络错误</td>
		<td>检查通信电缆的接触状态或接线，并重置设备。</td>
	</tr>
    <tr>
		<td>0xC0470298</td>
		<td>未提供DeviceNet 24V电源</td>
		<td>请检查DeviceNet 24V电源。</td>
	</tr>
	<tr>
		<td>0xC0620023</td>
		<td>检测到DeviceNet从站总线关闭 <br> [可能的原因] <br>  - 检测到CAN高/低通信线路短路 <br>  - 不稳定的电源电压 <br>  - 由于噪声等原因导致的持续网络错误</td>
		<td>检查通信电缆的接触状态或接线，并重置设备。</td>
	</tr>
    <tr>
		<td>0xC062002C</td>
		<td>未提供DeviceNet 24V电源</td>
		<td>请检查DeviceNet 24V电源。</td>
	</tr>
</tbody>
</table>
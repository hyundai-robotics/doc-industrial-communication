#### 1.3.5.3 EtherCAT从站规范

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td>最大输入大小</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>256 bytes</td>
	</tr>
    <tr>
		<td>IO连接</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO更新周期</td>
		<td>最小250us（推荐1ms）</td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>100 Mbit/s （全双工）</td>
	</tr>
    <tr>
		<td>拓扑</td>
		<td>线型，环型</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>同步</td>
		<td>DC（分布式时钟）</td>
	</tr>
</tbody>
</table>
<br>

**网络特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>数据传输层</td>
		<td>Ethernet II，IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>100 BASE-T Ethernet</td>
	</tr>
    <tr>
		<td>自动协商</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>集线器</td>
		<td>禁止</td>
	</tr>
    <tr>
		<td>交换机</td>
		<td>仅允许在主设备和第一个从设备之间</td>
	</tr>
</tbody>
</table>
<br>

**连接**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>电缆</td>
		<td>至少Cat5，STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最大100m</td>
	</tr>
</tbody>
</table>
<br>
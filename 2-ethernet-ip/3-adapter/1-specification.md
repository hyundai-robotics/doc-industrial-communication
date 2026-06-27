### 2.3.1 EtherNet/IP适配器规格（从设备）

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**协议特性**

<br>
<table class="tg">
<thead>
	<tr>
		<th class='powderblued'>类别</th>
		<th colspan=2, class='powderblued'>规格</th>
	</tr>
</thead>
<tbody>
    <tr>
        <td>连接</td>
        <td>O (主设备) -> T (从设备)</td>
		<td>T (从设备) -> O (主设备)</td>
	</tr>
    <tr>
        <td>最大IO大小</td>
        <td>240字节</td>
		<td>240字节</td>
	</tr>
    <tr>
        <td>实例号</td>
        <td>112 (0x70)</td>
		<td>100 (0x64)</td>
	</tr>
    <tr>
        <td>实时传输格式</td>
        <td>32位运行/空闲头</td>
		<td>无</td>
	</tr>
	<tr>
        <td>连接类型</td>
        <td>点对点</td>
		<td>点对点</td>
	</tr>
	<tr>
        <td>优先级</td>
        <td>计划的</td>
		<td>计划的</td>
	</tr>
    <tr>
		<td>IO循环时间（RPI）</td>
		<td colspan=2>最小5ms</td>
	</tr>
    <tr>
		<td>设备类型</td>
		<td colspan=2>通用离散I/O</td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td colspan=2>10或100 Mbit/s</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td colspan=2>不支持</td>
	</tr>
    <tr>
		<td >IP分配方法</td>
		<td colspan=2>静态IP地址</td>
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
		<td>以太网II，IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>10或100 BASE-T以太网</td>
	</tr>
    <tr>
		<td>自动协商</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>集线器</td>
		<td>允许</td>
	</tr>
    <tr>
		<td>交换机</td>
		<td>允许</td>
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
		<td>最小Cat5，STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最大100m</td>
	</tr>
</tbody>
</table>
<br>
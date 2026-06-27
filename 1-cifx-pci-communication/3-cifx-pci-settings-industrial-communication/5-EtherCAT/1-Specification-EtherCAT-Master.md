#### 1.3.5.1 EtherCAT 主站规格

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
		<td>最大可连接从设备数量</td>
		<td>200</td>
	</tr>
    <tr>
		<td>最大输入大小</td>
		<td>1200 字节</td>
	</tr>
    <tr>
		<td>最大输出大小</td>
		<td>1200 字节</td>
	</tr>
    <tr>
		<td>最大输入大小 (1 个从设备)</td>
		<td>256 字节</td>
	</tr>
    <tr>
		<td>最大输出大小 (1 个从设备)</td>
		<td>256 字节</td>
	</tr>
    <tr>
		<td>IO 连接</td>
		<td> - </td>
	</tr>
    <tr>
		<td>IO 更新周期</td>
		<td>最小 250us (推荐 1ms)</td>
	</tr>
    <tr>
		<td>通信速度</td>
		<td>100 Mbit/s (全双工)</td>
	</tr>
    <tr>
		<td>拓扑</td>
		<td>线，环</td>
	</tr>
    <tr>
		<td>网络从设备扫描</td>
		<td>支持</td>
	</tr>
    <tr>
		<td>快速连接</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td>冗余</td>
		<td>支持（无法与同步同时应用）</td>
	</tr>
    <tr>
		<td>同步</td>
		<td>DC (分布时钟)</td>
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
		<td>以太网 II, IEEE 802.3</td>
	</tr>
	<tr>
		<td>接口类型</td>
		<td>100 BASE-T 以太网</td>
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
		<td>仅允许在主站和第一个从设备之间</td>
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
		<td>至少 Cat5, STP</td>
	</tr>
	<tr>
		<td>长度</td>
		<td>最长 100m</td>
	</tr>
</tbody>
</table>
<br>
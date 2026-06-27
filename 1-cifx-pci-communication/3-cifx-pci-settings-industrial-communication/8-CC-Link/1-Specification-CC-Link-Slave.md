#### 1.3.8.1 CC-Link 从设备规格

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
		<th colspan=3, class='powderblued'>类别</th>
		<th class='powderblued'>规格 (版本 1.11)</th>
		<th class='powderblued'>规格 (版本 2.0)</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td colspan=3>最大输入大小</td>
		<td>48 字节</td>
		<td>368 字节</td>
	</tr>
    <tr>
		<td colspan=3>最大输出大小</td>
		<td>48 字节</td>
		<td>368 字节</td>
	</tr>
    <tr>
		<td rowspan=6>IO 大小</td>
		<td rowspan=2>IO 站</td>
        <td>RY</td>
		<td>4 字节</td>
		<td>不支持</td>
	</tr>
    <tr>
        <td>RX</td>
		<td>4 字节</td>
		<td>不支持</td>
	</tr>
    <tr>
		<td rowspan=4>远程设备</td>
        <td>RY</td>
		<td>16 字节</td>
		<td>112 字节</td>
	</tr>
    <tr>
        <td>RX</td>
		<td>16 字节</td>
		<td>112 字节</td>
	</tr>
    <tr>
        <td>RWw</td>
		<td>32 字节</td>
		<td>256 字节</td>
	</tr>
    <tr>
        <td>RWr</td>
		<td>32 字节</td>
		<td>256 字节</td>
	</tr>
    <tr>
        <td colspan=2, rowspan=2>被占用站</td>
        <td>IO 站</td>
		<td>1</td>
		<td> - </td>
	</tr>
    <tr>
        <td>远程设备</td>
		<td>1 ~ 4</td>
		<td>1 ~ 4</td>
	</tr>
    <tr>
        <td colspan=3>扩展周期</td>
		<td>不支持</td>
		<td>1, 2, 4, 8</td>
	</tr>
   <tr>
		<td colspan=3>通信速度</td>
		<td colspan=2>156 kbit/s ~ 10 Mbit/s</td>
	</tr>
</tbody>
</table>
<br>

**CC-Link IO 映射**

<br>

{% hint style="info" %}
   - CC-Link 版本 1
{% endhint %}

<br>

![[图 1.3.8.1-1 CC-Link IO 映射]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
   - CC-Link 版本 2

   - 扩展周期 : 单
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO 映射]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
   - CC-Link 版本 2

   - 扩展周期 : 双
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO 映射]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
   - CC-Link 版本 2

   - 扩展周期 : 四倍
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO 映射]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
   - CC-Link 版本 2

   - 扩展周期 : 八倍
{% endhint %}

<br>

![[图 1.3.8.1-2 CC-Link IO 映射]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_5.png>)
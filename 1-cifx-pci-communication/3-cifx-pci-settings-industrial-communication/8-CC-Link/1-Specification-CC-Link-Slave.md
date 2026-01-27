## 1.3.8.1 CC-Link Slave Specifications

<style type="text/css">
table  {border-collapse:collapse;}
td {border-color:gray;border-style:solid;border-width:1px;}
.grayed {background-color:lightgray;}
.powderblued {background-color:powderblue;}
</style>
<br>

**Protocol Characteristics**

<br>
<table class="tg">
<thead>
	<tr>
		<th colspan=3, class='powderblued'>Category</th>
		<th class='powderblued'>Specifications (Version 1.11)</th>
		<th class='powderblued'>Specifications (Version 2.0)</th>
	</tr>
</thead>
<tbody>
    <tr>
		<td colspan=3>Maximum Input Size</td>
		<td>48 bytes</td>
		<td>368 bytes</td>
	</tr>
    <tr>
		<td colspan=3>Maximum Output Size</td>
		<td>48 bytes</td>
		<td>368 bytes</td>
	</tr>
    <tr>
		<td rowspan=6>IO Size</td>
		<td rowspan=2>IO Station</td>
        <td>RY</td>
		<td>4 bytes</td>
		<td>Not supported</td>
	</tr>
    <tr>
        <td>RX</td>
		<td>4 bytes</td>
		<td>Not supported</td>
	</tr>
    <tr>
		<td rowspan=4>Remote Device</td>
        <td>RY</td>
		<td>16 bytes</td>
		<td>112 Bytes</td>
	</tr>
    <tr>
        <td>RX</td>
		<td>16 bytes</td>
		<td>112 Bytes</td>
	</tr>
    <tr>
        <td>RWw</td>
		<td>32 bytes</td>
		<td>256 Bytes</td>
	</tr>
    <tr>
        <td>RWr</td>
		<td>32 bytes</td>
		<td>256 Bytes</td>
	</tr>
    <tr>
        <td colspan=2, rowspan=2>Occupied Station</td>
        <td>IO Station</td>
		<td>1</td>
		<td> - </td>
	</tr>
    <tr>
        <td>Remote Device</td>
		<td>1 ~ 4</td>
		<td>1 ~ 4</td>
	</tr>
    <tr>
        <td colspan=3>Extension Cycle</td>
		<td>Not supported</td>
		<td>1, 2, 4, 8</td>
	</tr>
   <tr>
		<td colspan=3>Communication Speed</td>
		<td colspan=2>156 kbit/s ~ 10 Mbit/s</td>
	</tr>
</tbody>
</table>
<br>

**CC-Link IO Mapping**

<br>

{% hint style="info" %}
\.        CC-Link Version 1
{% endhint %}

<br>

![[Figure 1.3.8.1-1 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_1.png>)


<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Single
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_2.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Double
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_3.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle: Quadruple
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_4.png>)

<br>

{% hint style="info" %}
\.        CC-Link Version 2

\.        Extension Cycle : Octuple
{% endhint %}

<br>

![[Figure 1.3.8.1-2 CC-Link IO Mapping]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/3-Slave_spec/image_5.png>)

<br>
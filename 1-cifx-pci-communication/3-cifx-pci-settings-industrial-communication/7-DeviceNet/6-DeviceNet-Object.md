#### 1.3.7.6 DeviceNet Object


<br>

**1. Object**


DeviceNet 的设备内部由 Object 的集合体构成。各 Object 表示设备内部的特定构成要素。

<br>

![[图 1.3.7.6-1 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_1.png>) 


<br>

使用 Class Code 区分 Object。

<br>

![[图 1.3.7.6-2 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_2.png>)

<br>

Object内部由Instance编号和Attribute ID构成。

<br>

DeviceNet Master可以通过Explicit Message访问特定Slave的Object。

<br>

{% hint style="info" %}
   - EX） Crevis GN-9212的Object（该资料可在Crevis说明书中查看。）

   - 读取Identity Object（Class Code 0x01）的Vendor ID值

   - Instance : 1

   - Attribute ID : 1

   - 权限：Get（仅可读取）
{% endhint %}


![[图 1.3.7.6-3 DeviceNet Object Crevis GN-9212]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_3.png>)


<br>

各Object及内部的Instance和Attribute各自都有不同的访问权限。

<br>

{% hint style="info" %}
   - 访问权限

   - Get：读取权限

   - Set：写入权限 

   - Attribute Single：一次只能访问1个Attribute项目。

   - Attribute All：一次可访问Instance内的所有Attribute。
{% endhint %}

<br>
#### 1.3.7.6 DeviceNet 对象


<br>

**1. 对象**


DeviceNet 设备内部由一系列对象组成。每个对象代表设备内部的特定组件。

<br>

![[图 1.3.7.6-1 DeviceNet 对象]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_1.png>) 


<br>

单个对象通过类代码进行区分。

<br>

![[图 1.3.7.6-2 DeviceNet 对象]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_2.png>)

<br>

对象内部由实例编号和属性 ID 组成。

<br>

DeviceNet 主站可以通过显式消息访问特定从站的对象。

<br>

{% hint style="info" %}
   - 例) Crevis GN-9212 的对象（相关信息可以在 Crevis 手册中找到。）

   - 读取身份对象的供应商 ID 值（类代码 0x01）

   - 实例 : 1

   - 属性 ID : 1

   - 权限: 获取（仅可读）
{% endhint %}


![[图 1.3.7.6-3 DeviceNet 对象 Crevis GN-9212]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_3.png>)


<br>

每个对象、实例和属性都有不同的访问权限。

<br>

{% hint style="info" %}
   - 访问权限

   - 获取: 读取权限

   - 设置: 写入权限 

   - 属性单个: 每次只能访问一个属性项。

   - 属性全部: 可以一次性访问实例中的所有属性。
{% endhint %}
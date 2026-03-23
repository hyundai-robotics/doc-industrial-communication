#### 1.3.7.6 DeviceNet 对象


<br>

**1. 对象**


DeviceNet 设备内部由一系列对象组成。每个对象代表设备内部的一个特定组件。

<br>

![[Figure 1.3.7.6-1 DeviceNet 对象]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_1.png>) 


<br>

单独的对象通过类代码区分。

<br>

![[Figure 1.3.7.6-2 DeviceNet 对象]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_2.png>)

<br>

一个对象内部由实例编号和属性 ID 组成。

<br>

DeviceNet 主站可以通过显性消息访问特定从站的对象。

<br>

{% hint style="info" %}
   - EX) Crevis GN-9212 的对象（相应的信息可以在 Crevis 手册中找到。）

   - 读取身份对象的供应商 ID 值（类代码 0x01）

   - 实例 : 1

   - 属性 ID : 1

   - 权限: 获取（仅允许读取）
{% endhint %}


![[Figure 1.3.7.6-3 DeviceNet 对象 Crevis GN-9212]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_3.png>)


<br>

每个对象、实例和属性内部具有不同的访问权限。

<br>

{% hint style="info" %}
   - 访问权限

   - 获取: 读取权限

   - 设置: 写入权限 

   - 属性单个: 一次只能访问一个属性项目。

   - 属性全部: 可以一次访问实例中的所有属性。
{% endhint %}
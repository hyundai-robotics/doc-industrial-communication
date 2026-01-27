## 1.3.7.6 DeviceNet Object


<br>

**1. Object**


The inside of the DeviceNet device is composed of a collection of objects. Each object represents a specific component inside the device.

<br>

![[Figure 1.3.7.6-1 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_1.png>) 


<br>

Individual objects are distinguished using a class code.

<br>

![[Figure 1.3.7.6-2 DeviceNet Object]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_2.png>)

<br>

The inside of an object is composed of an instance number and attribute ID.

<br>

The DeviceNet master can access an object of a specific slave through a explicit message.

<br>

{% hint style="info" %}
\.      EX) Object of Crevis GN-9212 (The corresponding information can be found in the Crevis manual.)

\.      Reading the vendor ID value of the identity object (class code 0x01)

\.      Instance : 1

\.      Attribute ID : 1

\.      Permission: Get (Read only possible)
{% endhint %}


![[Figure 1.3.7.6-3 DeviceNet Object Crevis GN-9212]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/6-Object/image_3.png>)


<br>

Each Object, Instance, and Attribute inside has different access permissions.

<br>

{% hint style="info" %}
\.      Access permissions

\.      Get: Read permission

\.      Set: Write permission 

\.      Attribute Single: Can access only one attribute item at a time.

\.      Attribute All: Can access all attributes in Instance at once.
{% endhint %}

<br>
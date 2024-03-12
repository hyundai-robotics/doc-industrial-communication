# 3.7.6 Object of DeviceNet


<br>

##### 1. Object


The device is Modeled as a collection of objects. Object modeling organizes related data and procedures into one entity : the object.

<br>

![[Figure 3.7.6-1 DeviceNet Object]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/6-Object/image_1.png>) 


<br>

Object is identified by class code.

<br>

![[Figure 3.7.6-2 DeviceNet Object]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/6-Object/image_2.png>)

<br>

Inside the object, it consists of an Instance number and a Attribute ID.

<br>

You can access the Attribute of a specific Instance through the "Explicit Message"  from the DeviceNet Master.

<br>

{% hint style="info" %}
\.      EX) Object of "Crevis GN-9212" (You can check this data through the Company "user manual".)

\.      Identity Object (Class Code 0x01) - Read Vendor ID 

\.      Instance : 1

\.      Attribute ID : 1

\.      Access : Get (Read Only)
{% endhint %}


![[Figure 3.7.6-3 DeviceNet Object Crevis GN-9212]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/6-Object/image_3.png>)


<br>

Each object and its Internal Instance / Attribute have access rights. 

<br>

{% hint style="info" %}
\.      Access

\.      Get : Read

\.      Set : Write

\.      Attribute Single : Only one Attribute can be accessed at a time.

\.      Attribute All : Access all Attributes at once.
{% endhint %}

<br>
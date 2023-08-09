# 3.7.5 Actions for a DeviceNet Error

<br>

Please refer to “[**4.1 Error Code.**](../../4-monitoring-industrial-communication/4-1-error-code.md).”

<br>

##### 1. DeviceNet Terminating Resistance

{% hint style="info" %}
\.      When connecting the cable for DeviceNet, it is necessary to add resistance to the termination.

\.      If the network scan does not work, check the terminating resistance.

\.      DeviceNet terminating resistance: 120 ohms
{% endhint %}

{% hint style="info" %}
\.      As shown in the figure below, if the CIFX-50 DN PCI is the termination of DeviceNet, add terminating resistance.
{% endhint %}

![[Figure 3.7.5-1 DeviceNet Terminating Resistance]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/5-Error/image_1.png>) 

{% hint style="info" %}
\.      As shown in the figure below, if the DeviceNet remote IO is the termination, add terminating resistance or operate the DIP switches.
{% endhint %}

![[Figure 3.7.5-2 DeviceNet Terminating Resistance]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/5-Error/image_2.png>) 

<br>

##### 2. Communication Speed

{% hint style="info" %}
\.      If the communication speeds of the DeviceNet master and slave are different from each other, the network scan may not be performed.

\.      If the network scan does not work, check the communication speed.
{% endhint %}

![[Figure 3.7.5-3 DeviceNet Baudrate]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/5-Error/image_3.png>) 

<br>

##### 3. DeviceNet Error

{% hint style="info" %}
\.      If there is no power supply of 24 V to the cable of DeviceNet, the following error will appear.

\.      Check the power supply of 24 V.
{% endhint %}

![[Figure 3.7.5-4 DeviceNet Error]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/5-Error/image_4.png>) 
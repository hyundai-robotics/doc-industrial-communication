# 3.5.5 Cable Topology of EtherCAT

<br>

For EtherCAT, there are restrictions in cable topology and usable Ethernet ports, which are different from existing industrial communication methods.

##### 1. Ethernet Port

{% hint style="info" %}
\.      When the EtherCAT master needs to be connected to a slave, port 0 should be used.
{% endhint %}

![[Figure 3.5.5-1 EtherCAT Topology]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
\.      When connecting one slave to the master
{% endhint %}

![[Figure 3.5.5-2 EtherCAT Topology]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
\.      When connecting two slaves or more to the master

\.      Connect port 1 of a slave to port 0 of the next slave.
{% endhint %}

![[Figure 3.5.5-3 EtherCAT Topology]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_3.png>) 

<br>

##### 2. Redundancy 

{% hint style="info" %}
\.      When using the redundancy function in the master

\.      The last slave’s port 1 and the master’s port 1 need to be connected to form a ring structure.
{% endhint %}

![[Figure 3.5.5-4 EtherCAT Topology]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_4.png>) 


<br>

##### 3. Cable Topology Error


Please refer to “[**4.1 ERROR Code.**](../../4-monitoring-industrial-communication/4-1-error-code.md)” 

<br>

{% hint style="info" %}
\.     When the network scan function does not work

\.      Check the port and cable connected to the master.
{% endhint %}

![[Figure 3.5.5-5 EtherCAT ERROR]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
\.      Topology Error (error with configuration)

\.      Check the topology of cables connected between the master and slaves.
{% endhint %}

![[Figure 3.5.5-6 EtherCAT ERROR]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
\.      Topology Error 2 (configuration is normal, but diagnosis shows an error)

\.      Check the topology of cables connected between the master and slaves.

\.      Check the topology of cables connected between the slaves.
{% endhint %}

![[Figure 3.5.5-7 EtherCAT ERROR]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_7.png>)

![[Figure 3.5.5-8 EtherCAT ERROR]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
\.      Mandatory Slave Missing Error

\.      Check the topology of cables connected between the slaves.
{% endhint %}

![[Figure 3.5.5-9 EtherCAT ERROR]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/5-Error/image_9.png>)
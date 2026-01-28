#### 1.3.5.5 EtherCAT Cable Wiring (Topology)

<br>

Unlike existing industrial communications, EtherCAT has restrictions in cable wiring and usable Ethernet Ports.

**1. Ethernet Port**

{% hint style="info" %}
\.      When connecting the EtherCAT master and slave, port 0 should be used.
{% endhint %}

![[Figure 1.3.5.5-1 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_1.png>) 

{% hint style="info" %}
\.      When one slave is connected to the master
{% endhint %}

![[Figure 1.3.5.5-2 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_2.png>) 

{% hint style="info" %}
\.      When two or more slaves are connected to the master

\.      Connect from the slave port 1 to the next slave port 0.
{% endhint %}

![[Figure 1.3.5.5-3 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_3.png>)

<br>

**2. Redundancy**

{% hint style="info" %}
\.      When using the Redundancy function in the master 

\.      Connect port 1 of the last slave and port 1 of the master to form a ring structure.
{% endhint %}

![[Figure 1.3.5.5-4 EtherCAT Topology]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_4.png>) 


<br>

**3. Cable wiring error**


Please refer to "[**1.4.1 ERROR Code**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/1-error-code.md)".

<br>

{% hint style="info" %}
\.      If the Network scan function is not working.

\.      Please check the port and cable connected to the master.
{% endhint %}

![[Figure 1.3.5.5-5 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_5.png>)

{% hint style="info" %}
\.      Topology Error (Error in Configuration)

\.      Please check the cable wiring between the master and slave.
{% endhint %}

![[Figure 1.3.5.5-6 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_6.png>)

{% hint style="info" %}
\.      Topology error 2 (normal during configuration but there is an error during diagnosis)

\.      Please check the cable wiring between the master and slave.

\.      Please check the cable wiring between slaves.
{% endhint %}

![[Figure 1.3.5.5-7 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_7.png>)

![[Figure 1.3.5.5-8 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_8.png>)

{% hint style="info" %}
\.      Mandatory Slave Missing Error

\.      Please check the cable wiring between slaves.
{% endhint %}

![[Figure 1.3.5.5-9 EtherCAT ERROR]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/5-Error/image_9.png>)
# 1.4 CIFX PCI Communication Monitoring

<br>

After setting the communication according to the procedures of “[**1.2 CIFX PCI - Installing and Setting Industrial Communication Cards**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)” and “[**1.3 CIFX PCI - Setting Industrial Communication**](../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md),” you can check the operations in the following screens.

<br>

#### 1. Industrial Communication Monitoring

<br>

You can enter the screens by touching **\[Service > 19: Industrial Communication Monitoring]**, and check the details such as the set firmware information, communication status, and communication configuration in relevant screens.

<br>

{% hint style="info" %}
\.      Using the **\[Restart]** button, you can restart the industrial communication of the PCI communication card.

\.      Please check the status of the slot, firmware, and device.

\.      For the master, check whether the number of the configured and active slaves matches the number of configured slaves.
{% endhint %}

<br>

![[Figure 1.4-1 Industrial Communication Monitoring]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_1.png>)

<br>

{% hint style="info" %}
\.      [Status Information]   
\.       Communication: Communication link established and I/O data exchanging   
\.       Run: Communication card (PCI) is operating   
\.       Ready: Communication is in standby state   
\.       Error: Communication error state   

\.       Communication Error: Error code occurred during communication   
\.       Error Count: Accumulated number of communication errors   
\.       Active Slaves: Number of slaves currently connected and exchanging I/O data   
\.       Configured Slaves: Number of slaves configured for communication   
\.       Diag Slave: Number of slaves under communication diagnostics   
\.       Watchdog Time (ms): Timeout value for monitoring communication program activity   
{% endhint %}

<br>

#### 2. Industrial Communication Node Monitoring

<br> 

#### Supported version: TBD 

<br>

Click the Node Statue button at the bottom of the monitoring screen to monitor the status of devices connected to the master protocol

<br>

![[그림 1.4-2 Industrial Communication Monitoring]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_2.png>)

{% hint style="info" %}
\.      [Node Status Information]   
\.       Green: Node currently connected and exchanging I/O data   
\.       Red: Node configured but not connected   
{% endhint %}

<br>

{% hint style="info" %}
\.      In the case of DeviceNet Master, you can monitor by scanning the node information list
{% endhint %}

<br>

![[그림 1.4-3 Industrial Communication Monitoring]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_3.png>)
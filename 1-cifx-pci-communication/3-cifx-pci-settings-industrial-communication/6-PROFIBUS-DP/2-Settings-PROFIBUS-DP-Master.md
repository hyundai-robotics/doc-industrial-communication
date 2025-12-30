# 1.3.6.2 PROFIBUS-DP Master Settings


Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[**1.3.2 SYCON.NET Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
\.      When using SYCON.net, if there are insufficient explanations in the manual, please refer to the ""[**1.3.2 SYCON.NET Help**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" function.
{% endhint %}

<br>

##### 1. Select the PROFIBUS-DP master in the PCI slot settings and reboot the robot controller.

![[Figure 1.3.6.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.

<br>

{% hint style="info" %}
\.        For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.6.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_2.png>)

<br>

##### 3. Select the PROFIBUS-DP master PCI device by using Sycon.net.

![[Figure 1.3.6.2-3 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[Figure 1.3.6.2-4 PROFIBUS-DP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan the PCI device and apply the PROFIBUS-DP master.

![[Figure 1.3.6.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>


##### 5. Download the settings.

![[Figure 1.3.6.2-6 PROFIBUS-DP Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare the slave module to be connected to the PROFIBUS-DP Master.
   * In this example, we use the GN-9222 PROFIBUS-DP slave from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.6.2-7 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_7.png>) 


<br>

##### 7. Set the slave device

{% hint style="info" %}
\.      Set the node number and termination of the PROFIBUS-DP slave device.
{% endhint %}

![[Figure 1.3.6.2-8 Crevis GN-9222]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_8.png>) 


{% hint style="info" %}
\.      Termination: To be set using the DIP switch (Example: Termination processing ON)

\.      Node ID (station number): To be set using the DIP switch (Example: Node 3)
{% endhint %}

<br>

##### 8. Register the slave device GSD file.

{% hint style="info" %}
\.      A GSD file is required to use a device not registered in Sycon.net.

\.      The GSD file for the GN-9222 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.6.2-9 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      Register the downloaded GSD file in Sycon.net.

\.      When registering a GSD file, please check the industrial communication protocol (PROFIBUS-DP).
{% endhint %}

![[Figure 1.3.6.2-10 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.6.5-11 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_11.png>)

![[Figure 1.3.6.5-12 Crevis GSD File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_12.png>)



<br>

##### 9. Network Scan

{% hint style="warning" %}
\.      **When performing the Network Scan function, be sure to check the following.**

\.      **(1) Whether a cable is connected.**  
\.      **(2) Whether a termination DIP switch is used.**  
{% endhint %}

{% hint style="info" %}
\.      PROFIBUS-DP master supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the PROFIBUS-DP master device and click Network Scan.
{% endhint %}

![[Figure 1.3.6.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      If there is no GSD file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

{% hint style="info" %}
\.      If a GSD file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.6.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

##### 10. Configure the slave device

{% hint style="info" %}
\.      Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.6.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 1.3.6.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      Check the PROFIBUS-DP slave settings.

\.      Slot 1 : GN-9222  
\.      Slot 2 : GT-12DF (Input 2 Byte)  
\.      Slot 3 : GT-227F (Output 2 Byte)  
\.      Slot 4 : GT-3154 (Input 8 Byte)  
\.      Slot 5 : GT-4254 (Output 8 Byte)  
{% endhint %}

![[Figure 1.3.6.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_17.png>)

<br>

![[Figure 1.3.6.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_18.png>)


<br>

##### 11. Configure the master device.

{% hint style="info" %}
\.      Double-click the Master device.
{% endhint %}

![[Figure 1.3.6.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_19.png>)


{% hint style="info" %}
\.      Set the PROFIBUS-DP communication speed.

\.      9.6 - 12000 Kbit/s 
{% endhint %}

![[Figure 1.3.6.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Check from the master device if the slot information of the slave device is correct.
{% endhint %}

![[Figure 1.3.6.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.6.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
\.      Check if each device in the station table is in active status.
{% endhint %}

![[Figure 1.3.6.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.6.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

##### 12. Check the communication status.

{% hint style="info" %}
\.        Check the communication status in Sycon.net and TP.

\.        For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
\.      Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.6.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[Figure 1.3.6.2-26 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Using Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.6.2-27 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/6-PROFIBUS-DP/2-Master_setting/image_27.png>)

<br>

##### 13. Assign IO blocks after completing the settings.

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}

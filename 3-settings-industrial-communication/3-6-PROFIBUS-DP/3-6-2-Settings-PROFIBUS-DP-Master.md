# 3.6.2 Setting the PROFIBUS-DP Master


Perform settings according to the procedures of “[**3.1 Setting Industrial Communication Firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” and “[**3.2 Setting SYCON.net**](../../3-settings-industrial-communication/3-2-Settings-SYCON.md)” first and proceed with the following methods.


<br>

##### 1. Select the PROFIBUS-DP master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 3.6.2-1 Firmware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 3.6.2-2 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the PROFIBUS-DP master PCI device using SYCON.net.

![[Figure 3.6.2-3 PROFIBUS-DP Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_3.png>)
![[Figure 3.6.2-4 PROFIBUS-DP Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan a PCI device and apply the PROFIBUS-DP master.

![[Figure 3.6.2-5 Sycon.net Scan]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_5.png>) 

<br>


##### 5. Download the settings.

![[Figure 3.6.2-6 PROFIBUS-DP Master Download]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare a slave module that is to be connected to the PROFIBUS-DP master.
   * In this example, the GN-9222 PROFIBUS-DP slave of Crevis will be used. 
   * Activate the module by supplying the system power and field power.

![[Figure 3.6.2-7 Crevis GN-9222]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_7.png>) 


<br>

##### 7. Set the slave device.

{% hint style="info" %}
\.      Set the node number and termination for the PROFIBUS-DP slave device.
{% endhint %}

![[Figure 3.6.2-8 Crevis GN-9222]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_8.png>) 


{% hint style="info" %}
\.      Termination: Set the termination with the DIP switches (example: turning the termination to the On state).

\.      Node ID (station number): Set the ID with the DIP switches (example: Node 3).
{% endhint %}

<br>

##### 8. Register the general station description (GSD) files of the slave device.

{% hint style="info" %}
\.      GSD files are necessary to use a device that is not registered on SYCON.net.


\.      The GSD files of the GN-9222 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 3.6.2-9 Crevis GSD File]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      Register the downloaded GSD files on SYCON.net.

\.      When registering GSD files, check the industrial communication protocol (PROFIBUS-DP).
{% endhint %}

![[Figure 3.6.2-10 Crevis GSD File]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_10.png>)

<br>

![[Figure 3.6.5-11 Crevis GSD File]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_11.png>)

![[Figure 3.6.5-12 Crevis GSD File]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_12.png>)



<br>

##### 9. Perform a network scan.

{% hint style="warning" %}
\.      **The following items must be checked when performing a network scan.**

\.      **(1) Whether the cable is connected**  
\.      **(2) Whether the terminating DIP switches are used**  
{% endhint %}

{% hint style="info" %}
\.      The PROFIBUS-DP master supports the network scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the PROFIBUS-DP master device and then click the network scan menu.
{% endhint %}

![[Figure 3.6.2-13 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      If there is no registered GSD file, the slave information will appear when a network scan is performed, but registration will not be possible.
{% endhint %}

{% hint style="info" %}
\.      If GSD files are normally registered, slave devices can be added through the network scan function.
{% endhint %}

![[Figure 3.6.2-14 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_14.png>)

<br>

##### 10. Perform a slave device configuration.

{% hint style="info" %}
\.      Click the disconnect button of the master device to perform the configuration of the slave device.
{% endhint %}

![[Figure 3.6.2-15 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 3.6.2-16 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      Check the settings of the PROFIBUS-DP slave.

\.      Slot 1: GN-9222  
\.      Slot 1: GT-12DF (Input 2 bytes)  
\.      Slot 2: GT-227F (Output 2 bytes)  
\.      Slot 3: GT-3154 (Input 8 bytes)  
\.      Slot 4: GT-4254 (Output 8 bytes)  
{% endhint %}

![[Figure 3.6.2-17 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_17.png>)

<br>

![[Figure 3.6.2-18 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_18.png>)


<br>

##### 11. Perform a master device configuration.

{% hint style="info" %}
\.      Double-click the master device.
{% endhint %}

![[Figure 3.6.2-19 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_19.png>)


{% hint style="info" %}
\.      Set the communication speed of PROFIBUS-DP.

\.      9.6–12000 Kbit/s 
{% endhint %}

![[Figure 3.6.2-20 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.     Check the slot information of the slave device in the master.
{% endhint %}

![[Figure 3.6.2-21 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_21.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address of the slave slot in the address table.
{% endhint %}

![[Figure 3.6.2-22 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_22.png>)

{% hint style="info" %}
\.      Check in the station table whether each device is in an activated state.
{% endhint %}

![[Figure 3.6.2-23 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      When the settings are completed, proceed with the download.
{% endhint %}

![[Figure 3.6.2-24 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_24.png>)

<br>

##### 12. Check the communication status.

{% hint style="info" %}
\.        The communication status needs to be checked in SYCON.net and teach pendant.

\.        Please refer to (“[**4 Monitoring Industrial Communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.
{% endhint %}

{% hint style="info" %}
\.      Double-clicking the connected master device will enable you to check the communication status.
{% endhint %}

![[Figure 3.6.2-25 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_25.png>)

![[Figure 3.6.2-26 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Using the diagnosis function of SYCON.net will enable you to monitor the IO’s input and output status along with communication status.
{% endhint %}

![[Figure 3.6.2-27 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.6-PROFIBUS-DP/2-Master_setting/image_27.png>)



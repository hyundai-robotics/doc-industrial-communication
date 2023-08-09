# 3.7.2 Setting the DeviceNet Master

Perform settings according to the procedures of “[**3.1 Setting Industrial Communication Firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” and “[**3.2 Setting SYCON.net**](../../3-settings-industrial-communication/3-2-Settings-SYCON.md)” first and proceed with the following methods.

<br>

{% hint style="info" %}
\.      Refer to the following for the connection of the DeviceNet connector.

\.      (“[**2.2 Connectors**](../../2-mounting-settings-industrial-communication-card/2-2-Connector.md)”)
{% endhint %}

<br>

##### 1. Select the DeviceNet master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 3.7.2-1 Firmware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication.

![[Figure 3.7.2-2 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the DeviceNet master PCI device using SYCON.net.

![[Figure 3.7.2-3 DeviceNet Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_3.png>)
![[Figure 3.7.2-4 DeviceNet Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan a PCI device and apply the DeviceNet master.

![[Figure 3.7.2-5 Sycon.net Scan]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_5.png>) 

<br>

##### 5. Set the communication speed.

{% hint style="warning" %}
\.      If the communication speeds of the master and slaves are different, the network scan will not be performed normally.
{% endhint %}

![[Figure 3.7.2-6 DeviceNet Master Download]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_6.png>) 

<br>

##### 6. Download the settings.

![[Figure 3.7.2-7 DeviceNet Master Download]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_7.png>) 

<br>

##### 7. Prepare a slave module that is to be connected to the DeviceNet master.
   * In this example, the NA-9211 DeviceNet slave of Crevis will be used. 
   * Activate the module by supplying the system power and field power.

![[Figure 3.7.2-8 Crevis NA-9211]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_8.png>) 

<br>

##### 8. Set the slave device.

{% hint style="info" %}
\.      Set the node number and terminating resistance for the DeviceNet slave device.
{% endhint %}

![[Figure 3.7.2-9 Crevis NA-9211]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_9.png>) 

![[Figure 3.7.2-10 Crevis NA-9211]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_10.png>)

{% hint style="info" %}
\.      [Example of setting]

\.      Terminating resistance: Install terminating resistance at the cable for use (the terminating DIP switches in the Off state).

\.      MAC ID (station number): Set it to 4 (only DIP switch 3 in the On state).

\.      Baud Rate: Set it to the Auto state (DIP switches 7 and 8 in the On state).
{% endhint %}

<br>

##### 9. Register the EDS files of the slave device.

{% hint style="info" %}
\.      EDS files are necessary to use a device that is not registered on SYCON.net.

\.      The EDS files of the NA-9211 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 3.7.2-11 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_11.png>)

{% hint style="info" %}
\.      Register the downloaded EDS files on SYCON.net.

\.      When registering EDS files, check the industrial communication protocol (DeviceNet).
{% endhint %}

![[Figure 3.7.2-12 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_12.png>)

<br>

![[Figure 3.7.2-13 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_13.png>)



<br>

##### 10. Perform a network scan.

{% hint style="warning" %}
\.      **The following items must be checked when performing a network scan.**

\.      **(1) Whether the cable is connected**  
\.      **(2) Whether the terminating resistance is connected or the terminating DIP switches are used**  
\.      **(3) Whether the communication speed between the master and slave is set**  

\.      **Must check with (“[**3.7.5 Actions for an DeviceNet error**](../3-7-DeviceNet/3-7-5-Error-DeviceNet.md)”) for smooth communication connection**
{% endhint %}

{% hint style="info" %}
\.      The DeviceNet master supports the network scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the DeviceNet master device and then click the network scan menu.
{% endhint %}

![[Figure 3.7.2-14 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      If there is no registered EDS file, the slave information will appear when a network scan is performed, but registration will not be possible.
{% endhint %}

{% hint style="info" %}
\.      If EDS files are normally registered, slave devices can be added through the network scan function.
{% endhint %}

![[Figure 3.7.2-15 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_15.png>)

![[Figure 3.7.2-16 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_16.png>)

<br>

##### 11. Perform a slave device configuration.

{% hint style="info" %}
\.      Click the disconnect button of the master device to perform the configuration of the slave device.
{% endhint %}

![[Figure 3.7.2-17 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 3.7.2-18 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_18.png>)

{% hint style="info" %}
\.      Check the settings of the DeviceNet slave.

\.      Output: ST-2318 (1 byte)  
\.      Input: ST-1218 (1 byte)  
{% endhint %}

![[Figure 3.7.2-19 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_19.png>)



<br>

##### 12. Perform a master device configuration.

{% hint style="info" %}
\.      Double-click the master device.
{% endhint %}

![[Figure 3.7.2-20 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_20.png>)


{% hint style="info" %}
\.      Set the communication speed of DeviceNet (to be the same as that of the slave). 
{% endhint %}

![[Figure 3.7.2-21 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_21.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address of the slave slot in the address table.
{% endhint %}

![[Figure 3.7.2-22 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_22.png>)

{% hint style="info" %}
\.      Set whether to use the quick connect function.
{% endhint %}

![[Figure 3.7.2-23 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      When the settings are completed, proceed with the download.
{% endhint %}

![[Figure 3.7.2-24 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_24.png>)

<br>

##### 13. Check the communication status.

{% hint style="info" %}
\.        The communication status needs to be checked in SYCON.net and teach pendant.

\.        Please refer to (“[**4 Monitoring industrial communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.
{% endhint %}

{% hint style="info" %}
\.      Double-clicking the connected master device will enable you to check the communication status.
{% endhint %}

![[Figure 3.7.2-25 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_25.png>)

![[Figure 3.7.2-26 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Using the diagnosis function of SYCON.net will enable you to monitor the IO’s input and output status along with the communication status.
{% endhint %}

![[Figure 3.7.2-27 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.7-DeviceNet/2-Master_setting/image_27.png>)


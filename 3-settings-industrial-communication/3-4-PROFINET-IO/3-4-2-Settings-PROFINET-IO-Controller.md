# 3.4.2 Setting a PROFINET IO Controller

Perform settings according to the procedures of “[**3.1 Setting the Industrial Communication Firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” and “[**3.2 Setting SYCON.net**](../../3-settings-industrial-communication/3-2-Settings-SYCON.md)” first and proceed with the following methods.

<br>

##### 1. Select the PROFINET IO master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 3.4.2-1 Firmware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication. 

![[Figure 3.4.2-2 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

##### 3. Select a PROFINET IO controller PCI device using SYCON.net. 

![[Figure 3.4.2-3 PROFINET IO Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_3.png>)
![[Figure 3.4.2-4 PROFINET IO Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan a PCI device and apply the PROFINET IO controller.


![[Figure 3.4.2-5 SYCON.net Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

##### 5. Download the settings.

![[Figure 3.4.2-6 PROFINET IO Controller Download]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare a device (slave) module that is to be connected to the PROFINET IO controller.
   * In this example, the M9287 PROFINET IO device of Crevis will be used. 
   * Activate the module by supplying system power and field power.

![[Figure 3.4.2-7 Crevis M9287]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
\.      How to set the name of the PROFINET IO device using the DIP switch.

\.      M9287-XX: The number set using the DIP switch

\.      In this example, the name was set as M9287-01 using the No. 1 DIP switch.
{% endhint %}

<br>

##### 7. (Example of using a DIP switch) Set the name of the slave device by using the DIP switch.
   * Change only the No. 1 DIP switch to On mode.


![[Figure 3.4.2-8 Crevis M9287 Dip Switch]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      After the DIP switches are set, reboot the device.
{% endhint %}

<br>

##### 8. Register the general station description markup language (GSDML) files of the slave device.

{% hint style="info" %}
\.      GSDML files are necessary to use a device that is not registered to SYCON.net.

\.      The GSDML files of the M9287 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 3.4.2-9 Crevis GSDML File]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
\.      Register the downloaded EDS files on SYCON.net.

\.      When registering the GSDML files, check the industrial communication protocol (PROFINET IO).
{% endhint %}

![[Figure 3.4.2-10 Crevis GSDML File]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_10.png>)![[Figure 3.4.2-11 Crevis GSDML File]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_11.png>)
![[Figure 3.4.2-12 Crevis GSDML File]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_12.png>)

![[Figure 3.4.2-13 Crevis GSDML File]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_13.png>)


<br>

##### 9. Perform a network scan.

{% hint style="info" %}
\.      The PROFINET IO controller supports the network scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the PROFINET IO master device and then click the network scan menu.
{% endhint %}

![[Figure 3.4.2-14 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      If there is no registered GSDML file, the slave information will appear when a network scan is performed, but registration will not be possible.
{% endhint %}

![[Figure 3.4.2-15 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      If the GSDML files are normally registered, slave devices can be added through the network scan function.
{% endhint %}

![[Figure 3.4.2-16 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_16.png>)

![[Figure 3.4.2-17 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_17.png>)

![[Figure 3.4.2-18 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

##### 10. Perform a slave (device) configuration.

{% hint style="info" %}
\.      Click the disconnect button of the master device to perform the configuration of the slave device.
{% endhint %}

![[Figure 3.4.2-19 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 3.4.2-20 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Add a slot connected to M9287 to set a PROFINET IO slave (device).

\.      Slot 1: M7001  
\.      Slot 2: M12DF  
\.      Slot 3: M225F  
{% endhint %}

![[Figure 3.4.2-21 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_21.png>)

![[Figure 3.4.2-22 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

##### 11. Performa a master (controller) device configuration.

{% hint style="info" %}
\.      Double-click the master device.
{% endhint %}

![[Figure 3.4.2-23 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      Set the IP addresses of the master and slave devices.

\.      Set the IP address of the PROFINET IO slave device in the master.

\.      Ensure that the IP addresses of the master and slave devices do not overlap with each other within the same band.
{% endhint %}

![[Figure 3.4.2-24 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_24.png>)

![[Figure 3.4.2-25 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      Check whether the slot information of the slave device is correct in the master device.
{% endhint %}

![[Figure 3.4.2-26 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address of the slave slot in the address table.
{% endhint %}

![[Figure 3.4.2-27 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.      Set the IO communication speed of PROFINET IO. 
{% endhint %}

![[Figure 3.4.2-28 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.      When the settings are completed, proceed with the download.
{% endhint %}

![[Figure 3.4.2-29 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

##### 12. Check the communication status.

{% hint style="info" %}
\.        The communication's status needs to be checked on SYCON.net and the teach pendant.

\.        Refer to (“[**4 Monitoring Industrial Communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.
{% endhint %}

{% hint style="info" %}
\.      Double-clicking the connected master device will enable you to check the communication status.
{% endhint %}

![[Figure 3.4.2-30 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_30.png>)

![[Figure 3.4.2-31 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
\.        Using the diagnosis function of SYCON.net will enable you to monitor the IO's input and output status along with the communication status.
{% endhint %}

![[Figure 3.4.2-32 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/2-Master_setting/image_32.png>)
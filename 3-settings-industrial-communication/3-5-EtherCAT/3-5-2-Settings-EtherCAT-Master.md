# 3.5.2 Setting the EtherCAT Master

Perform settings according to the procedures of “[**3.1 Setting Industrial Communication firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” and “[**3.2 Setting SYCON.net**](../../3-settings-industrial-communication/3-2-Settings-SYCON.md)” first and proceed with the following methods.


<br>

##### 1. Select the EtherCAT master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 3.5.2-1 Firmware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication. 

![[Figure 3.5.2-2  Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the EtherCAT master PCI device using SYCON.net.

![[Figure 3.5.2-3 EtherCAT Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_3.png>)
![[Figure 3.5.2-4 EtherCAT Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan a PCI device and apply the EtherCAT master.

![[Figure 3.5.2-5 SYCON.net Scan]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_5.png>) 

<br>

##### 5. Download the settings.

![[Figure 3.5.2-6 EtherCAT Master Download]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare a slave module that is to be connected to the EtherCAT master.
   * In this example, the M9386 EtherCAT slave of Crevis will be used. 
   * Activate the module by supplying the system power and field power.

![[Figure 3.5.2-7 Crevis M9386]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_7.png>) 

<br>

##### 7. Set the station address of the slave device.

{% hint style="info" %}
\.      The station address of the EtherCAT slave device should be set in the master.
{% endhint %}

<br>

##### 8. Register the extensible markup language (XML) files of the slave device.

{% hint style="info" %}
\.      XML files are necessary to use a device that is not registered on SYCON.net.

\.      The XML files of the M9386 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 3.5.2-8 Crevis XML File]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      Register the downloaded XML files on SYCON.net.

\.      When registering XML files, check the industrial communication protocol (EtherCAT).
{% endhint %}

![[Figure 3.5.2-9 Crevis XML File]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_9.png>)![[Figure 3.5.5-10 Crevis XML File]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_10.png>)
![[Figure 3.5.2-11 Crevis XML File]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_11.png>)

![[Figure 3.5.2-12 Crevis XML File]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_12.png>)


<br>

##### 9. Perform a network scan.

{% hint style="warning" %}
\.      **For EtherCAT, the applicable cable topology and ports are designated.**

\.      **For smooth communication connection, you must check (“[**3.5.5 EtherCAT cable topology.**](../3-5-EtherCAT/3-5-5-EtherCAT-Topology.md)”)**
{% endhint %}

{% hint style="info" %}
\.      The EtherCAT master supports the network scan function.
{% endhint %}

{% hint style="info" %}
\.      Right-click the EtherCAT master device and then click the network scan menu.
{% endhint %}

![[Figure 3.5.2-13 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      If there is no registered XML file, the slave information will appear when a network scan is performed, but registration will not be possible.
{% endhint %}

{% hint style="info" %}
\.      If XML files are normally registered, slave devices can be added through the network scan function.
{% endhint %}

![[Figure 3.5.2-14 Network Scan]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_14.png>)

<br>

##### 10. Perform a slave device configuration.

{% hint style="info" %}
\.      Click the disconnect button of the master device to perform the configuration of the slave device.
{% endhint %}

![[Figure 3.5.2-15 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      Double-click the slave device.
{% endhint %}

![[Figure 3.5.2-16 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      Add a slot connected to M9386 to set an EtherCAT slave.

\.      Slot 1: M7001  
\.      Slot 2: M12DF  
\.      Slot 3: M225F  
{% endhint %}

![[Figure 3.5.2-17 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_17.png>)

![[Figure 3.5.2-18 Slave Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_18.png>)


<br>

##### 11. Perform a master device configuration.

{% hint style="info" %}
\.      Double-click the master device.
{% endhint %}

![[Figure 3.5.2-19 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      Synchronization: To choose between Freerun and Distributed Clocks (DC)

\.      Redundancy: Whether to use redundancy (cannot be used together with Distributed Clocks)

\.      Bus Cycle Time: Can support at least 250 us (1 ms or above is recommended)
{% endhint %}

<br>

{% hint style="info" %}
\.      The station address of each slave can be set.
{% endhint %}

![[Figure 3.5.2-20 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      Check the assigned IO and start address of the slave slot in the address table.
{% endhint %}

![[Figure 3.5.2-21 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_21.png>)


{% hint style="info" %}
\.      When the settings are completed, proceed with the download.
{% endhint %}

![[Figure 3.5.2-22 Master Configuration]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_22.png>)

<br>

##### 12. Check the communication status.

{% hint style="info" %}
\.        The communication status needs to be checked in SYCON.net and teach pendant.

\.        Please refer to (“[**4 Monitoring Industrial Communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.
{% endhint %}

{% hint style="info" %}
\.      Double-clicking the connected master device will enable you to check the communication status.
{% endhint %}

![[Figure 3.5.2-23 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_23.png>)

![[Figure 3.5.2-24 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.        Using the diagnosis function of SYCON.net will enable you to monitor the IO’s input and output status along with communication status.
{% endhint %}

![[Figure 3.5.2-25 Status Diagnosis]](<../../_assets/3-Settings-Industrial-Communication/3.5-EtherCAT/2-Master_setting/image_25.png>)

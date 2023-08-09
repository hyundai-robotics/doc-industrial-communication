# 3.3.2 Setting an EtherNet/IP Scanner

Perform settings according to the procedures of “[**3.1 Setting Industrial Communication Firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” and “[**3.2 Setting SYCON.net**](../../3-settings-industrial-communication/3-2-Settings-SYCON.md)” first and proceed with the following methods.


<br>

##### 1. Select the EtherNet/IP master in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 3.3.2-1 Firmware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication. 

![[Figure 3.3.2-2 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

##### 3. Select the EtherNet/IP scanner PCI device using SYCON.net. 

![[Figure 3.3.2-3 EtherNet/IP Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_3.png>)
![[Figure 3.3.2-4 EtherNet/IP Master PCI]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

##### 4. Scan a PCI device and apply the EtherNet/IP scanner.

![[Figure 3.3.2-5 SYCON.net Scan]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

##### 5. Download the settings.

![[Figure 3.3.2-6 EtherNet/IP Scanner Download]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

##### 6. Prepare an adapter (slave) module that is to be connected to the EtherNet/IP scanner.
   * In this example, the M9289 EtherNet/IP adapter of Crevis will be used. 
   * Activate the module by supplying system power and field power.

![[Figure 3.3.2-7 Crevis M9289]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

##### 7. Set the IP address of the adapter (slave) for EtherNet/IP communication connection.

{% hint style="info" %}
\.      Set an IP address by using the DIP switches.
{% endhint %}

![[Figure 3.3.2-8 Crevis M9289 Dip Swicth]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
\.      How to set an IP address using BootpSvr.exe.
{% endhint %}

<br>

##### 8. (Example of Bootp) Set the IP address of the slave device using Bootp.
   * Change the No. 9 DIP switch to the On state.

![[Figure 3.3.2-9 Crevis M9289 Dip Swicth]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_9.png>)

   * Connect the PC to the M9289 adapter's LAN port.

![[Figure 3.3.2-10 Crevis M9289 LAN Port]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

##### 9. Run BootpSvr.exe on the PC.
   * The program is provided by Crevis (download IO Guide Pro from the website and install it)

![[Figure 3.3.2-11 Crevis IO Guide Pro]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_11.png>)

![[Figure 3.3.2-12 Crevis Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
\.      While pressing Start Bootp, disconnect the power of the M9289 module and apply the power again to reboot.
{% endhint %}

![[Figure 3.3.2-13 Crevis Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

##### 10. When the adapter device reboots, the device's information will appear in the BootpSvr.exe program.

![[Figure 3.3.2-14 Crevis Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

##### 11. Select a device and set an IP.

![[Figure 3.3.2-15 Crevis Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_15.png>)![[Figure 3.3.2-16 Crevis Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

##### 12. Change all DIP switches of the adapter, where the IP settings are completed, to the Off state, then reboot the device.

{% hint style="info" %}
\.      The status of the DIP switches and whether the adapter has rebooted must be checked.
{% endhint %}

![[Figure 3.3.2-17 Crevis DIP Switch]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

##### 13. Register the electronic data sheet (EDS) files of the slave device.

{% hint style="info" %}
\.      EDS files are required to use a device that is not registered at SYCON.net.

\.     The EDS files of the M9289 adapter can be downloaded from the Crevis website.
{% endhint %}

![[Figure 3.3.2-18 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
\.      Register the downloaded EDS files on SYCON.net.

\.     When registering the EDS files, check the industrial communication protocol (EtherNet/IP.)
{% endhint %}

![[Figure 3.3.2-19 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_19.png>)![[Figure 3.3.2-20 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_20.png>)
![[Figure 3.3.2-21 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_21.png>)

![[Figure 3.3.2-22 Crevis EDS File]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

##### 14. Perform a network scan.

{% hint style="info" %}
\.      The EtherNet/IP scanner does not support the network scan function.
{% endhint %}

<br>

##### 15. Perform a slave (adapter) device configuration.

{% hint style="info" %}
\.      Import the registered device and place it on the EtherNet/IP master's bus line.
{% endhint %}

![[Figure 3.3.2-23 Sycon.net Bus]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
\.      Double-click the relevant device (adapter) to proceed to the settings.

\.      Set the input/output byte count appropriately for the IO devices mounted on the relevant device.

\.      In this example, the settings are as follows:
{% endhint %}

{% hint style="info" %}
\.        O -> T: Originator (Master) -> Target (Slave)

\.        Output: EtherNet/IP Scanner (OUT) -> M9289 (INPUT Module M225F): 2 bytes
{% endhint %}

![[Figure 3.3.2-24 Adapter Device Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.        T -> O: Target (Slave) -> Originator (Master)

\.        Input: M9289 (OUTPUT Module M12DF) -> EtherNet/IP Scanner (IN)

\.        **System status (default) 1 byte + M12DF 2 bytes => 3 bytes**
{% endhint %}

![[Figure 3.3.2-25 Adapter Device Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_25.png>)

<br>

##### 16. Perform a master (scanner) device configuration.
    

{% hint style="info" %}
\.        Right-click the master device to disconnect it.
{% endhint %}

![[Figure 3.3.2-26 Adapter Device Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
\.        Double-click the master device. 

\.        Set the IP address of the master device.
{% endhint %}

![[Figure 3.3.2-27 Adapter Device Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
\.        Set the IP address of the slave device.
{% endhint %}

![[Figure 3.3.2-28 Scanner Device Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
\.        Set the scan time of the slave device.

\.        Set an appropriate communication speed by adjusting the relevant value.
{% endhint %}

![[Figure 3.3.2-29 Scanner Device Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.        Check the settings of the slave device in the address table.

\.        Check the input/output IO byte count and the start address.
{% endhint %}

![[Figure 3.3.2-30 Scanner Device Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
\.        [Quick Connect]

\.        EtherNet/IP supports the quick connect function.  
{% endhint %}

{% hint style="info" %}
\.        The following conditions should be met to use the quick connect function.

\.        (1) Products that support the master and slave quick connect function are necessary.  
\.        (2) The quick connect function cannot be used when using the auto negotiation function.  
\.        (3) The quick connect function cannot be used when using the auto MDI-X function.  
\.        (4) 100 Mbit/s and full duplex should be made available.  
{% endhint %}

{% hint style="info" %}
\.        When the settings are established, proceed the download.
{% endhint %}

![[Figure 3.3.2-31 Scanner Device Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

##### 17. Check the communication status. 

{% hint style="info" %}
\.        The communications status should be checked in SYCON.net and the teach pendant.

\.        Refer to (“[**4 Monitoring Industrial Communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communication status in the teach pendant.
{% endhint %}

{% hint style="info" %}
\.      Double-clicking the connected master device will allow you to check the communication status.
{% endhint %}

![[Figure 3.3.2-32 Communication State]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_32.png>)

![[Figure 3.3.2-33 Communication State]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
\.        Using the diagnosis function of SYCON.net will allow you to monitor the IO's input and output status along with the communication status.
{% endhint %}

![[Figure 3.3.2-34 Communication State]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/2-Master_setting/image_34.png>)
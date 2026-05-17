#### 1.3.3.2 EtherNet/IP Scanner Settings

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[1.3.2 SYCON.NET Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - When using SYCON.net, if there are insufficient explanations in the manual, please refer to the "[1.3.2 SYCON.NET Help](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" function.
{% endhint %}

<br>

**1. Select EtherNet/IP Master in the PCI slot settings and reboot the robot controller.**

![[Figure 1.3.3.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_1.png>)

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.3.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_2.png>) 

<br>

**3. Select the EtherNet/IP scanner PCI device by using Sycon.net.**

![[Figure 1.3.3.2-3 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_3.png>)
![[Figure 1.3.3.2-4 EtherNet/IP Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_4.png>) 

<br>

**4. Scan the PCI device and apply the EtherNet/IP scanner.**

![[Figure 1.3.3.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_5.png>) 

<br>

**5. Download the settings.**

![[Figure 1.3.3.2-6 EtherNet/IP Scanner Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_6.png>) 

<br>

**6. Prepare the adapter (slave) module to be connected to the EtherNet/IP scanner.**
   * In this example, we use the M9289 EtherNet/IP adapter from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.3.2-7 Crevis M9289]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_7.png>) 

<br>

**7. Set the IP address of the adapter (slave) for EtherNet/IP communication connection.**

{% hint style="info" %}
   - Setting an IP address using the dip switch.
{% endhint %}

![[Figure 1.3.3.2-8 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_8.png>) 

{% hint style="info" %}
   - How to set an IP address using BootpSvr.exe
{% endhint %}

<br>

**8. (Bootp example) Set the slave device IP address using Bootp.**
   * Change only DIP switch 9 to ON.

![[Figure 1.3.3.2-9 Crevis M9289 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_9.png>)

   * Connect the PC to the M9289 adapter LAN port.

![[Figure 1.3.3.2-10 Crevis M9289 LAN Port]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_10.png>)

<br>

**9. Execute BootpSvr.exe on the PC.**
   * This program is provided by Crevis. (Download and install IO Guide Pro from the website.)

![[Figure 1.3.3.2-11 Crevis IO Guide Pro]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_11.png>)

![[Figure 1.3.3.2-12 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_12.png>)

{% hint style="info" %}
   - With Start BootP being pressed, disconnect and reapply power to the M9289 module to reboot it.
{% endhint %}

![[Figure 1.3.3.2-13 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_13.png>)

<br>

**10. When the adapter device is rebooted, the device information will appear in the BootpSvr.exe program.**

![[Figure 1.3.3.2-14 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_14.png>)

<br>

**11. Select the device and set the IP.**

![[Figure 1.3.3.2-15 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_15.png>)![[Figure 1.3.3.2-16 Crevis Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_16.png>)

<br>

**12. After setting the IP, turn all DIP switches of the adapter to OFF and reboot the device.**

{% hint style="info" %}
   - Be sure to check the DIP switch status and whether the adapter is rebooted.
{% endhint %}

![[Figure 1.3.3.2-17 Crevis DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_17.png>)

<br>

**13. Register the slave device EDS file.**

{% hint style="info" %}
   - An EDS file is required to use a device not registered in Sycon.net.

   - The EDS file for M9289 adapter can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.3.2-18 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_18.png>)

{% hint style="info" %}
   - Register the downloaded EDS file in Sycon.net.

   - When registering an EDS file, please check the industrial communication protocol (EtherNet/IP).
{% endhint %}

![[Figure 1.3.3.2-19 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_19.png>)![[Figure 1.3.3.2-20 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_20.png>)
![[Figure 1.3.3.2-21 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_21.png>)

![[Figure 1.3.3.2-22 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_22.png>)

<br>

**14. Network Scan**

{% hint style="info" %}
   - The EtherNet/IP scanner does not support the Network Scan function.
{% endhint %}

<br>

**15. Configure the slave (adapter) device**

{% hint style="info" %}
   - Drag the registered device and place it on the EtherNet/IP master bus line.
{% endhint %}

![[Figure 1.3.3.2-23 Sycon.net Bus]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - Double-click the device (adapter) to proceed with settings.

   - Set the input/output byte count appropriate for the IO device installed in that device.

   - In this example, settings were made as follows.
{% endhint %}

<br>

![[Figure 1.3.3.2-24 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - O -> T : Originator(Master) -> Target (Slave)

   - Output : EtherNet/IP Scanner  -> M9289

   [Output Module]   
      (1) M225F (2Bytes)   
      **=> 2Bytes**   
{% endhint %}

<br>

![[Figure 1.3.3.2-25 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - T -> O : Target (Slave) -> Originator(Master)

   - Input : M9289 -> EtherNet/IP Scanner

   [Input Module]
      (1) M7001  (1Byte)
      (2) M12DF  (2Bytes)
      **=> 3Bytes**


      (1) M7002 (0Byte)
      (2) M12DF (2Bytes)
      **=> 2Bytes**  
{% endhint %}

<br>

**16. Configure the master (scanner) device.**


{% hint style="info" %}
   - Right-click the master device to disconnect it.
{% endhint %}

![[Figure 1.3.3.2-26 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - Double-click the master device.

   - Set the master device IP address. 
{% endhint %}

![[Figure 1.3.3.2-27 Adapter Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - Set the slave device IP address.
{% endhint %}

![[Figure 1.3.3.2-28 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - Set the slave device scan time. 

   - Please adjust the corresponding values to set an appropriate communication speed.
{% endhint %}

![[Figure 1.3.3.2-29 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_29.png>)

{% hint style="info" %}
   - Check the slave device settings in the address table.

   - Check the input/output IO byte count and start address.
{% endhint %}

![[Figure 1.3.3.2-30 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_30.png>)

{% hint style="info" %}
   [Quick Connect]

   - EtherNet/IP supports the Quick Connect function.
{% endhint %}

{% hint style="info" %}
   - The following conditions should be met to use the Quick Connect function.

      (1) Products that support the Quick Connection function for the master and slaves are required  
      (2) Quick Connect cannot be used when using Auto Negotiation  
      (3) Quick Connect cannot be used when using Auto MDI-X  
      (4) 100 Mbit/s, Full Duplex required  
{% endhint %}

{% hint style="info" %}
   - After completing the settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.3.2-31 Scanner Device Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_31.png>)

<br>

**17. Check the communication status**

{% hint style="info" %}
   - Check the communication status in Sycon.net and TP.

   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
   - Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.3.2-32 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_32.png>)

![[Figure 1.3.3.2-33 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_33.png>)


{% hint style="info" %}
   - Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.3.2-34 Communication State]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/2-Master_setting/image_34.png>)

<br>

**18. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)").**
{% endhint %}
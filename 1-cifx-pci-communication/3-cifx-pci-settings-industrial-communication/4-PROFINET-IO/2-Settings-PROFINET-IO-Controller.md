#### 1.3.4.2 PROFINET IO Controller Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[**1.3.2 SYCON.NET Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - When using SYCON.net, if there are insufficient explanations in the manual, please refer to the ""[**1.3.2 SYCON.NET Help**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" function.
{% endhint %}

<br>

**1. Select the PROFINET IO master in the PCI slot settings and reboot the robot controller.**

![[Figure 1.3.4.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_1.png>) 

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.4.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_2.png>) 

<br>

**3. Select the PROFINET IO controller PCI device by using Sycon.net.**

![[Figure 1.3.4.2-3 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_3.png>)
![[Figure 1.3.4.2-4 PROFINET IO Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_4.png>) 

<br>

**4. Scan the PCI device and apply the PROFINET IO controller.**

![[Figure 1.3.4.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_5.png>) 

<br>

**5. Download the settings.**

![[Figure 1.3.4.2-6 PROFINET IO Controller Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_6.png>) 

<br>

**6. Prepare the device (slave) module to be connected to the PROFINET IO controller.**
   * In this example, we use the M9287 PROFINET IO device from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.4.2-7 Crevis M9287]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_7.png>) 

<br>

{% hint style="info" %}
   - How to set the PROFINET IO device name using the DIP switch

   - M9287-XX: Number set using the DIP switch

   - In this example, the name was set to M9287-01 using DIP switch 1.
{% endhint %}

<br>

**7. (DIP switch use example) Set the slave device name using the DIP Switch.**
   * Change only DIP Switch 1 to ON.


![[Figure 1.3.4.2-8 Crevis M9287 Dip Swicth]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_8.png>)

{% hint style="info" %}
   - Please reboot the device after setting the DIP switch.
{% endhint %}

<br>

**8. Register the slave device GSDML file.**

{% hint style="info" %}
   - A GSDML file is required to use a device not registered in Sycon.net.

   - The GSDML file for the M9287 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.4.2-9 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_9.png>)

{% hint style="info" %}
   - Register the downloaded GSDML file in Sycon.net.

   - When registering a GSDML file, please check the industrial communication Protocol (PROFINET IO).
{% endhint %}

![[Figure 1.3.4.2-10 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_10.png>)![[Figure 1.3.4.2-11 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_11.png>)
![[Figure 1.3.4.2-12 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_12.png>)

![[Figure 1.3.4.2-13 Crevis GSDML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_13.png>)


<br>

**9. Network Scan**

{% hint style="info" %}
   - The PROFINET IO controller supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
   - Right-click the PROFINET IO master device and click Network Scan.
{% endhint %}

![[Figure 1.3.4.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_14.png>)

{% hint style="warning" %}
   - If there is no GSDML file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

![[Figure 1.3.4.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - If a GSDML file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.4.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_16.png>)

![[Figure 1.3.4.2-17 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_17.png>)

![[Figure 1.3.4.2-18 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_18.png>)

<br>

**10. Configure the slave (device).**

{% hint style="info" %}
   - Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.4.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - Double-click the slave device.
{% endhint %}

![[Figure 1.3.4.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - Add a slot connected to M9287 to set the PROFINET IO slave (device).

   - Slot 1 : M7001  
   - Slot 2 : M12DF  
   - Slot 3 : M225F  
{% endhint %}

![[Figure 1.3.4.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_21.png>)

![[Figure 1.3.4.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_22.png>)

<br>

**11. Configure the master (controller) device**

{% hint style="info" %}
   - Double-click the Master device.
{% endhint %}

![[Figure 1.3.4.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_23.png>)

{% hint style="info" %}
   - Set the IP addresses of the master and slave devices.

   - The slave IP address of the PROFINET IO Device is to be set from the master.

   - Please ensure that the IP addresses of the master and slave do not overlap within the same band.
{% endhint %}

![[Figure 1.3.4.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_24.png>)

![[Figure 1.3.4.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - Check from the master device if the slot information of the slave device is correct.
{% endhint %}

![[Figure 1.3.4.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_26.png>)

{% hint style="info" %}
   - Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.4.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_27.png>)

{% hint style="info" %}
   - Set the IO communication speed for the PROFINET IO.
{% endhint %}

![[Figure 1.3.4.2-28 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_28.png>)

{% hint style="info" %}
   - After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.4.2-29 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_29.png>)

<br>

**12. Check the communication status.**

{% hint style="info" %}
   - Check the communication status in Sycon.net and TP.

   - For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
   - Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.4.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_30.png>)

![[Figure 1.3.4.2-31 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_31.png>)

{% hint style="info" %}
   - Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.4.2-32 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/2-Master_setting/image_32.png>)

<br>

**13. Assign IO blocks after completing the settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}
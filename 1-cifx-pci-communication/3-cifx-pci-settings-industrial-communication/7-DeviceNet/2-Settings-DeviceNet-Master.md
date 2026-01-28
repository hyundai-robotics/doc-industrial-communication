#### 1.3.7.2 DeviceNet Master Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[**1.3.2 SYCON.NET Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - When using SYCON.net, if there are insufficient explanations in the manual, please refer to the ""[**1.3.2 SYCON.NET Help**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" function.
{% endhint %}

<br>

{% hint style="info" %}
   - For DeviceNet connector connection, please refer to the following.

      ("[**1.2.2 Connector**](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)")
{% endhint %}

<br>

**1. Select the DeviceNet master in the PCI slot settings and reboot the robot controller.**

![[Figure 1.3.7.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_1.png>)

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.7.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_2.png>) 

<br>

**3. Select the DeviceNet master PCI device by using Sycon.net.**

![[Figure 1.3.7.2-3 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_3.png>)
![[Figure 1.3.7.2-4 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_4.png>) 

<br>

**4. Scan the PCI device and apply the DeviceNet master.**

![[Figure 1.3.7.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_5.png>) 

<br>

**5. Set the communication speed.**

{% hint style="warning" %}
   - If the communication speed differs between the master and the slave, the Network Scan function does not work normally.
{% endhint %}

![[Figure 1.3.7.2-6 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_6.png>) 

<br>

**6. Download the settings.**

![[Figure 1.3.7.2-7 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_7.png>) 

<br>

**7. Prepare the slave module to be connected to the DeviceNet master.**
   * In this example, we use the NA-9211 DeviceNet slave from Crevis.
   * Please supply the system power and field power to activate the module.

![[Figure 1.3.7.2-8 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_8.png>) 

<br>

**8. Set the slave device.**

{% hint style="info" %}
   - Set the MAC ID, communication speed, and termination resistor of the DeviceNet slave device.
{% endhint %}

![[Figure 1.3.7.2-9 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_9.png>) 

![[Figure 1.3.7.2-10 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_10.png>)

{% hint style="info" %}
   [Example Settings]

   - Termination resistor: Used by being installed in the cable (termination DIP switch OFF)

   - MAC ID (station number): Set to 4 (Only DIP switch 3 is ON.)

   - Communication speed (baudrate): Set to Auto (DIP switches 7 and 8 are ON.)
{% endhint %}

<br>

**9. Register the slave device EDS file.**

{% hint style="info" %}
   - An EDS file is required to use a device not registered in Sycon.net.

   - The EDS file for NA-9211 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.7.2-11 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_11.png>)

{% hint style="info" %}
   - Register all downloaded EDS files in Sycon.net.

   - When registering an EDS file, please check the industrial communication protocol (DeviceNet).
{% endhint %}

![[Figure 1.3.7.2-12 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_12.png>)

<br>

![[Figure 1.3.7.5-13 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_13.png>)



<br>

**10. Network Scan**

{% hint style="warning" %}
   **When performing the Network Scan function, be sure to check the following.**

   **(1) Whether a cable is connected.**  
   **(2) Whether a termination resistor is connected or a termination DIP switch is used.**  
   **(3) Whether the master - slave communication speed is set.**  

   **For smooth communication connection, be sure to check ("[**1.3.7.5 DeviceNet ERROR Handling**](../7-DeviceNet/5-Error-DeviceNet.md)").**
{% endhint %}

{% hint style="info" %}
   - The DeviceNet master supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
   - Right-click the DeviceNet master device and click Network Scan.
{% endhint %}

![[Figure 1.3.7.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
   - If there is no EDS file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

{% hint style="info" %}
   - If an EDS file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.7.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_15.png>)

![[Figure 1.3.7.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_16.png>)

<br>

**11. Configure the slave device**

{% hint style="info" %}
   - Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.7.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
   - Double-click the slave device.
{% endhint %}

![[Figure 1.3.7.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_18.png>)


<br>

{% hint style="info" %}
   - Set the connection type of the slave device.

   - Select the message transmission method for DeviceNet communication connection.

   **If the UCMM checkbox is not checked, UCMM group 2 is set as the default value.**   

   - UCMM GROUP 1 : IO Message   
   - UCMM GROUP 2: Master - Slave connection message during network initialization (default setting)   
   - UCMM GROUP 3: Explicit Message   

   - For certain devices, UCMM group 3 may be used, so please check the product specifications before proceeding.
{% endhint %}

![[Figure 1.3.7.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_19.png>)

<br>

{% hint style="info" %}
   - For Crevis NA-9211, proceed without checking the UCMM check box. (Use the group 2 default value.)
{% endhint %}

![[Figure 1.3.7.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_20.png>)

<br>


{% hint style="info" %}
   - Check the DeviceNet slave settings.

   - Output: ST-2318 (1 byte)  
   - Input: ST-1218 (1 byte)  
{% endhint %}

<br>

{% hint style="info" %}
   - Required to set according to the communication method (Poll, Change of State, Cyclic, Bit-Strobe).
{% endhint %}

<br>

![[Figure 1.3.7.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_21.png>)

<br>

{% hint style="info" %}
   [Production Inhibit Time]

   - Set the IO data generation cycle of the slave device (ms)  

   - Example) 10 ms: IO data is generated every 10 ms.  
   - Example) 0 ms: The slave generates IO data as quickly as possible.  

   - The shorter the cycle, the greater the load on the slave device may be. (Specifications need to be checked for each slave.) 
{% endhint %}

<br>

{% hint style="info" %}
   [Expected Packet Rate]

   - Set the time for IO data update between the master and the slave.  
{% endhint %}

<br>

![[Figure 1.3.7.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_22.png>)



<br>

**12. Configure the master device**

{% hint style="info" %}
   - Double-click the Master device.
{% endhint %}

![[Figure 1.3.7.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_23.png>)


{% hint style="info" %}
   - Set the DeviceNet communication speed (to be the same as the slave communication speed).
{% endhint %}

![[Figure 1.3.7.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.7.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_25.png>)

{% hint style="info" %}
   - Set whether to use the Quick Connect function.
{% endhint %}

![[Figure 1.3.7.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_26.png>)


{% hint style="info" %}
   - After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.7.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_27.png>)

<br>

**13. Check the communication status.**

{% hint style="info" %}
   - Check the communication status in Sycon.net and TP.

   - For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
   - Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.7.2-28 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_28.png>)

![[Figure 1.3.7.2-29 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_29.png>)

{% hint style="info" %}
   - Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.7.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_30.png>)

<br>

**14. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}
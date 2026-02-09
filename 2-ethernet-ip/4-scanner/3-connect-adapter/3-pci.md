#### 2.4.3.3 Connecting External Adapter Devices - Hilscher CIFX PCI EtherNet/IP Adapter

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[**Download EDS File Tool (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - Please refer to the Hilscher manual for the IP configuration of the device.
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

![[figure 2.4.3.3-1 CIFX PCI]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_1.png>) 

<br>

**2. Open the EDS file using the EZ-EDS program and verify the device information.**

<br>

![[figure 2.4.3.3-2 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_2.png>) 

<br>

{% hint style="info" %}
   - Check the connection type in the Connection Manager   
      - Example: Exclusive Owner

   - Check for the presence of headers in the Real Time Transfer Format   
      - Input (T > O) : 32-bit run/idle header   
      - Output (O > T) : 32-bit run/idle header   
{% endhint %}

<br>

![[figure 2.4.3.3-3 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_3.png>) 

<br>

{% hint style="info" %}
   - Check the Instance ID in Param   
      - Input (T > O) : 101   
      - Output (O > T) : 100   
{% endhint %}

<br>

**3. Check the I/O size in the device manual.**

<br>

{% hint style="info" %}
   - Check the I/O Size of the current device to be connected (Refer to the corresponding PCI device settings)   
{% endhint %}

<br>

**4. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.3-4 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_4.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the settings correctly.   
      - Input (T > O) : Slave > Master   
      - Output (O > T) : Master > Slave   

   [IO Assembly Information]   
   [T > O]   
      - Size: 240 bytes (Value configured in the PCI device)   
      - Instance: 101   
      - Run/Idle Header: 32Bit   

   [O > T]    
      - Size: 240 bytes (Value configured in the PCI device)   
      - Instance: 100   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
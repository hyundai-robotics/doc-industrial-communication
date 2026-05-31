#### 2.4.3.1 Connecting External Adapter Devices - Crevis Remote IO

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[Download EDS File Tool (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - For the IP settings of the Remote I/O used in the example, please refer to the manual link below.

   - "[1.3.10.2 Remote IO IP Setting](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

![[figure 2.4.3.1-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_1.png>) 

<br>

![[figure 2.4.3.1-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_2.png>) 

<br>

![[figure 2.4.3.1-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_3.png>) 

<br>

**2. Open the EDS file using the EZ-EDS program and verify the device information.**

<br>

![[figure 2.4.3.1-4 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_4.png>) 

<br>

{% hint style="info" %}
   - Check the connection type in the Connection Manager   
      - Example: Exclusive Owner

   - Check for the presence of headers in the Real Time Transfer Format   
      - Input (T > O) : No header   
      - Output (O > T) : 32-bit run/idle header   

   - Click "Create / Decode Path" to verify the Instance ID   
{% endhint %}

<br>

![[figure 2.4.3.1-5 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_5.png>) 

<br>

{% hint style="info" %}
      - Input (T > O) : 1   
      - Output (O > T) : 2   
{% endhint %}

<br>

**3. Check the I/O size in the device manual.**

<br>

{% hint style="info" %}
   - Verify the I/O configuration of the device to be connected. 
{% endhint %}

<br>

![[figure 2.4.3.1-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_6.png>) 

<br>

{% hint style="info" %}
   - Refer to the manual for each slot configuration to determine the total I/O size.
{% endhint %}

<br>

![[figure 2.4.3.1-7 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_7.png>) 

<br>

![[그림 2.4.3.1-8 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_8.png>) 

<br>

**4. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.1-8 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_9.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the settings correctly.   
      - Input (T > O) : Slave > Master   
      - Output (O > T) : Master > Slave   

   [Adapter Configuration]   
   - Crevis M9289   
      - M7002 : None   
      - M2768 : 1byte (O > T)   
      - M2768 : 1byte (O > T)   
      - M12DF : 2bytes (T > O)   
      - M12DF : 2bytes (T > O)   
      - M2768 : 1byte (O > T)   
      - M2768 : 1byte (O > T)   

   [IO Assembly Information]   
   [T > O]   
      - Size: 4bytes   
      - Instance: 1   
      - Run/Idle Header: No   

   [O > T]    
      - Size: 4bytes   
      - Instance: 2   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
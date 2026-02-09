#### 2.4.3.2 Connecting External Adapter Devices - Wago Remote IO

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[**Download EDS File Tool (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - Please refer to the Wago manual for the IP configuration of the device.
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

![[figure 2.4.3.2-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_1.png>) 

<br>

**2. Check the Instance ID provided in the device manual**

<br>

![[figure 2.4.3.2-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_2.png>) 

<br>

{% hint style="info" %}
   - Input (T > O)   
      - 104: Status  + Analog  + Digital   
      - 105: Status  + Digital   
      - 106: Status  + Analog   
      - 107: Analog  + Digital   
      - 108: Digital   
      - 109: Analog   

   - Output (O > T)   
      - 101: Analog + Digital   
      - 102: Digital   
      - 103: Analog   
{% endhint %}

<br>

**3. Open the EDS file using the EZ-EDS program and verify the device information.**

<br>

![[figure 2.4.3.2-3 EDS Info](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_3.png>) 

<br>

{% hint style="info" %}
   - Check the connection type in the Connection Manager   
      - Example: Exclusive Owner

   - Check for the presence of headers in the Real Time Transfer Format   
      - Input (T > O) : No header   
      - Output (O > T) : 32-bit run/idle header   
{% endhint %}

<br>

**4. Check the I/O size in the device manual.**

<br>

{% hint style="info" %}
   - Verify the I/O configuration of the device to be connected. 
{% endhint %}

<br>

![[figure 2.4.3.2-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_4.png>) 

<br>

{% hint style="info" %}
   - Refer to the manual for each slot configuration to determine the total I/O size.
{% endhint %}

<br>

![[figure 2.4.3.2-5 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_5.png>) 

<br>

![[figure 2.4.3.2-6 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_6.png>) 

<br>

**5. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.2-7 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_7.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the settings correctly.   
      - Input (T > O) : Slave > Master   
      - Output (O > T) : Master > Slave   

   [Adapter Configuration]   
   - Wago 750-366   
      - Status 1byte (T > O) (When selecting Instance ID 104, 105, 106)   
      - 753-436 : 1byte (T > O)   
      - 753-536 : 1byte (O > T)   

   [IO Assembly Information]   
   [T > O]   
      - Size: 2bytes   
      - Instance: 105   
      - Run/Idle Header: No   

   [O > T]    
      - Size: 1bytes   
      - Instance: 101   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
#### 2.4.3.4 Connecting External Adapter Devices - Baumer OM-70

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[Download EDS File Tool (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - Please refer to the Baumer manual for the IP configuration of the device.
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

![[figure 2.4.3.4-1 Baumer OM-70]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_1.png>) 

<br>

**2. Verify the Instance ID and I/O Size in the device manual.**

<br>

![[figure 2.4.3.4-2 Baumer OM-70]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_2.png>) 

<br>

{% hint style="info" %}
   [Input Only Connection]   

   - Input (T > O)   
      - Instance ID: 100   
      - Size : 34 bytes   

   - Output (O > T)   
      - Instance ID: 238   
      - Size : 0 byte    
{% endhint %}

<br>

**3. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.4-3 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/4-baumer/img_3.png>)

<br>
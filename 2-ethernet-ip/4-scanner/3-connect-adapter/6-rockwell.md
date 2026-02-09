#### 2.4.3.6 Connecting External Adapter Devices - Rockwell Automation (AB) Remote IO

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[**Download EDS File Tool (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - Please refer to the Rockwell Automation manual for the IP configuration of the device.
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

<br>

![[figure 2.4.3.6-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_1.png>) 

<br>

![[figure 2.4.3.6-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_2.png>) 

<br>

**2. Open the EDS file using the EZ-EDS program and verify the device information.**

<br>

![[figure 2.4.3.6-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_3.png>) 

<br>

![[figure 2.4.3.6-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_4.png>) 

<br>

{% hint style="info" %}
   - Check the connection type in the Connection Manager   
      - Example: Exclusive Owner

   - Check for the presence of headers in the Real Time Transfer Format   
      - Input (T > O) : No header   
      - Output (O > T) : 32-bit run/idle header   

   - Click "Create / Decode Path" to verify the Instance ID   
      - Input (T > O) : 101   
      - Output (O > T) : 100   
      - Configuration : 102   
{% endhint %}

<br>

**3. Check the I/O size in the device manual.**

<br>

{% hint style="info" %}
   - Verify the I/O configuration of the device to be connected. 
{% endhint %}

<br>

![[figure 2.4.3.6-5 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_5.png>) 

<br>

{% hint style="info" %}
   - Verify the I/O configuration of the device to be connected. 
{% endhint %}

<br>

![[figure 2.4.3.6-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_6.png>) 

<br>

![[figure 2.4.3.6-7 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_7.png>) 

<br>

**4. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.6-8 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_8.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the settings correctly.   
      - Input (T > O) : Slave > Master    
      - Output (O > T) : Master > Slave    

   [Adapter Configuration]   
   - Point I/O 1734-AENTR    
      - Status : 8byte (T > O)    
      - 1734-IB8 : 1byte (T > O)   
      - 1734-OB8E : 1byte (O > T) + 1byte (T > O, Status)   

   [IO Assembly Information]   
   [T > O]   
      - Size: 10bytes   
      - Instance: 101   
      - Run/Idle Header: No   

   [O > T]    
      - Size: 1byte   
      - Instance: 100   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>

![[figure 2.4.3.6-9 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_9.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the additional settings correctly.   
      - Input (T > O) : Slave > Master   
      - Output (O > T) : Master > Slave   

   [Additional Settings]   
      - Config Segment : ON   
      - Instance: 102   
      - Size: 10bytes    

   [Config Segment Information]    
      - (4bytes) 1 : Header    
      - (2bytes) 3 : Connected Slots + 1   
      - (1byte)  0 : T > O Alignment (in bytes)      
      - (1byte)  1 : T > O Data Size per slot      
      - (1byte)  0 : O > T Alignment (in bytes)      
      - (1byte)  1 : O > T Data Size per slot      
{% endhint %}

<br>
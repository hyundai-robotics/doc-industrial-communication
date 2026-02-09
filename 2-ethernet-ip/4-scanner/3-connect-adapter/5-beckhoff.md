#### 2.4.3.5 Connecting External Adapter Devices - Beckhoff Remote IO

<br>

{% hint style="info" %}
   - You can easily verify the configuration information of an EtherNet/IP Adapter device using the EZ-EDS program.

   - "[**Download EDS File Tool (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - Please refer to the Beckhoff manual for the IP configuration of the device.
{% endhint %}

<br>

**1. Prepare the manual and the EDS file for the Adapter device.**

![[figure 2.4.3.5-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_1.png>) 

<br>

**2. Access the device's webpage to configure the IP address.**

<br>

{% hint style="info" %}
   - In this example, the initial IP address is set to 192.168.1.2 (DIP switch No. 2 is ON)
{% endhint %}

<br>

![[figure 2.4.3.5-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_2.png>) 

<br>

![[figure 2.4.3.5-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_3.png>) 

<br>

{% hint style="info" %}
   - In this example, the IP address is changed to 192.168.10.95. 

   - After entering the IP address, click the Check button to save. 
{% endhint %}

<br>

![[figure 2.4.3.5-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_4.png>) 

<br>

{% hint style="info" %}
   - Set the DIP switches as shown below and reboot the device:   
      - 1 ~ 8  : ON   
      - 9 ~ 10 : OFF   
{% endhint %}

<br>

![[figure 2.4.3.5-5 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_5.png>) 

<br>

![[figure 2.4.3.5-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_6.png>) 

<br>

**3. Access the device's webpage to verify the EtherNet/IP configuration information.**

<br>

{% hint style="info" %}
   - Re-access the webpage using the newly configured IP address and verify the IP address and EtherNet/IP configuration details.
{% endhint %}

<br>

![[figure 2.4.3.5-7 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_7.png>) 

<br>

![[figure 2.4.3.5-8 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_8.png>) 

<br>

{% hint style="info" %}
   - Input (T > O)   
      - Instance ID: 129   
      - Byte Size: 6      

   - Output (O > T)   
      - Instance ID: 130   
      - Byte Size: 6   
{% endhint %}

<br>

**4. Enter the communication settings based on the Adapter device information.**

<br>

![[figure 2.4.3.5-9 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_9.png>)

<br>

{% hint style="info" %}
   - Please refer to the manual of the target device to enter the settings correctly.   
      - Input (T > O) : Slave > Master    
      - Output (O > T) : Master > Slave   

   [Adapter Configuration]   
   - Beckhoff EK-9500   
      - EK-1008 : 1byte (T > O)   
      - EK-2008 : 1byte (O > T)   

   [IO Assembly Information]   
   [T > O]   
      - Size: 6bytes   
      - Instance: 129   
      - Run/Idle Header: No   

   [O > T]    
      - Size: 6bytes   
      - Instance: 130   
      - Run/Idle Header: 32Bit   
{% endhint %}

<br>
# 3.3.4 Setting an EtherNet/IP Adapter

Perform settings according to the procedures of “[**3.1 Setting Industrial Communication Firmware**](../../3-settings-industrial-communication/3-1-Settings-firmware.md)” and proceed with the following methods.

<br>

{% hint style="info" %}
\.      **[EtherNet/IP Adapter EDS File Download]**

\.      Refer to “[**6. Slave Device Description Files**](../../6-slave-config-file.md)".
{% endhint %}

<br>

##### 1. By using the teach pendant, select an EtherNet/IP slave in the section for setting industrial communication firmware and reboot the robot controller.

![[Figure 3.3.4-1 Firware Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

##### 2. Check the readiness of the selected protocol in the section for monitoring industrial communication. 

![[Figure 3.3.4-2 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If the Config file set using SYCON.net has been downloaded to the relevant PCI slot, the setting values of the teach pendant will be ignored.
{% endhint %}

<br>

##### 3. Click the menu to enter the slave setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 2: Slave Configuration >  EtherNet/IP Slave]**

![[Figure 3.3.4-3 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[Figure 3.3.4-4 Slave Setting]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

##### 4. Description of Each Item

{% hint style="info" %}
\.      [IP setting]

\.      Fixed IP: For setting the IP address, subnet mask, and gateway information.

\.      DHCP: For receiving an IP address from the dynamic host configuration protocol (DHCP) server.
{% endhint %}

{% hint style="info" %}
\.      [Action in Bus Error]

\.      Clear: For initializing all inputs to 0 when a communication error occurs.

\.      Hold: For retaining the last valid input values when a communication error occurs.
{% endhint %}

{% hint style="info" %}
\.      (Error Allowed Time)

\.      For outputting a field bus error signal and an alarm if the communication error lasts for a specified allowable time.
{% endhint %}

{% hint style="info" %}
\.      [Input Bytes]

\.      Input Bytes: Master -> For setting the size of the data to be inputted from the master to the slave.

\.      O -> T: Originator (Master) -> Target (Slave)
{% endhint %}

{% hint style="info" %}
\.      [Output Bytes]

\.      Output Bytes: Slave -> For setting the size of the data to be outputted from the slave to the master.

\.      T -> O: Target (Slave) -> Originator (Master)
{% endhint %}

{% hint style="info" %}
\.      [Run/Idle Header]

\.      The CIFX-50 RE EtherNet/IP Adapter applied to the controller uses a 32-bit Run/Idle Header when exchanging IOs with the scanner (default).

\.      Depending on the specifications of the scanner, properly set whether to use the Input and Out 32-bit Run/Idle Header where appropriate.
{% endhint %}

<br>

{% hint style="info" %}
\.        [Quick Connect]

\.        EtherNet/IP supports the quick connect function.

\.        When using the quick connect function is necessary, set the EtherNet/IP adapter using SYCO.net.

\.        (1) Products that support the master and slave quick connect function are needed.  
\.        (2) The quick connect function cannot be used when using the auto negotiation function.  
\.        (3) The quick connect function cannot be used when using auto MDI-X function.  
\.        (4) 100 Mbit/s and full duplex need to be used.  
{% endhint %}

<br>

##### 5. When the settings are completed, check the communication status according to the following procedures.

Refer to (“[**4 Monitoring Industrial Communication**](../../4-monitoring-industrial-communication/README.md)”) for the procedures to check the industrial communications status in the teach pendant.

![[Figure 3.3.4-5 Industrial Communication Monitoring]](<../../_assets/3-Settings-Industrial-Communication/3.3-EtherNet-IP/4-Slave_setting/image_5.png>) 
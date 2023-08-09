# 3.10.2 Setting the Remote IO IP Address

This shows how to set the IP address of the Crevis M9289 EtherNet/IP network adapter.

<br>

{% hint style="info" %}
\.      The factory set IP address of the remote IO M9289 of the Crevis is 192.168.100.99.

\.      If the IP address of the remote IO is not known or needs to be changed, comply with the following.
{% endhint %}

<br>

##### 1. Connect the PC and remote IO directly using the LAN cable.

![[Figure 3.10.2-1 LAN Connection]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

##### 2. Change only the DIP switch 9 of the remote IO adapter to the On state.

![[Figure 3.10.2-2 DIP Switch]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

##### 3. Run the Bootpsvr.exe program.
   * The program is to be provided by Crevis. (Download IO Guide Pro from the company’s website and install it.)

![[Figure 3.10.2-3 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[Figure 3.10.2-4 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
\.      While pressing the Start BootP button, disconnect the power of the M9289 module and apply it again to reboot it.
{% endhint %}

![[Figure 3.10.2-5 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>


##### 4. When the adapter device is rebooted, the device information will appear in the BootSvr.exe program.

![[Figure 3.10.2-6 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

##### 5. Select a device and set the IP address.

![[Figure 3.10.2-7 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[Figure 3.10.2-8 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

##### 6. After changing all DIP switches of the adapter whose IP settings are complete to the Off state, reboot the device.

{% hint style="info" %}
\.      You must check the status of the DIP switches and whether the adapter is rebooted.
{% endhint %}

![[Figure 3.10.2-9 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

##### 7. Check the IP address by using some methods such as a ping test in the PC.

![[Figure 3.10.2-10 Bootp]](<../../_assets/3-Settings-Industrial-Communication/3.10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

##### 8. If the IP address is normally changed, proceed with the settings.

{% hint style="info" %}
\.      Please proceed with settings according to the  procedures of “[**3.10.1 EtherNet/IP - Setting the Connection of a Standard remote IO**](../../3-settings-industrial-communication/3-10-EtherNet-IP-Remote-IO/3-10-1-Settings-EtherNet-IP-Remote-IO.md).”
{% endhint %}

#### 1.3.10.2 Remote IO IP Address Settings

This is how to set the IP address of the M9289 EtherNet/IP network adapter from Crevis.

<br>

{% hint style="info" %}
   - The factory default IP of the Crevis M9289 Remote IO is 192.168.100.99.

   - If you do not know the Remote IO IP or need to change it, please follow the steps below.
{% endhint %}

<br>

**1. Connect the PC and Remote IO directly using a LAN cable.**

![[Figure 1.3.10.2-1 LAN Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

**2. Change only DIP switch 9 of the Remote IO Adapter to ON.**

![[Figure 1.3.10.2-2 DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

**3. Execute the Bootpsvr.exe program.**
   * This program is provided by Crevis. (Download and install IO Guide Pro from the website.)

![[Figure 1.3.10.2-3 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[Figure 1.3.10.2-4 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
   - With Start BootP being pressed, disconnect and reapply power to the M9289 module to reboot it.
{% endhint %}

![[Figure 1.3.10.2-5 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>


**4. When the adapter device is rebooted, the device information will appear in the BootpSvr.exe program.**

![[Figure 1.3.10.2-6 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

**5. Select the device and set the IP.**

![[Figure 1.3.10.2-7 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[Figure 1.3.10.2-8 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

**6. After completing the IP setting, turn all DIP switches of the adapter to OFF and reboot the device.**

{% hint style="info" %}
   - Be sure to check the DIP switch status and whether the adapter is rebooted.
{% endhint %}

![[Figure 1.3.10.2-9 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

**7. Use the ping test, etc. on the PC to verify the IP.**

![[Figure 1.3.10.2-10 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

**8. If the IP address has been changed successfully, proceed with settings.**

{% hint style="info" %}
   - Please proceed with the settings according to the "[**1.3.10.1 EtherNet/IP - Standard Remote IO Connection Settings**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)" procedure.
{% endhint %}

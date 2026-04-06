#### 1.3.10.1 EtherNet/IP - Standard Remote IO Connection Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

**1. Select EtherNet/IP Master in the industrial communication firmware settings and reboot the robot controller.**

![[Figure 1.3.10.1-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_1.png>) 

<br>

**2. Check the readiness status of the selected protocol in the industrial communication monitoring menu.**

![[Figure 1.3.10.1-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_2.png>) 

<br>

**3. Connect the PCI and Remote IO cables, etc. for communication and check the status.**

![[Figure 1.3.10.1-3 Hardware Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_3.png>) 

![[Figure 1.3.10.1-4 Hardware Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_4.png>) 

<br>

{% hint style="info" %}
   - Please connect the PCI and Remote IO using a LAN cable.

   - Set all DIP switches of the Remote IO to OFF.

   - Connect both the Remote IO power and Field Power (24 V DC).
{% endhint %}

<br>

{% hint style="info" %}
   - The factory default IP of the Crevis M9289 Remote IO is 192.168.100.99.

   - The Remote IO IP should be set to 192.168.100.99 to enable communication connection.

   - "[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

**4. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > EtherNet/IP Remote IO Setting]**

![[Figure 1.3.10.1-5 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_5.png>)

![[Figure 1.3.10.1-6 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_6.png>)

<br>

{% hint style="info" %}
   - The IP is set as a fixed value.

   - Check the input and output byte counts.

   - The selected input and output byte counts should be less than or equal to the IO byte counts of the card installed in the Remote IO slot.
{% endhint %}

<br>

{% hint style="info" %}
   - Input Module  
   - M12DF: Digital 16 points  
   - M3534: Analog 4 points  
{% endhint %}

{% hint style="info" %}
   - Output Module  
   - M225F: Digital 16 points  
   - M226F: Digital 16 points  
   - M2768: Digital 8 points   
   - M4534: Analog 4 points  
{% endhint %}

{% hint style="info" %}
   - Special Module  
   - M5112 : Conveyer I/F
{% endhint %}

<br>

**5. Reboot the controller after completing the settings.**

![[Figure 1.3.10.1-7 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_7.png>)

![[Figure 1.3.10.1-8 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_8.png>) 

{% hint style="info" %}
   - Please reboot the controller after completing the settings.
{% endhint %}

<br>

**6. After confirming that the setting values are reflected, check the communication status.**

![[Figure 1.3.10.1-9 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_9.png>)

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.10.1-10 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_10.png>)

{% hint style="info" %}
   - If communication is not connected, you should check the Remote IO IP.

   - Please follow the steps below. (If not 192.168.100.99)

   - "[**1.3.10.2 Remote IO IP Setting**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

![[Figure 1.3.10.1-11 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_11.png>) 

![[Figure 1.3.10.1-12 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Setting/image_12.png>)

<br>

**7. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**5. Industrial Communication IO Block Assignment**](../../../5-io-block-allocation.md)").**
{% endhint %}
## 2.1 Network Settings

**1. Main Module**

<br>

The LAN ports that can connect with the EtherNet/IP adapter are LAN1/LAN2/LAN3.

<br>

![figure 2.1-1 Main Module](../_assets/2-ethernet-ip/1-network/hi6com.png)

<br>

**2. Network Settings**

<br>

Select a LAN port to connect EtherNet/IP communication and then check the settings of the LAN port through the TP screen as shown below and change the settings as needed.

<br>

![figure 2.1-2 Network configuration](../_assets/2-ethernet-ip/1-network/networkConfig.png)

<br>

{% hint style="info" %}
   - The subnet portion of each IP address of LAN1/LAN2/LAN3 should be set differently.

   - After changing the settings, reboot the robot controller.
{% endhint %}

<br>

**3. Connection Status Check**

<br>

The status of the physical connection with the EtherNet/IP scanner can be checked according to the status of the Link/Act LED of the LAN port.

<br>

Connect the EtherNet/IP adapter and scanner with a LAN cable and then check the LED status. If the LED on the left does not light up or blink, it means there is a problem with the cable or adapter or scanner device. Please check the connection status of the cable or device.

<br>

![figure 2.1-3 LAN Port](../_assets/2-ethernet-ip/1-network/lanPort.png)

<br>

**4. Network Configuration**

<br>

It is recommended to configure the EtherNet/IP Network and Factory Network as separate networks. As shown in the figure below, if you configure the EtherNet/IP Network and Factory Network as one network, they will share one transmission medium, increasing the network load. Therefore, it is recommended to use a separately configured network for the EtherNet/IP Network if possible.

<br>

![figure 2.1-4 Network](../_assets/2-ethernet-ip/1-network/NG_Network.png)

<br>

![figure 2.1-5 Network](../_assets/2-ethernet-ip/1-network/Good_Network.png)

<br>

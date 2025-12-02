## 2.2 EtherNet/IP Adapter Network Settings

### 2.2.1 Hi6 Com
The LAN ports that can connect with the EtherNet/IP adapter are LAN1/LAN2/LAN3.<br>

![!hi6com.png<br>](../_assets/2-EtherNet-IP-Adapter/Network/hi6com.png)<br>
* [Figure 2.2.1 Hi6 Com]*<br>

### 2.2.2 Network Settings
Select a LAN port to connect EtherNet/IP communication and then check the settings of the LAN port through the TP screen as shown below and change the settings as needed.<br>

![!networkConfig.png<br>](../_assets/2-EtherNet-IP-Adapter/Network/networkConfig.png)<br>
* [Figure 2.2.2 Network Settings]*<br>

{% hint style="info" %}
\.      The subnet portion of each IP address of LAN1/LAN2/LAN3 should be set differently.

\.      After changing the settings, reboot the robot controller.
{% endhint %}

### 2.2.3 Connection Status Check
The status of the physical connection with the EtherNet/IP scanner can be checked according to the status of the Link/Act LED of the LAN port.<br>

![!lanPort.png<br>](../_assets/2-EtherNet-IP-Adapter/Network/lanPort.png)<br>
* [Figure 2.2.3 LAN Port]*<br>

Connect the EtherNet/IP adapter and scanner with a LAN cable and then check the LED status. If the LED on the left does not light up or blink, it means there is a problem with the cable or adapter or scanner device. Please check the connection status of the cable or device.<br>

### 2.2.4 Network Configuration
It is recommended to configure the EtherNet/IP Network and Factory Network as separate networks. As shown in the figure below, if you configure the EtherNet/IP Network and Factory Network as one network, they will share one transmission medium, increasing the network load. Therefore, it is recommended to use a separately configured network for each EtherNet and IP Network if possible.<br>

![!NG_Network.png<br>](../_assets/2-EtherNet-IP-Adapter/Network/NG_Network.png)<br>
* [Figure 2.2.4 Non-separated Network]*<br>

![!Good_Network.png<br>](../_assets/2-EtherNet-IP-Adapter/Network/Good_Network.png)<br>
* [Figure 2.2.5 Separated Network]*<br>

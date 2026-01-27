## 2.3 EtherNet/IP Adapter

<br>

**2.3.1 EtherNet/IP Adapter Specifications**

<br>

|Item|Description|
|------|---|
|Device Type|General Purpose Discrete I/O (7)|
|Input Assembly Instance|100|
|Output Assembly Instance|112|
|Input Size Range(bytes)|0 - 240|
|Output Size Range(bytes)|0 - 240|
|RPI Range (ms)|5 – 3000|<br>

<br>

**2.3.2 EtherNet/IP Adapter Settings and Monitoring via Teaching Pendant**

<br>

On the initial screen, navigate to "SYSTEM" > "Control Parameter" > "Industrial Communication" > "Ethernet/IP Adapter"<br>
![Config.PNG](../_assets/2-EtherNet-IP-Adapter/Spec/Config.PNG)<br>
*[Figure 2.3.1 Settings]*

<br>

**[Network]**
-	Function Use: Select whether to use the Ethernet/IP adapter.
-	Ethernet Port Selection: Select the LAN port to be connected to the Ethernet/IP scanner. (The information of the selected LAN port is displayed on the line immediately below.)<br>

**[I/O Size]**
-	Input Byte Count: 0–240 can be set.
-	Output Byte Count: 0–240 can be set.<br>

**[Monitoring]**
- Run: Indicates the I/O data exchange status of Ethernet/IP (On: Normal communication. Off: No communication).
- Ready: Indicates the initialization status of the Ethernet/IP adapter (On: Initialization normal. Off: Initialization abnormal).
- Error: Displays the alarm or warning status of the Ethernet/IP adapter (On: Alarm/warning status. Off: Normal).
- Version: Displays the Ethernet/IP adapter S/W version information.
- Error Code: Displays the alarm or warning code when an alarm or warning occurs.

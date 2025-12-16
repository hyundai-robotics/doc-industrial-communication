### 2.6.1 Connection with LS ELECTRIC PLC

This section explains how to connect the LS ELECTRIC PLC with Hi6 EtherNet/IP.  
The PLC and communication module used below are as follows.  
(PLC: XGI-CPUS, Communication Module: XGL-EFMTB)

#### 2.6.1.1 XG5000 Running
![xg5000.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/xg5000.png) <br>
*[Figure 2.6.1.1 XG5000 Running]*<br>
For downloading the XG5000 program and detailed usage methods, please refer to the LS ELECTRIC website.

#### 2.6.1.2 EDS File Registration
Click Menu > Tools > EDS(D) > EDS File Registration, and then select "Hi6_EIP_240402.eds."<br>
Confirm EDS file registration as shown in the figure below.<br>
![eds.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/eds.png)<br>
*[Figure 2.6.1.2 EDS File Registration]*<br>


#### 2.6.1.3 Device Connection
[1] Create a project.<br>
![newProject_1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_1.png)<br>
*[Figure 2.6.1.3 Creating a New Project]*<br>

[2] Add a communication module.<br>
![newProject_2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_2.png)<br>
*[Figure 2.6.1.4 Adding a Communication Module 1]*<br>

![newProject_3.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_3.png)<br>
*[Figure 2.6.1.5 Adding a Communication Module 2]*<br>

![newProject_4.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_4.png)<br>
*[Figure 2.6.1.6 Adding a Communication Module 3]*<br>

[3] Set a communication module <br>
Double-click XGL-EFMT shown in the left tab in the figure below.<br>
![newProject_6.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_6.png)<br>
*[Figure 2.6.1.7 Communication Module Settings]*<br>
- Set the IP address, subnet mask, gateway, etc.  
- To use the two LAN ports of the PLC as a relay function, select the "Relay" checkbox.  
- Change the RAPIEnet setting to Disable.

#### 2.6.1.4 Online Connection Settings
[1] Connect the PLC with a USB cable.<br>
![newProject_7.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_7.png)<br>
*[Figure 2.6.1.8 Online Connection Settings 1]*<br>

[2] Press the button shown on the left in the figure below to download the entire settings.<br>
![newProject_8.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/newProject_8.png)<br>
*[Figure 2.6.1.9 Online Connection Settings 2]*<br>

#### 2.6.1.5 Auto Scan
[1] Auto Scan is possible when connected to the PLC.<br>
If the current state is not online, click Menu > Online > Connect to change to online status.<br>

[2] Right-click XGL-EFMT > Add Item > Smart Expansion<br>
![auto1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto1.png)<br>
*[Figure 2.6.1.10 Auto Scan 1]*<br>

[3] Click Next. <br>
![auto2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto2.png)<br>
*[Figure 2.6.1.11 Auto Scan 2]*<br>

[4] Click Auto Scan. <br>
![auto3.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto3.png)<br>
*[Figure 2.6.1.12 Auto Scan 3]*<br>

![auto4.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto4.png)<br>
*[Figure 2.6.1.13 Auto Scan4]*<br>

[5] Check the automatically scanned devices.  
![auto5.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto5.png)<br>
*[Figure 2.6.1.14 Auto Scan5]*<br>

![auto6.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto6.png)<br>
*[Figure 2.6.1.15 Auto Scan6]*<br>

The Hi6 EtherNet/IP adapter device appears in the list as shown in the figure below. <br>
![auto7.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/auto7.png)<br>
*[Figure 2.6.1.16 Auto Scan7]*<br>

#### 2.6.1.6 Program Variable Registration
[1] Scan Program > NewProgram > Local Variables (double-click)<br>
![variable1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/variable1.png)<br>
*[Figure 2.6.1.17 Variable Registration 1]*<br>

[2] Set the input/output data to be used in communication.<br>
![variable2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/variable2.png)<br>
*[Figure 2.6.1.18 Variable Registration 2]*<br>

#### 2.6.1.7 EtherNet/IP Adapter Settings
[1] Double-click EB01 (Hi6 EtherNet/IP adapter) in the list on the left.<br>

[2] Press the EIP detailed settings button.<br>
![AdapterSetting1.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting1.png)<br>
*[Figure 2.6.1.19 EtherNet/IP Adapter Settings 1]*<br>

[3] Refer to the figure below to select the setting values for the EtherNet/IP adapter. <br>
- Connection type
- T2O RPI Range, O2T RPI Range
- T2O Input, O2T Output size
- Transmission cycle
- Timeout
- Local tag, Remote tag <br>
![AdapterSetting2.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting2.png) <br>
*[Figure 2.6.1.20 EtherNet/IP Adapter Settings 2]*<br>

[4] Click Online > Communication Module Settings and Diagnostics > Service Enable.<br>
![AdapterSetting3.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting3.png)<br>
*[Figure 2.6.1.21 EtherNet/IP Adapter Settings 3]*<br>

[5] Check the FEnet I/O Service checkbox.<br>
![AdapterSetting4.png](../../_assets/2-EtherNet-IP-Adapter/ConnectWithScanner/AdapterSetting4.png)<br>
*[Figure 2.6.1.22 EtherNet/IP Adapter Settings 4]*<br>

<br>

##### 2.6.1.8 Assignment of IO Blocks after Completion of Communication Settings

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../4-io-block-allocation.md)").**
{% endhint %}
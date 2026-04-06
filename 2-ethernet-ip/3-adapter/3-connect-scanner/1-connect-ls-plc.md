#### 2.3.3.1 LS ELECTRIC PLC

<br>

This section explains how to connect the LS ELECTRIC PLC with EtherNet/IP.  
The PLC and communication module used below are as follows.  
(PLC: XGI-CPUS, Communication Module: XGL-EFMTB)

<br>

**1. XG5000 Running**

<br>

![xg5000.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/xg5000.png)

<br>

For downloading the XG5000 program and detailed usage methods, please refer to the LS ELECTRIC website.

<br>

**2. EDS File Registration**

<br>

Click Menu > Tools > EDS(D) > EDS File Registration, and then select "Hi6_EIP_240402.eds."
Confirm EDS file registration as shown in the figure below.

<br>

![eds.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/eds.png)

<br>

**3. Device Connection**

<br>

[1] Create a project.<br>
![newProject_1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_1.png)<br>

[2] Add a communication module.<br>
![newProject_2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_2.png)<br>

![newProject_3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_3.png)<br>

![newProject_4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_4.png)<br>

<br>

[3] Set a communication module <br>
Double-click XGL-EFMT shown in the left tab in the figure below.<br>
![newProject_6.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_6.png)

<br>

- Set the IP address, subnet mask, gateway, etc.  
- To use the two LAN ports of the PLC as a relay function, select the "Relay" checkbox.  
- Change the RAPIEnet setting to Disable.

<br>

**4. Online Connection Settings**

<br>

[1] Connect the PLC with a USB cable.<br>
![newProject_7.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_7.png)<br>

[2] Press the button shown on the left in the figure below to download the entire settings.<br>
![newProject_8.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/newProject_8.png)<br>

<br>

**5. Auto Scan**

<br>

[1] Auto Scan is possible when connected to the PLC.<br>
If the current state is not online, click Menu > Online > Connect to change to online status.<br>

[2] Right-click XGL-EFMT > Add Item > Smart Expansion<br>
![auto1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto1.png)<br>

[3] Click Next. <br>
![auto2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto2.png)<br>

[4] Click Auto Scan. <br>
![auto3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto3.png)<br>

![auto4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto4.png)<br>

[5] Check the automatically scanned devices.  
![auto5.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto5.png)<br>

![auto6.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto6.png)<br>

The Hi6 EtherNet/IP adapter device appears in the list as shown in the figure below. <br>
![auto7.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/auto7.png)<br>

<br>

**6. Program Variable Registration**

<br>

[1] Scan Program > NewProgram > Local Variables (double-click)<br>
![variable1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/variable1.png)<br>

[2] Set the input/output data to be used in communication.<br>
![variable2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/variable2.png)<br>

<br>

**7. EtherNet/IP Adapter Settings**

<br>

[1] Double-click EB01 (Hi6 EtherNet/IP adapter) in the list on the left.<br>

[2] Press the EIP detailed settings button.<br>
![AdapterSetting1.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting1.png)<br>

[3] Refer to the figure below to select the setting values for the EtherNet/IP adapter. <br>
- Connection type
- T2O RPI Range, O2T RPI Range
- T2O Input, O2T Output size
- Transmission cycle
- Timeout
- Local tag, Remote tag <br>
![AdapterSetting2.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting2.png) <br>

[4] Click Online > Communication Module Settings and Diagnostics > Service Enable.<br>
![AdapterSetting3.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting3.png)<br>

[5] Check the FEnet I/O Service checkbox.<br>
![AdapterSetting4.png](../../../_assets/2-ethernet-ip/3-adapter/3-connect-scanner/AdapterSetting4.png)<br>

<br>

**8. Assignment of IO Blocks after Completion of Communication Settings**

<br>

{% hint style="info" %}
   **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**5. Industrial Communication IO Block Assignment**](../../../5-io-block-allocation.md)").**
{% endhint %}
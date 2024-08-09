# 3.1 Setting the EtherCAT Master IO

<br>

##### 1. Click the menu to enter the setting screen. 
**\[System > 2: Control Parameter > 11: Industrial Communication > 4: EtherCAT Master Settings]**

<br>

![[Figure 3.1-1 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_1.png>) 

<br>

{% hint style="info" %}
\.      Check the controller LAN port number on ther EtherCAT Master Settings screen.
{% endhint %}

##### 2. For communication, connect the cables for the controller LAN port and remote IOs and check their status.

<br>

![[Figure 3.1-2 Cable Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_2.png>) 
![[Figure 3.1-3 Cable Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_3.png>) 

<br>

{% hint style="info" %}
\.      Connect the controller LAN port and remote IO using the LAN cable.

\.      Set all DIP switches of the remote IO to the Off state.

\.      Connect every remote IO power and field power (24 V DC).
{% endhint %}

<br>

##### 3. Select whether to use EtherCAT Master to ON in the settings screen.

<br>

![[Figure 3.1-4 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_4.png>) 

<br>

{% hint style="info" %}
\.      Select the communication cycle time.

\.      Supported 1ms, 2ms, 5ms
{% endhint %}

<br>

##### 4. On the settings screen, Select configured module from the slave device list.

<br>

![[Figure 3.1-5 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_5.png>)

<br>

{% hint style="info" %}
\.      Check the Input Bytes and Output Bytes.
{% endhint %}

<br>

{% hint style="info" %}
\.      Input Module  
\.      M12DF: Digital 16 points  
\.      M3534: Analog 4 points  
{% endhint %}

{% hint style="info" %}
\.      Output Module  
\.      M225F: Digital 16 points  
\.      M226F: Digital 16 points  
\.      M2768: Digital 8 points  
\.      M4534: Analog 4 points  
{% endhint %}

{% hint style="info" %}
\.      Special Module   
\.      M5112: Conveyer I/F 
{% endhint %}

<br>

![[Figure 3.1-6 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_6.png>) 

<br>

##### 5. After the settings are completed, reboot the controller.

![[Figure 3.1-7 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_7.png>) 

<br>

![[Figure 3.1-8 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_8.png>) 

<br>

{% hint style="info" %}
\.      After the settings are completed, reboot the controller.
{% endhint %}

<br>

##### 6. Check whether the set values are reflected and then check the communication status.

![[Figure 3.1-9 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_9.png>) 

<br>

{% hint style="info" %}
\.      Please check the communication connection status and error.
{% endhint %}

<br>

![[Figure 3.1-10 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_10.png>)

<br>

{% hint style="info" %}
\.      Please check ther LED on the Remote IO Module if communication is working properly.
{% endhint %}

<br>

{% hint style="info" %}
\.      **If error occurs, Please check the following : (“[**3.2 Action for the EtherCAT Master IO Error**](../3-ethercat-master-io/2-Error-EtherCAT-Master.md)”)**
{% endhint %}

<br>

##### 7. After completing communication setup, Allocate IO block

{% hint style="info" %}
\.      **You can use input/output signals by allocating an IO block. Please Check (“[**4. Setting IO Block Allocation of the Industrial Communication**](../4-io-block-allocation.md)”)**
{% endhint %}


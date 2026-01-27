## 3.1 EtherCAT Master IO Settings

<br>

**1. Touch the menu to enter the settings screen. **
**\[System > 2: Control Parameters > 11: Industrial Communication > 4: EtherCAT Master Settings]**

<br>

![[Figure 3.1-1 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_1.png>) 

<br>

{% hint style="info" %}
\.      Check the selected controller LAN port number on the EtherCAT master settings screen. 
{% endhint %}

**2. Connect the controller LAN port and Remote IO cables, etc. for communication and check the status.**

<br>

![[Figure 3.1-2 Hardware Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_2.png>) 
![[Figure 3.1-3 Hardware Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_3.png>) 

<br>

{% hint style="info" %}
\.      Please connect the controller and Remote IO using a LAN Cable.

\.      Set all DIP switches of the Remote IO to OFF.

\.      Connect both the Remote IO power and Field Power (24 V DC).
{% endhint %}

<br>

**3. Select "ON" for the EtherCAT master usage in the settings menu.**

<br>

![[Figure 3.1-4 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_4.png>)

<br>

{% hint style="info" %}
\.      Set the communication cycle according to your usage environment.

\.      Communication cycles of 1 ms, 2 ms, and 5 ms are supported.
{% endhint %}

<br>

**4. Select the same configuration as the connected Remote IO module from the slave list in the settings menu.**

<br>

![[Figure 3.1-5 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_5.png>)

<br>

{% hint style="info" %}
\.      Check the input and output byte counts.
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
\.      M5112 : Conveyer I/F 
{% endhint %}

<br>

![[Figure 3.1-6 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_6.png>) 

<br>

**5. Reboot the controller after completing the settings.**

![[Figure 3.1-7 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_7.png>) 

<br>

![[Figure 3.1-8 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_8.png>) 

<br>

{% hint style="info" %}
\.      Please reboot the controller after completing the settings.
{% endhint %}

<br>

**6. After confirming that the setting values are reflected, check the communication status.**

![[Figure 3.1-9 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_9.png>) 

<br>

{% hint style="info" %}
\.      Please check the communication connection status and check for any error.
{% endhint %}

<br>

![[Figure 3.1-10 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_10.png>)

<br>

{% hint style="info" %}
\.      Please check if communication is properly established using LEDs on the Remote IO Module.
{% endhint %}

<br>

{% hint style="info" %}
\.      **If an error occurs during communication, refer to ("[**3.2 EtherCAT Master IO Error Handling**](../3-ethercat-master-io/2-Error-EtherCAT-Master.md)").**
{% endhint %}

<br>

**7. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../4-io-block-allocation.md)").**
{% endhint %}


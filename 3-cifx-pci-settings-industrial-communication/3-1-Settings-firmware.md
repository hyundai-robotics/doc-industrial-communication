# 3.1 Setting Industrial Communication Firmware

The methods for setting up the industrial communication firmware to be used is as follows. After the settings are completed, restarting the controller's power to apply the firmware will be necessary.

<br>

##### 1. Click the menu to enter the firmware setting screen.
**\[System > 2: Control Parameter > 11: Industrial Communication > 1: Firmware Setting > 1 Channel]**


<br>

##### 2. By referring to the screens shown below, select the slot, communication mode (master/slave), and protocol.
   * The slot number is the rotary switch number of the PCI communication card.
   * If you do not want to set the communication firmware, click the **\[OK]** button to end the process.

{% hint style="warning" %}
**\[Caution]**: Clicking the **\[Clear]** or **\[Apply]** buttons will initialize the firmware information on the tab you are currently viewing. Note that the Config file will be also initialized.  
{% endhint %}

![[Figure 3.1-1 Industrial Communication Setting Screen]](<../_assets/3-Settings-Industrial-Communication/3.1-Setting-Firmware/image_1.png>)

![[Figure 3.1-2 Industrial Communication Setting Screen (master)]](<../_assets/3-Settings-Industrial-Communication/3.1-Setting-Firmware/image_2.png>) ![[Figure 3.1-3 Industrial Communication Setting Screen (slave)]](<../_assets/3-Settings-Industrial-Communication/3.1-Setting-Firmware/image_3.png>)

<br>

##### 3. Complete the firmware settings. 
Click on the **\[Apply]** button.

![[Figure 3.1-4 Industrial Communication Setting Screen]](<../_assets/3-Settings-Industrial-Communication/3.1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[Caution]**

<1>. When you finish setting up the firmware by clicking the **\[Apply]** button, all Config files set in the corresponding slots will be deleted. When required to change the communication firmware during use, back up the current Config settings separately.

<2>. If you click the **\[OK]** button without clicking the **\[Apply]** button first, the set firmware will not be applied.
{% endhint %}

<br>

##### 4. Repeat steps 2 and 3 for each slot to set the firmware.

<br>

##### 5. Reboot the Controller for the set firmware to be applied.
Click the menu under **\[Service > 19: Industrial Communication Monitoring]** to check if the set communication has been applied.

![[Figure 3.1-5 Industrial Communication Setting Screen]](<../_assets/3-Settings-Industrial-Communication/3.1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[Caution]**: When you set the use of the firmware, you must Reboot Controller to apply the settings to the system.
{% endhint %}

# 3.1 Setting the Industrial Communication Firmware

The method to set and use the industrial communication firmware is as shown below. After the setting is completed, the controller power should be turned off and then back on to allow the firmware to be applied.

1. Set the **\[Set Up > 2: Control Parameter > 11: Industrial Communication > 1: Firmware Setting > 1 Channel]** menu to enter the firmware setting screen.
2. By referring to the screen shown below, select the slot you set in advance and then set the communication method (Master/Slave). Finally, select the desired protocol.
   * The slot number is the rotary switch number of the PCI communication card.
   * If you do not want to set the communication firmware, you should initialize the firmware information on the tab you are looking at now by touching the **\[Clear]** button. Please take note that the Config file will also be initialized.

![Figure 3 Screen for setting the industrial communication (master)](<../_assets/image (7).png>) ![Figure 3 Screen for setting the industrial communication (Slave)](<../_assets/image (3).png>)

3\. Touch the **\[Apply]** menu to complete the firmware setting.

{% hint style="warning" %}
**\[Caution]**

1. When you complete the firmware setting by touching the **\[Apply]** button, the Config file set for the relevant slot will also be deleted. If you want to modify the communication firmware in the middle of using it, you need to back up the existing Config setting.
2. If you touch the **\[OK]** button without touching the **\[Apply]** button first, the set firmware will not be applied.
{% endhint %}

4\. **** Set the firmware for each slot by repeating Steps #2 and #3.

5\. **** The firmware will be applied when you turn the controller power off and then back on.

{% hint style="warning" %}
**\[Caution]**: When you set the use of the firmware, the setting values will be applied to the system only when you turn the controller power off and then back on.
{% endhint %}

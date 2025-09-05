# 1.3.1 Setting CIFX PCI Slot

Set the CIFX PCI slot communication method. After the settings are completed, restarting the controller's power to apply the settings will be necessary.

<br>

{% hint style="info" %}
\.      Refer to the following information.

\.      (“[**1.2.1 Industrial a PCI Communication Card**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)”)
{% endhint %}

<br>

##### 1. Click the menu to enter the slot setting screen.
**\[System > 2: Control Parameter > 11: Industrial Communication > 1: PCI Slot Setting > 1 Channel]**


<br>

##### 2. By referring to the screens shown below, select the slot, communication mode (master/slave), and protocol.
   * The slot number is the rotary switch number of the PCI communication card.
   * If you do not want to set the communication firmware, click the **\[OK]** button to end the process.

{% hint style="warning" %}
**\[Caution]**: Clicking the **\[Clear]** or **\[Apply]** buttons will initialize the PCI slot information on the tab you are currently viewing. Note that the Config file will be also initialized.  
{% endhint %}

![[Figure 1.3.1-1 PCI Slot Setting]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[Figure 1.3.1-2 PCI Slot Setting (master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[Figure 1.3.1-3 PCI Slot Setting (slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

##### 3. Complete the slot settings. 
Click on the **\[Apply]** button.

![[Figure 1.3.1-4 PCI Slot Setting]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[Caution]**

<1>. When you finish setting up the slot by clicking the **\[Apply]** button, all Config files set in the corresponding slots will be deleted. When required to change the communication during use, back up the current Config settings separately.

<2>. If you click the **\[OK]** button without clicking the **\[Apply]** button first, the set will not be applied.
{% endhint %}

<br>

##### 4. Repeat steps 2 and 3 for each slot to set.

<br>

##### 5. Reboot the Controller for the setting to be applied.
Click the menu under **\[Service > 19: Industrial Communication Monitoring]** to check if the set communication has been applied.

![[Figure 1.3.1-5 Industrial Communication Setting Screen]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[Caution]**: When you set the use of the slot, you must Reboot Controller to apply the settings to the system.
{% endhint %}

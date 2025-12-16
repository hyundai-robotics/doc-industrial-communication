# 1.3.1 CIFX PCI Slot Settings.

Configure the communication method for the CIFX PCI slot. To apply the settings, please disconnect the controller power and then supply it again.

<br>

Refer to "[**1.2.1 PCI Industrial Communication Card**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" and proceed with the method below.

<br>

##### 1. Touch the menu to enter the slot settings screen.
**\[System > 2: Control Parameters > 11: Industrial Communication > 1: PCI Slot Settings > Channel 1]** 


<br>

##### 2. Refer to the screen below to select the slot, communication method (master/slave), and protocol.
   * The slot number is the rotary switch number of the PCI communication card.
   * If you do not want to change the communication settings, touch the **\[OK]** button to exit.

{% hint style="warning" %}
**\[Caution]**: Touching the **\[Initialize]** or **\[Apply]** button will initialize the slot information on the current tab. The Config file will also be initialized, so please be aware.
{% endhint %}

![[Figure 1.3.1-1 PCI Slot Settings]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[Figure 1.3.1-2 PCI Slot Settings (master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[Figure 1.3.1-3 PCI Slot Settings (Slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

##### 3. Complete the slot settings.
Touch the **\[Apply]** menu.

![[Figure 1.3.1-4 PCI Slot Settings]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[Caution]**

<1>. When applying the settings by touching the **\[Apply]** button, all CONFIG files applied to the corresponding slot will be deleted and changed. It is recommended to keep a separate backup of existing settings when changing communication.

<2>. If you touch the **\[OK]** button without touching the **\[Apply]** button, the selected communication will not be applied.
{% endhint %}

<br>

##### 4. Repeat steps 2. \~ 3. for each slot.

<br>

##### 5. Reboot the controller to apply the set communication.
Touch the **\[Service > 19: Industrial Communication Monitoring]** menu to check if the set communication has been applied.

![[Figure 1.3.1-5 Industrial Communication Settings Screen]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[Caution]**: Settings are applied when the controller is rebooted after slot settings.
{% endhint %}

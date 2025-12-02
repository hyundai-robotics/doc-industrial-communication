# 1.3.1 CIFX PCI Slot Settings.

Configure the communication method for the CIFX PCI slot. To apply the settings, please disconnect the controller power and then supply it again.

<br>

“[Refer to "**1.2.1 PCI Industrial Communication Card**" and proceed with the method below.](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" 참고하여 아래 방법을 진행해 주십시오.

<br>

##### 1. Touch the menu to enter the slot settings screen.
*\[System > 2: Control Parameters > 11: Industrial Communication > 1: PCI Slot Settings > Channel 1]**


<br>

##### 2. Refer to the screen below to select the slot, communication method (master/slave), and protocol.
   * The slot number is the rotary switch number of the PCI communication card.
   * 통신 설정 변경을 원하지 않을 경우 **If you do not want to change the communication settings, touch the \[OK] button to exit.** 버튼을 터치하여 종료합니다.

{% hint style="warning" %}
* *\[주의]***\[Caution]: Touching the \[Initialize] or \[Apply]** button will initialize the slot information on the current tab. The Config file will also be initialized, so please be aware.**\[초기화]***\[Caution]: Touching the \[Initialize] or \[Apply]** button will initialize the slot information on the current tab. The Config file will also be initialized, so please be aware.**\[적용]** 버튼을 터치하면 현재 탭의 슬롯 정보가 초기화 됩니다. Config 파일도 같이 초기화 되니 유의하시기 바랍니다.
{% endhint %}

![[Figure 1.3.1-1 PCI Slot Settings]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[Figure 1.3.1-2 PCI Slot Settings(master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[Figure 1.3.1-3 PCI Slot Settings(Slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

##### 3. Complete the slot settings.
Touch the *\[Apply]** menu.

![[Figure 1.3.1-4 PCI Slot Settings]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
*\[Caution]**

<1>. **<1>. When applying the settings by touching the \[Apply] button, all CONFIG files applied to the corresponding slot will be deleted and changed. It is recommended to keep a separate backup of existing settings when changing communication.** 버튼을 터치하여 설정 시 해당 슬롯에 적용 되어있는 CONFIG 파일이 모두 삭제된 후 변경됩니다. 통신을 변경 하실 경우 기존 설정을 별도로 보관하는 것을 권장합니다.

<2>. **<2>. If you touch the \[OK] button without touching the \[Apply] button, the selected communication will not be applied.** 버튼을 터치하지 않고 **<2>. If you touch the \[OK] button without touching the \[Apply] button, the selected communication will not be applied.**버튼을 터치할 경우 선택한 통신이 적용되지 않습니다.
{% endhint %}

<br>

##### 4. Repeat steps 2. \~ 3. for each slot.

<br>

##### 5. Reboot the controller to apply the set communication.
Touch the *\[Service > 19: Industrial Communication Monitoring]** menu to check if the set communication has been applied.

![[Figure 1.3.1-5 Industrial Communication Settings Screen]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
*\[Caution]**: Settings are applied when the controller is rebooted after slot settings.
{% endhint %}

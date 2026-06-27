### 1.3.1 CIFX PCI 插槽设置

配置 CIFX PCI 插槽的通信方法。要应用设置，请断开控制器电源，然后再重新供电。

<br>

请参阅 "[1.2.1 PCI 工业通信卡](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" 并按照以下方法进行操作。

<br>

**1. 触摸菜单以进入插槽设置屏幕。**
**\[System > 2: Control Parameters > 11: Industrial Communication > 1: PCI Slot Settings > Channel 1]**

<br>

**2. 请参阅以下屏幕以选择插槽、通信方法（主/从）和协议。**
   * 插槽编号是 PCI 通信卡的旋钮开关编号。
   * 如果您不想更改通信设置，请触摸 **\[OK]** 按钮以退出。

{% hint style="warning" %}
**\[注意]**: 触摸 **\[Initialize]** 或 **\[Apply]** 按钮将初始化当前选项卡上的插槽信息。配置文件也将被初始化，请注意。
{% endhint %}

![[Figure 1.3.1-1 PCI 插槽设置]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[Figure 1.3.1-2 PCI 插槽设置（主）]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[Figure 1.3.1-3 PCI 插槽设置（从）]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

**3. 完成插槽设置。**
触摸 **\[Apply]** 菜单。

![[Figure 1.3.1-4 PCI 插槽设置]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[注意]**

<1>. 当通过触摸 **\[Apply]** 按钮应用设置时，所有应用于相应插槽的 CONFIG 文件将被删除并更改。建议在更改通信时保留现有设置的单独备份。

<2>. 如果在未触摸 **\[Apply]** 按钮的情况下触摸 **\[OK]** 按钮，则选定的通信将不被应用。
{% endhint %}

<br>

**4. 为每个插槽重复步骤 2. ~ 3.。**

<br>

**5. 重启控制器以应用设置的通信。**
触摸 **\[Service > 19: Industrial Communication Monitoring]** 菜单以检查设置的通信是否已应用。

![[Figure 1.3.1-5 工业通信设置屏幕]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)

{% hint style="warning" %}
**\[注意]**: 当插槽设置后重启控制器时，设置将被应用。
{% endhint %}
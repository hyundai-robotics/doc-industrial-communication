# 1.3.1 CIFX PCI插槽设置。

设置CIFX PCI插槽的通信方式。为了应用设置，请先切断控制器电源后再重新供电。

<br>

请参考“[**1.2.1 PCI 工业通信卡**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)”后，按照以下方法进行操作。

<br>

##### 1. 触摸菜单来进入插槽设置界面。
**\[系统 > 2: 控制参数 > 11: 工业通信 > 1: PCI插槽设置 > 1 通道]** 


<br>

##### 2. 请参考下面的画面，选择插槽、通信方式（Master/Slave）及协议。
   * 插槽编号是PCI通信卡的Rotary Swtich编号。
   * 如不需要更改通信设置，请触摸 **\[OK]** 按钮来退出。

{% hint style="warning" %}
**\[注意]**：触摸 **\[初始化]** 或 **\[应用]** 按钮时，当前选项卡中的插槽信息将被初始化。Config 文件也会一并初始化，请务必注意。
{% endhint %}

![[图1.3.1-1 PCI 插槽设置]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[图 1.3.1-2 PCI 插槽设置（master）]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[图 1.3.1-3 PCI 插槽设置（Slave）]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

##### 3. 完成插槽设置。
触摸 **\[应用]** 菜单

![[图 1.3.1-4 PCI 插槽设置]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[注意]**

<1>. 触摸 **\[应用]** 按钮进行设置时，已应用于该插槽的 CONFIG 文件将被全部删除后再更改。若要更改通信，建议单独备份现有设置。

<2>. 若未触摸 **\[应用]** 按钮而触摸 **\[OK]** 按钮，则所选的通信将不会被应用。
{% endhint %}

<br>

##### 4. 对每个插槽重复执行上述2. \~ 3.号步骤的设置。

<br>

##### 5. 重启控制器以应用已设置的通信。
触摸 **\[服务 > 19: 工业通信监控]** 菜单，确认所设置的通信是否已被应用。

![[图1.3.1-5 工业通信设置界面]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
**\[注意]**：插槽设置后，重启控制器时，设定值才会生效。
{% endhint %}

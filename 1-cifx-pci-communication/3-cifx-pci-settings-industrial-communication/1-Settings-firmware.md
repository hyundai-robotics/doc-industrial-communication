### 1.3.1 CIFX PCI插槽设置

配置CIFX PCI插槽的通信方法。要应用设置，请断开控制器电源，然后重新供电。

<br>

请参考"[**1.2.1 PCI工业通信卡**](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)"并按照以下方法进行操作。

<br>

**1. 点击菜单进入插槽设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 1: PCI插槽设置 > 通道1]** 

<br>

**2. 请参考下面的屏幕选择插槽、通信方法（主/从）和协议。**
   * 插槽号是PCI通信卡的旋转开关编号。
   * 如果您不想更改通信设置，请点击**\[确定]**按钮退出。

{% hint style="warning" %}
**\[注意]**: 点击**\[初始化]**或**\[应用]**按钮将初始化当前选项卡上的插槽信息。配置文件也将被初始化，请注意。
{% endhint %}

![[图 1.3.1-1 PCI插槽设置]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[图 1.3.1-2 PCI插槽设置（主）]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[图 1.3.1-3 PCI插槽设置（从）]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

**3. 完成插槽设置。**
点击**\[应用]**菜单。

![[图 1.3.1-4 PCI插槽设置]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
**\[注意]**

<1>. 当通过点击**\[应用]**按钮来应用设置时，所有应用于相应插槽的CONFIG文件将被删除并更改。建议在更改通信时保留现有设置的单独备份。

<2>. 如果您在未点击**\[应用]**按钮的情况下点击**\[确定]**按钮，所选的通信将不会被应用。
{% endhint %}

<br>

**4. 对每个插槽重复步骤2. ~ 3.**

<br>

**5. 重新启动控制器以应用所设置的通信。**
点击**\[服务 > 19: 工业通信监控]**菜单以检查所设置的通信是否已被应用。

![[图 1.3.1-5 工业通信设置屏幕]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)

{% hint style="warning" %}
**\[注意]**: 在插槽设置后，重新启动控制器时会应用设置。
{% endhint %}
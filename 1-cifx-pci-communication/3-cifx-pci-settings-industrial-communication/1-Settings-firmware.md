# 1.3.1 CIFX PCI插槽设置

设置CIFX PCI插槽的通信方式。为了应用设置，请先切断控制器电源后再重新供电。

<br>

“[请参考“**1.2.1 PCI 工业通信卡**”后，按照以下方法进行操作。](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" 참고하여 아래 방법을 진행해 주십시오.

<br>

##### 1. 触摸菜单来进入插槽设置界面。
\[系统 > 2: 控制参数 > 11: 工业通信 > 1: PCI插槽设置 > 1 通道]*


<br>

##### 2. 请参考下面的画面，选择插槽、通信方式（Master/Slave）及协议。
   * 插槽编号是PCI通信卡的Rotary Swtich编号。
   * 통신 설정 변경을 원하지 않을 경우 **如不需要更改通信设置，请触摸\[OK]按钮来退出。** 버튼을 터치하여 종료합니다.

{% hint style="warning" %}
* *\[주의]***\[注意]: 触摸\[初始化] 或 \[应用]** 按钮时，当前选项卡中的插槽信息将被初始化。Config文件也会一并初始化，请务必注意。**\[초기화]***\[注意]: 触摸\[初始化] 或 \[应用]** 按钮时，当前选项卡中的插槽信息将被初始化。Config文件也会一并初始化，请务必注意。**\[적용]** 버튼을 터치하면 현재 탭의 슬롯 정보가 초기화 됩니다. Config 파일도 같이 초기화 되니 유의하시기 바랍니다.
{% endhint %}

![[图1.3.1-1 PCI 插槽设置]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_1.png>)

![[图 1.3.1-2 PCI 插槽设置(master)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_2.png>) ![[图 1.3.1-3 PCI 插槽设置(Slave)]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_3.png>)

<br>

##### 3. 完成插槽设置。
触摸*\[应用]** 菜单

![[图 1.3.1-4 PCI 插槽设置]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_4.png>)

{% hint style="warning" %}
*\[注意]**

<1>. **<1>. 触摸\[应用]按钮进行设置时，已应用于该插槽的CONFIG文件将被全部删除后再更改。若要更改通信，建议单独备份现有设置。** 버튼을 터치하여 설정 시 해당 슬롯에 적용 되어있는 CONFIG 파일이 모두 삭제된 후 변경됩니다. 통신을 변경 하실 경우 기존 설정을 별도로 보관하는 것을 권장합니다.

<2>. **<2>. 若未触摸\[应用]按钮而触摸\[OK]按钮，则所选的通信将不会被应用。** 버튼을 터치하지 않고 **<2>. 若未触摸\[应用]按钮而触摸\[OK]按钮，则所选的通信将不会被应用。**버튼을 터치할 경우 선택한 통신이 적용되지 않습니다.
{% endhint %}

<br>

##### 4. 对每个插槽重复执行上述2. \~ 3.号步骤的设置。

<br>

##### 5. 重启控制器以应用已设置的通信。
触摸*\[服务 > 19: 工业通信监控]**菜单，确认所设置的通信是否已被应用。

![[图1.3.1-5 工业通信设置界面]](<../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Setting-Firmware/image_5.png>)



{% hint style="warning" %}
*\[注意]**: 插槽设置后，重启控制器时，设定值才会生效。
{% endhint %}

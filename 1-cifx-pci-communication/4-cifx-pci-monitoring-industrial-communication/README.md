## 1.4 CIFX PCI 通信监控

<br>

按照 "[1.2 CIFX PCI - 安装和设置工业通信卡](../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/1-PCI-industrial-communication-card.md)" 和 "[1.3 CIFX PCI - 设置工业通信](../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 的程序设置通信后，可以在以下屏幕中查看操作。

<br>

**1. 工业通信监控**

<br>

通过触摸 **\[服务 > 19: 工业通信监控]** 进入屏幕，并在相关屏幕中检查设置的固件信息、通信状态和通信配置等详细信息。

<br>

{% hint style="info" %}
   - 使用 **\[重启]** 按钮可重启 PCI 通信卡的工业通信。

   - 请检查插槽、固件和设备的状态。

   - 对于主设备，请检查配置和活动从设备的数量是否与配置的从设备数量相匹配。
{% endhint %}

<br>

![[Figure 1.4-1 工业通信监控]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_1.png>)

<br>

{% hint style="info" %}
   [状态信息]   
      - 通信: 通信链路已建立，I/O 数据正在交换   
      - 运行: 通信卡 (PCI) 正在运行   
      - 就绪: 通信处于待机状态   
      - 错误: 通信错误状态   

      - 通信错误: 通信过程中发生的错误代码   
      - 错误计数: 累计的通信错误数量   
      - 活动从设备: 当前连接并交换 I/O 数据的从设备数量   
      - 配置从设备: 配置用于通信的从设备数量   
      - 诊断从设备: 处于通信诊断中的从设备数量   
      - 看门狗时间 (毫秒): 监控通信程序活动的超时值   
{% endhint %}

<br>

**2. 工业通信节点监控**

<br> 

点击监控屏幕底部的节点状态按钮以监控连接到主协议的设备状态

<br>

![[Figure 1.4-2 工业通信监控]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_2.png>)

{% hint style="info" %}
   [节点状态信息]   
      - 绿色: 节点当前已连接并交换 I/O 数据   
      - 红色: 节点已配置但未连接   
{% endhint %}

<br>

{% hint style="info" %}
   - 在 DeviceNet 主设备的情况下，可以通过扫描节点信息列表进行监控
{% endhint %}

<br>

![[Figure 1.4-3 工业通信监控]](<../../_assets/1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/image_3.png>)
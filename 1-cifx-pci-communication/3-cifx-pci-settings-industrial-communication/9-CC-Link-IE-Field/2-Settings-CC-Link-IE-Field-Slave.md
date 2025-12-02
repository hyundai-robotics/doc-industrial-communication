# 1.3.9.2 CC-Link IE Field Slave设置

“[请按照“**1.3.1 CIFX PCI槽位设置**”流程设置后，再按以下方法进行操作。](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.


<br>

##### 1. 使用TP在工业通信固件设置中选择CC-Link IE Field Slave，并重启机器人控制器。

![[图 1.3.9.2-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_1.png>)

<br>

##### 2. 在工业通信监控中，确认当前所选通信协议的准备状态。

![[图 1.3.9.4-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_2.png>)

<br>

{% hint style="warning" %}
*\[注意]**: 如果用Sycon.net设置的Configuration文件已下载到该PCI插槽，则TP中的设定值将被忽略。
{% endhint %}

<br>

##### 3. 触摸菜单来进入从站设置界面。
*\[系统 > 2: 控制参数 > 11: 工业通信 > 2: PCI从站插槽设置 >  CC-Link IE Field Slave]**

![[图 1.3.9.4-3 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_3.png>)

![[图 1.3.9.4-4 从站设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_4.png>)

<br>

##### 4. 各项目说明

{% hint style="info" %}
\.      [Network Number]

\.      CC-Link IE Field network编号（1~239）
{% endhint %}

{% hint style="info" %}
\.      [Station Address]

\.      已连接网络内的设备ID（1 ~ 120）
{% endhint %}

{% hint style="info" %}
\.      [IO Type]

\.      IO Type由master设备设置决定。
\.      - Mixed：使用输入与输出不同的索引（不同地址）
\.      - Input：仅用于输入
\.      - Output：仅用于输出
\.      - FrontBackMixture：使用输入与输出相同的索引（相同地址）
{% endhint %}

{% hint style="info" %}
\.      [Device Type]

\.      根据Device Type可设置的IO最大大小不同。

\.      Intelligent Device Station
\.      - RY, RX (max): 256 bytes
\.      - RWw, RWr (max): 1024 words

\.      Remote Device Station
\.      - RY, RX (max): 16 bytes
\.      - RWw, RWr (max): 64 words
{% endhint %}

{% hint style="info" %}
\.      [IO Size]

\.      Master -> Slave
\.      - RWw (word data)
\.      - RY (bit data)

\.      Slave -> Master
\.      - RWr (word data)
\.      - RX (bit data)
{% endhint %}

<br>

##### 5. 设置完成后，请按照以下流程确认通信状态。

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[在TP上确认工业通信状态的程序，请参考（“**1.4 CIFX PCI 通信监控**”）。](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

<br>

##### 6. 通信设置完成后分配IO Block。

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[\.      **通信设置完成后，可以通过分配IO Block来使用输入输出信号。请确认（“**4. 工业通信IO Block分配**”）。**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}

<br>

![[图 1.3.9.4-5 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/9-CC-Link-IE-Field/4-Slave_setting/image_5.png>)
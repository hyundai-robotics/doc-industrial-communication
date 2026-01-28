#### 1.3.7.2 DeviceNet Master设置

请按照“[**1.3.1 CIFX PCI槽位设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)”及“[**1.3.2 SYCON.NET设置**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)”流程设置后，再按以下方法进行操作。

<br>

{% hint style="info" %}
\.      在使用SYCON.net过程中，如有说明书中解释不足的部分，请参考“[**1.3.2 SYCON.NET帮助**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)”功能。
{% endhint %}

<br>

{% hint style="info" %}
\.      关于DeviceNet连接器的连接，请参考以下内容。

\.      （[“**1.2.2 连接器**”](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)）
{% endhint %}

<br>

**1. 在工业通信固件设置中，选择DeviceNet Master并重启机器人控制器。**

![[图 1.3.7.2-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_1.png>) 

<br>

**2. 在工业通信监控中，确认所选协议的准备状态。**

![[图 1.3.7.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_2.png>) 

<br>

**3. 使用 Sycon.net 选择 DeviceNet Master PCI 设备。**

![[图 1.3.7.2-3 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_3.png>)
![[图 1.3.7.2-4 DeviceNet Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_4.png>) 

<br>

**4. 扫描 PCI 设备并应用 DeviceNet Master（Apply）。**

![[图 1.3.7.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_5.png>) 

<br>

**5. 设置通信速度。**

{% hint style="warning" %}
\.      如果Master与Slave的通信速度不同，Network Scan将无法正常进行。
{% endhint %}

![[图 1.3.7.2-6 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_6.png>) 

<br>

**6. 下载设置。**

![[图 1.3.7.2-7 DeviceNet Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_7.png>) 

<br>

**7. 准备所要连接到 DeviceNet Master 的 Slave 模块。**
   * 本示例中使用Crevis公司的NA-9211 DeviceNet Slave。
   * 请提供系统电源及现场电源以激活模块。

![[图 1.3.7.2-8 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_8.png>) 

<br>

**8. Slave设备设置**

{% hint style="info" %}
\.      设置DeviceNet Slave设备的MAC ID、通信速度、终端电阻。
{% endhint %}

![[图 1.3.7.2-9 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_9.png>) 

![[图 1.3.7.2-10 Crevis NA-9211]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_10.png>)

{% hint style="info" %}
\.      [示例设置]

\.      终端电阻：在电缆上安装终端电阻（终端DIP Switch OFF）

\.      MAC ID（Station Number）：设置为4（仅3号DIP Switch为ON）

\.      通信速度（Baudrate）：设置为Auto（7号、8号DIP Switch为ON）
{% endhint %}

<br>

**9. 注册Slave设备的EDS文件。**

{% hint style="info" %}
\.      要使用未注册到Sycon.net的Device，就需要EDS文件。

\.      NA-9211 Device 的 EDS 文件可以在 Crevis 官网下载。
{% endhint %}

![[图 1.3.7.2-11 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_11.png>)

{% hint style="info" %}
\.      将所下载的 EDS 文件全部注册到 Sycon.net。

\.      注册EDS File时，请确认工业通信协议（DeviceNet）。
{% endhint %}

![[图 1.3.7.2-12 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_12.png>)

<br>

![[图 1.3.7.5-13 Crevis EDS File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_13.png>)



<br>

**10. Network Scan**

{% hint style="warning" %}
\.      **当进行Network Scan时，请务必确认以下事项。**

\.      **（1） 电缆连接情况**  
\.      **（2） 终端电阻连接或终端DIP Switch使用情况**  
\.      **（3） Master - Slave通信速度设置情况**  

\.      **为了顺利连接通信，请务必确认（“[**1.3.7.5 DeviceNet ERROR处理**](../7-DeviceNet/5-Error-DeviceNet.md)”）。**
{% endhint %}

{% hint style="info" %}
\.      DeviceNet Master 支持 Network Scan 功能。
{% endhint %}

{% hint style="info" %}
\.      在 DeviceNet Master 设备上右击后点击 Network Scan。
{% endhint %}

![[图 1.3.7.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_14.png>)

{% hint style="warning" %}
\.      如果 EDS 文件未注册，当进行 Network Scan 时则会显示 Slave 信息，但无法注册。
{% endhint %}

{% hint style="info" %}
\.      正常注册EDS文件后，可以通过Network Scan添加Slave设备。
{% endhint %}

![[图 1.3.7.2-15 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_15.png>)

![[图 1.3.7.2-16 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_16.png>)

<br>

**11. Slave 设备 Configuration**

{% hint style="info" %}
\.      为了进行 Slave 设备 Configuration，点击 Master 设备的 Disconnect。
{% endhint %}

![[图 1.3.7.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_17.png>)

{% hint style="info" %}
\.      双击Slave设备。
{% endhint %}

![[图 1.3.7.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_18.png>)


<br>

{% hint style="info" %}
\.      设置Slave设备的连接类型。

\.      选择用于连接DeviceNet通信的消息传输方式。

\.      ** 当未勾选UCMM时，则设置为UCMM Group 2默认值。**   

\.      UCMM GROUP 1 : IO Message   
\.      UCMM GROUP 2：Network初始化时，Master - Slave连接Message（默认设置）
\.      UCMM GROUP 3：Explicit Message   

\.      某些Device可以使用UCMM Group 3，请确认产品规格书后进行。
{% endhint %}

![[图 1.3.7.2-19 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_19.png>)

<br>

{% hint style="info" %}
\.      Crevis NA-9211在未选中UCMM的情况下进行。（使用Group2默认值）
{% endhint %}

![[图 1.3.7.2-20 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_20.png>)

<br>


{% hint style="info" %}
\.      确认DeviceNet Slave的设置。

\.      Output：ST-2318（1 Byte）  
\.      Input：ST-1218（1 Byte）  
{% endhint %}

<br>

{% hint style="info" %}
\.      需要根据通信方式（Poll、Change of State、Cyclic、Bit-Strobe）进行设置  
{% endhint %}

<br>

![[图 1.3.7.2-21 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_21.png>)

<br>

{% hint style="info" %}
\.      [Production Inhibit Time]

\.      设置从站设备的IO数据生成周期（ms）  
\.  
\.      示例）10ms：以10ms周期生成IO数据  
\.      示例）0ms：Slave在可能的最快时间内生成IO数据  

\.      周期越短，Slave设备的负载可能越大。（需确认各Slave的规格） 
{% endhint %}

<br>

{% hint style="info" %}
\.      [Expected Packet Rate]

\.      设置主站与从站之间的IO数据更新时间  
{% endhint %}

<br>

![[图 1.3.7.2-22 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_22.png>)



<br>

**12. Master 设备 Configuration**

{% hint style="info" %}
\.      双击Master设备。
{% endhint %}

![[图 1.3.7.2-23 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_23.png>)


{% hint style="info" %}
\.      设置DeviceNet通信速度。（与Slave通信速度相同）
{% endhint %}

![[图 1.3.7.2-24 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.      请在Address Table中确认各Slave Slot分配的IO及起始地址。
{% endhint %}

![[图 1.3.7.2-25 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_25.png>)

{% hint style="info" %}
\.      设置 Quick Connect 功能的使用与否。
{% endhint %}

![[图 1.3.7.2-26 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_26.png>)


{% hint style="info" %}
\.      设置完成后，请进行 Download。
{% endhint %}

![[图 1.3.7.2-27 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_27.png>)

<br>

**13. 通信状态确认**

{% hint style="info" %}
\.      在Sycon.net及TP上确认通信状态。

\.        在TP上确认工业通信状态的程序，请参考（“[**1.4 CIFX PCI 通信监控**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”）。
{% endhint %}

{% hint style="info" %}
\.      双击已Connected的Master设备，可以确认通信状态。
{% endhint %}

![[图 1.3.7.2-28 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_28.png>)

![[图 1.3.7.2-29 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_29.png>)

{% hint style="info" %}
\.        可以利用Sycon.net的Diagnosis功能，监控通信状态及IO输入输出状态。
{% endhint %}

![[图 1.3.7.2-30 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/2-Master_setting/image_30.png>)

<br>

**14. 通信设置完成后分配IO Block。**

{% hint style="info" %}
\.      **通信设置完成后，可以通过分配IO Block来使用输入输出信号。请确认（“[**4. 工业通信IO Block分配**](../../../4-io-block-allocation.md)”）。**
{% endhint %}
# 1.3.5.2 EtherCAT Master设置

“[请按照“**1.3.1 CIFX PCI槽位设置**”及“**1.3.2 SYCON.NET设置**”流程设置后，再按以下方法进行操作。](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 및 "[请按照“**1.3.1 CIFX PCI槽位设置**”及“**1.3.2 SYCON.NET设置**”流程设置后，再按以下方法进行操作。](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      SYCON.net 이용 중 매뉴얼에 설명이 부족한 부분은  ""[\.      在使用SYCON.net过程中，如有说明书中解释不足的部分，请参考“**1.3.2 SYCON.NET帮助**”功能。](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)"" 기능을 참고해 주십시오.
{% endhint %}

<br>

##### 1. 在工业通信固件设置中，选择EtherCAT Master并重启机器人控制器。

![[图 1.3.5.2-1 固件设置]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_1.png>)

<br>

##### 2. 在工业通信监控中，确认所选协议的准备状态。

![[图 1.3.5.2-2 工业通信监控]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_2.png>)

<br>

##### 3. 使用Sycon.net选择EtherCAT Master PCI设备。

![[图 1.3.5.2-3 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_3.png>)
![[图 1.3.5.2-4 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_4.png>)

<br>

##### 4. 扫描PCI设备并应用EtherCAT Master（Apply）。

![[图 1.3.5.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_5.png>)

<br>

##### 5. 下载设置。

![[图 1.3.5.2-6 EtherCAT Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_6.png>)

<br>

##### 6. 准备所要连接到EtherCAT Master的Slave模块。
   * 本示例中使用Crevis公司的M9386 EtherCAT Slave。
   * 请提供系统电源及现场电源以激活模块。

![[图 1.3.5.2-7 Crevis M9386]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_7.png>)

<br>

##### 7. Slave设备的Station Address

{% hint style="info" %}
\.      EtherCAT Slave设备的Station Address在Master中设置。
{% endhint %}

<br>

##### 8. 注册Slave设备的XML文件。

{% hint style="info" %}
\.      要使用未注册到Sycon.net的Device，就需要XML文件。

\.      M9386 Device的XML文件可以在Crevis官网下载。
{% endhint %}

![[图 1.3.5.2-8 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_8.png>)

{% hint style="info" %}
\.      将所下载的XML文件注册到Sycon.net。

\.      注册XML File时，请确认工业通信协议（EtherCAT）。
{% endhint %}

![[图 1.3.5.2-9 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_9.png>)

<br>

![[图 1.3.5.5-10 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_10.png>)

<br>

![[图 1.3.5.2-11 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_11.png>)

<br>

![[图 1.3.5.2-12 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_12.png>)


<br>

##### 9. Network Scan

{% hint style="warning" %}
\.      **\.      EtherCAT可使用的电缆接线和端口已指定。**

\.      **원활한 통신 연결을 위해 (“[\.      **为了顺利连接通信，请务必确认（“**1.3.5.5 EtherCAT电缆接线**”）。**](../5-EtherCAT/5-EtherCAT-Topology.md)”)을 반드시 확인해 주십시오.**
{% endhint %}

{% hint style="info" %}
\.      EtherCAT Master支持Network Scan功能。
{% endhint %}

{% hint style="info" %}
\.      在EtherCAT Master设备上右击后，点击Network Scan。
{% endhint %}

![[图 1.3.5.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_13.png>)

{% hint style="warning" %}
\.      如果XML文件未注册，当进行Network Scan时则会显示Slave信息，但无法注册。
{% endhint %}

{% hint style="info" %}
\.      正常注册XML文件后，可以通过Network Scan添加Slave设备。
{% endhint %}

![[图 1.3.5.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_14.png>)

<br>

##### 10. Slave设备Configuration

{% hint style="info" %}
\.      为了进行Slave设备Configuration，点击Master设备的Disconnect。
{% endhint %}

![[图 1.3.5.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_15.png>)

{% hint style="info" %}
\.      双击Slave设备。
{% endhint %}

![[图 1.3.5.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_16.png>)

{% hint style="info" %}
\.      为了设置EtherCAT Slave，添加连接到M9386的Slot。

\.      Slot 1 : M7001
\.      Slot 2 : M12DF
\.      Slot 3 : M225F
{% endhint %}

![[图 1.3.5.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_17.png>)

![[图 1.3.5.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_18.png>)


<br>

##### 11. Master设备Configuration

{% hint style="info" %}
\.      双击Master设备。
{% endhint %}

![[图 1.3.5.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_19.png>)

{% hint style="info" %}
\.      Synchronization：选择Freerun / DC（Distributed Clocks）

\.      Redundancy使用与否（不可与Distributed Clocks一并使用）

\.      Bus Cycle Time：可支持最小250us（建议1ms以上）
{% endhint %}

<br>

{% hint style="info" %}
\.      可设置各Slave的Station Address。
{% endhint %}

![[图 1.3.5.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_20.png>)

{% hint style="info" %}
\.      请在Address Table中确认各Slave Slot分配的IO及起始地址。
{% endhint %}

![[图 1.3.5.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_21.png>)


{% hint style="info" %}
\.      设置完成后，请进行Download。
{% endhint %}

![[图 1.3.5.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_22.png>)

<br>

##### 12. 通信状态确认

{% hint style="info" %}
\.      在Sycon.net及TP上确认通信状态。

\.        TP 에서 산업용 통신 상태를 확인하는 절차는 (“[\.      在TP上确认工业通信状态的程序，请参考（“1.4 CIFX PCI 通信监控”）。](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.
{% endhint %}

{% hint style="info" %}
\.      双击已Connected的Master设备，可以确认通信状态。
{% endhint %}

![[图 1.3.5.2-23 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_23.png>)

![[图 1.3.5.2-24 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_24.png>)

{% hint style="info" %}
\.      可以利用Sycon.net的Diagnosis功能，监控通信状态及IO输入输出状态。
{% endhint %}

![[图 1.3.5.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_25.png>)

<br>

##### 13. 通信设置完成后分配IO Block。

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[\.      **通信设置完成后，可以通过分配IO Block来使用输入输出信号。请确认（“**4. 工业通信IO Block分配**”）。**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
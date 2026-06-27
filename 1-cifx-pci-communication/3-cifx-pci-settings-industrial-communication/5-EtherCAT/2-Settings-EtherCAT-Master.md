#### 1.3.5.2 EtherCAT 主设置

Please follow the "[1.3.1 CIFX PCI Slot Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" and "[1.3.2 SYCON.NET Settings](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/README.md)" procedures and then proceed with the method below.

<br>

{% hint style="info" %}
   - When using SYCON.net, if there are insufficient explanations in the manual, please refer to the "[1.3.2 SYCON.NET Help](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/2-Settings-SYCON/1-Help-SYCON.md)" function.
{% endhint %}

<br>

**1. 在 PCI 插槽设置中选择 EtherCAT 主控并重启机器人控制器。**

![[Figure 1.3.5.2-1 PCI slot Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_1.png>) 

<br>

**2. 在工业通信监控菜单中检查所选协议的就绪状态。**

<br>

{% hint style="info" %}
   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

<br>

![[Figure 1.3.5.2-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_2.png>) 

<br>

**3. 使用 Sycon.net 选择 EtherCAT 主控 PCI 设备。**

![[Figure 1.3.5.2-3 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_3.png>)
![[Figure 1.3.5.2-4 EtherCAT Master PCI]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_4.png>) 

<br>

**4. 扫描 PCI 设备并应用 EtherCAT 主控。**

![[Figure 1.3.5.2-5 Sycon.net Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_5.png>) 

<br>

**5. 下载设置。**

![[Figure 1.3.5.2-6 EtherCAT Master Download]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_6.png>) 

<br>

**6. 准备要连接到 EtherCAT 主控的从模块。**
   * 在此示例中，我们使用 Crevis 的 M9386 EtherCAT 从设备。
   * 请提供系统电源和现场电源以启用模块。

![[Figure 1.3.5.2-7 Crevis M9386]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_7.png>) 

<br>

**7. 从设备站地址**

{% hint style="info" %}
   - The station address of the EtherCAT slave device is set by the master.
{% endhint %}

<br>

**8. 注册从设备 XML 文件。**

{% hint style="info" %}
   - An XML file is required to use a device not registered in Sycon.net.

   - The XML file for the M9386 device can be downloaded from the Crevis website.
{% endhint %}

![[Figure 1.3.5.2-8 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_8.png>)

{% hint style="info" %}
   - Register the downloaded XML file in Sycon.net.

   - When registering an XML File, please check the industrial communication Protocol (EtherCAT).
{% endhint %}

![[Figure 1.3.5.2-9 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_9.png>)

<br>

![[Figure 1.3.5.5-10 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_10.png>)

<br>

![[Figure 1.3.5.2-11 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_11.png>)

<br>

![[Figure 1.3.5.2-12 Crevis XML File]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_12.png>)


<br>

**9. 网络扫描**

{% hint style="warning" %}
   **对于 EtherCAT，可用的电缆连接和端口已指定。**

   **为了确保顺畅的通信连接，请务必检查 ("[1.3.5.5 EtherCAT Cable Wiring](../5-EtherCAT/5-EtherCAT-Topology.md)")。**
{% endhint %}

{% hint style="info" %}
   - The EtherCAT master supports the Network Scan function.
{% endhint %}

{% hint style="info" %}
   - Right-click the EtherCAT master device and click Network Scan.
{% endhint %}

![[Figure 1.3.5.2-13 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_13.png>)

{% hint style="warning" %}
   - If there is no XML file registered, the slave information will appear when the Network Scan function is performed, but registration is not possible.
{% endhint %}

{% hint style="info" %}
   - If an XML file is normally registered, a slave device can be added using the Network Scan function.
{% endhint %}

![[Figure 1.3.5.2-14 Network Scan]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_14.png>)

<br>

**10. 配置从设备。**

{% hint style="info" %}
   - Click Disconnect on the master device to configure the slave device.
{% endhint %}

![[Figure 1.3.5.2-15 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_15.png>)

{% hint style="info" %}
   - Double-click the slave device.
{% endhint %}

![[Figure 1.3.5.2-16 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_16.png>)

{% hint style="info" %}
   - Add a slot connected to M9386 to set the EtherCAT slave.

   - Slot 1 : M7001  
   - Slot 2 : M12DF  
   - Slot 3 : M225F  
{% endhint %}

![[Figure 1.3.5.2-17 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_17.png>)

![[Figure 1.3.5.2-18 Slave Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_18.png>)


<br>

**11. 配置主设备。**

{% hint style="info" %}
   - Double-click the Master device.
{% endhint %}

![[Figure 1.3.5.2-19 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_19.png>)

{% hint style="info" %}
   - Synchronization: Select Freerun/DC (Distributed Clocks).

   - Whether to use Redundancy (cannot be used together with Distributed Clocks)

   - Bus Cycle Time: At least 250 us is supported. (1 ms or more is recommended.)
{% endhint %}

<br>

{% hint style="info" %}
   - You can set the station address for each slave.
{% endhint %}

![[Figure 1.3.5.2-20 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_20.png>)

{% hint style="info" %}
   - Check the assigned IO and start address for each slave slot in the address table.
{% endhint %}

![[Figure 1.3.5.2-21 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_21.png>)


{% hint style="info" %}
   - After completing settings, proceed with downloading.
{% endhint %}

![[Figure 1.3.5.2-22 Master Configuration]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_22.png>)

<br>

**12. 检查通信状态。**

{% hint style="info" %}
   - Check the communication status in Sycon.net and TP.

   - For the procedure to check the industrial communication status on the TP, please refer to ("[1.4 CIFX PCI Communication Monitoring](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").
{% endhint %}

{% hint style="info" %}
   - Double-click the connected master device to check the communication status.
{% endhint %}

![[Figure 1.3.5.2-23 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_23.png>)

![[Figure 1.3.5.2-24 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_24.png>)

{% hint style="info" %}
   - Using the Sycon.net's diagnosis function, you can monitor the communication status and input/output status.
{% endhint %}

![[Figure 1.3.5.2-25 Status Diagnosis]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/5-EtherCAT/2-Master_setting/image_25.png>)

<br>

**13. 在完成设置后分配 IO 块。**

{% hint style="info" %}
   **在完成通信设置后，您可以通过分配 IO 块来使用输入/输出信号。请参考 ("[5. Industrial Communication IO Reading and Writing](../../../5-io-block-allocation.md)")。**
{% endhint %}
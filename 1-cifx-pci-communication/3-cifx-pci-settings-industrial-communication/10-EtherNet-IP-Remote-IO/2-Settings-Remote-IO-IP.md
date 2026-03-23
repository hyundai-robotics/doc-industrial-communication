#### 1.3.10.2 远程 IO IP 地址设置

这是如何设置 Crevis 的 M9289 EtherNet/IP 网络适配器的 IP 地址。

<br>

{% hint style="info" %}
   - Crevis M9289 远程 IO 的出厂默认 IP 是 192.168.100.99。

   - 如果您不知道远程 IO IP 或需要更改它，请遵循以下步骤。
{% endhint %}

<br>

**1. 使用 LAN 电缆直接连接 PC 和远程 IO。**

![[Figure 1.3.10.2-1 LAN Connection]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

**2. 将远程 IO 适配器的 DIP 开关 9 仅更改为 ON。**

![[Figure 1.3.10.2-2 DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

**3. 执行 Bootpsvr.exe 程序。**
   * 该程序由 Crevis 提供。 （从网站下载并安装 IO Guide Pro。）

![[Figure 1.3.10.2-3 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[Figure 1.3.10.2-4 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
   - 按下“启动 BootP”后，断开并重新施加电源以重启 M9289 模块。
{% endhint %}

![[Figure 1.3.10.2-5 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>

**4. 当适配器设备重启时，设备信息将在 BootpSvr.exe 程序中显示。**

![[Figure 1.3.10.2-6 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

**5. 选择设备并设置 IP。**

![[Figure 1.3.10.2-7 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[Figure 1.3.10.2-8 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

**6. 完成 IP 设置后，将适配器的所有 DIP 开关切换为 OFF 并重启设备。**

{% hint style="info" %}
   - 一定要检查 DIP 开关状态及适配器是否已重启。
{% endhint %}

![[Figure 1.3.10.2-9 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

**7. 在 PC 上使用 ping 测试等验证 IP。**

![[Figure 1.3.10.2-10 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

**8. 如果 IP 地址已成功更改，请继续进行设置。**

{% hint style="info" %}
   - 请根据 "[**1.3.10.1 EtherNet/IP - 标准远程 IO 连接设置**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)" 程序进行设置。
{% endhint %}
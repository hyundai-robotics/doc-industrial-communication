#### 1.3.10.2 Remote IO IP地址设置

这是Crevis M9289 EtherNet/IP Network Adapter的IP地址设置方法。

<br>

{% hint style="info" %}
\.      Remote IO Crevis M9289的出厂设置IP（默认值）为192.168.100.99。

\.      如果不知道Remote IO的IP或需要更改，请按照以下方法进行操作。
{% endhint %}

<br>

**1. 请用LAN电缆将PC与Remote IO直接连接。**

![[图1.3.10.2-1 LAN连接]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_1.png>)  

<br>

**2. 仅将Remote IO Adapter的9号DIP Switch更改为ON。**

![[图 1.3.10.2-2 DIP Switch]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_2.png>)  

<br>

**3. 执行Bootpsvr.exe程序。**
   * 该程序由Crevis公司提供。（在官网下载IO Guide Pro后安装）

![[图 1.3.10.2-3 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_3.png>)  

![[图 1.3.10.2-4 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_4.png>)  

<br>

{% hint style="info" %}
\.      在按住Start BootP的状态下，断开M9289模块的电源并重新供电以重启。
{% endhint %}

![[图 1.3.10.2-5 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_5.png>)  

<br>


**4. 重启Adapter设备后，在BootpSvr.exe程序中会显示Device信息。**

![[图 1.3.10.2-6 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_6.png>) 

<br>

**5. 选择Device来设置IP。**

![[图 1.3.10.2-7 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_7.png>)
![[图 1.3.10.2-8 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_8.png>) 

<br>

**6. IP设置完成后，将Adapter的DIP Switch全部更改为OFF后重启设备。**

{% hint style="info" %}
\.      请务必确认DIP Switch的状态及Adapter是否重启。
{% endhint %}

![[图 1.3.10.2-9 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_9.png>) 

<br>

**7. 在PC上使用Ping Test等确认IP。**

![[图 1.3.10.2-10 Bootp]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-IP-Setting/image_10.png>) 

<br>

**8. 如果IP地址正常更改，请进行设置。**

{% hint style="info" %}
\.      请按照“[**1.3.10.1 EtherNet/IP - 标准Remote IO连接设置**](../../3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/1-Settings-EtherNet-IP-Remote-IO.md)”流程进行设置。
{% endhint %}

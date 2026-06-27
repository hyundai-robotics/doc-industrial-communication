## 2.1 网络设置

**1. 主模块**

<br>

可以与 EtherNet/IP 适配器连接的 LAN 端口是 LAN1/LAN2/LAN3。

<br>

![figure 2.1-1 Main Module](../_assets/2-ethernet-ip/1-network/hi6com.png)

<br>

**2. 网络设置**

<br>

选择一个 LAN 端口来连接 EtherNet/IP 通信，然后通过 TP 屏幕检查 LAN 端口的设置，如下所示，并根据需要更改设置。

<br>

![figure 2.1-2 Network configuration](../_assets/2-ethernet-ip/1-network/networkConfig.png)

<br>

{% hint style="info" %}
   - LAN1/LAN2/LAN3 每个 IP 地址的子网部分应该设置得不同。

   - 更改设置后，请重新启动机器人控制器。
{% endhint %}

<br>

**3. 连接状态检查**

<br>

可以根据 LAN 端口的 Link/Act LED 状态检查与 EtherNet/IP 扫描仪的物理连接状态。

<br>

使用 LAN 电缆连接 EtherNet/IP 适配器和扫描仪，然后检查 LED 状态。如果左侧的 LED 不亮或不闪烁，则表示电缆、适配器或扫描仪设备存在问题。请检查电缆或设备的连接状态。

<br>

![figure 2.1-3 LAN Port](../_assets/2-ethernet-ip/1-network/lanPort.png)

<br>

**4. 网络配置**

<br>

建议将 EtherNet/IP 网络和工厂网络配置为不同的网络。如下面的图所示，如果将 EtherNet/IP 网络和工厂网络配置为一个网络，它们将共享一个传输介质，增加网络负载。因此，建议如果可能的话，为 EtherNet/IP 网络使用单独配置的网络。

<br>

![figure 2.1-4 Network](../_assets/2-ethernet-ip/1-network/NG_Network.png)

<br>

![figure 2.1-5 Network](../_assets/2-ethernet-ip/1-network/Good_Network.png)

<br>
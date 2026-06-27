### 2.3.2 EtherNet/IP 适配器 (从设备) 设置

<br>

**1. 通过教学挂件设置和监控 EtherNet/IP 适配器**

<br>

**\[系统 > 2: 控制参数 > 11: 工业通信 > 3: EtherNet/IP 设置]**

<br>

![Config.PNG](../../_assets/2-ethernet-ip/3-adapter/Config.png)<br>

<br>

{% hint style="info" %}
   [协议设置]

      - OFF : 禁用 EtherNet/IP  
      - Adapter : EtherNet/IP 适配器模式  
      - Scanner : EtherNet/IP 扫描器模式  
      - Adapter + Scanner : EtherNet/IP 适配器 + 扫描器模式  
{% endhint %}

<br>

{% hint style="info" %}
   [端口设置]

      - 通用控制器 LAN1 到 LAN3 可用 (确保状态为 "OK")
{% endhint %}

<br>

{% hint style="info" %}
   [IO 大小]

      - 输入字节数: 可设置为 0-240。  
      - 输出字节数: 可设置为 0-240。
{% endhint %}   

<br>

{% hint style="info" %}
   [通信状态检查]   

      - License: 当前许可证状态  
      - Run: 指示 EtherNet/IP 功能的操作状态  
      - Communication: 指示 EtherNet/IP 连接状态  
      - Error: 指示 EtherNet/IP 错误状态    
{% endhint %}
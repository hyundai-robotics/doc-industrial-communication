### 2.3.2 EtherNet/IP适配器（从属）设置

<br>

**1. 通过教学挂件进行EtherNet/IP适配器设置和监控**

<br>

**\[系统 > 2: 控制参数 > 11: 工业通信 > 3: EtherNet/IP设置]**

<br>

![Config.PNG](../../_assets/2-ethernet-ip/3-adapter/Config.png)<br>

<br>

{% hint style="info" %}
   [协议设置]

      - OFF : 禁用EtherNet/IP   
      - Adapter : EtherNet/IP适配器模式   
      - Scanner : EtherNet/IP扫描模式   
      - Adapter + Scanner : EtherNet/IP适配器 + 扫描仪模式   
{% endhint %}

<br>

{% hint style="info" %}
   [端口设置]

      - 通用控制器LAN1到LAN3可用（确保状态为“OK”）
{% endhint %}

<br>

{% hint style="info" %}
   [IO大小]

      - 输入字节数：可以设置为0-240。   
      - 输出字节数：可以设置为0-240。
{% endhint %}   

<br>

{% hint style="info" %}
   [通信状态检查]   

      - License: 当前许可证状态   
      - Run: 表示EtherNet/IP功能的操作状态   
      - Communication: 表示EtherNet/IP连接状态   
      - Error: 表示EtherNet/IP错误状态    
{% endhint %}
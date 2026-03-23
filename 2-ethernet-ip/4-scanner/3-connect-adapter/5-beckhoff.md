#### 2.4.3.5 连接外部适配器设备 - Beckhoff Remote IO

<br>

{% hint style="info" %}
   - 您可以使用 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置文件信息。

   - "[**下载 EDS 文件工具 (EZ-EDS)**](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 请参阅 Beckhoff 手册以获取设备的 IP 配置。
{% endhint %}

<br>

**1. 准备适配器设备的手册和 EDS 文件。**

![[figure 2.4.3.5-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_1.png>) 

<br>

**2. 访问设备的网页以配置 IP 地址。**

<br>

{% hint style="info" %}
   - 在此示例中，初始 IP 地址设置为 192.168.1.2 (DIP 开关 No. 2 是 ON)
{% endhint %}

<br>

![[figure 2.4.3.5-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_2.png>) 

<br>

![[figure 2.4.3.5-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_3.png>) 

<br>

{% hint style="info" %}
   - 在此示例中，IP 地址更改为 192.168.10.95。

   - 输入 IP 地址后，单击检查按钮以保存。
{% endhint %}

<br>

![[figure 2.4.3.5-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_4.png>) 

<br>

{% hint style="info" %}
   - 按照以下方式设置 DIP 开关并重新启动设备：   
      - 1 ~ 8  : ON   
      - 9 ~ 10 : OFF   
{% endhint %}

<br>

![[figure 2.4.3.5-5 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_5.png>) 

<br>

![[figure 2.4.3.5-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_6.png>) 

<br>

**3. 访问设备的网页以验证 EtherNet/IP 配置信息。**

<br>

{% hint style="info" %}
   - 使用新配置的 IP 地址重新访问网页，并验证 IP 地址和 EtherNet/IP 配置详细信息。
{% endhint %}

<br>

![[figure 2.4.3.5-7 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_7.png>) 

<br>

![[figure 2.4.3.5-8 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_8.png>) 

<br>

{% hint style="info" %}
   - 输入 (T > O)   
      - 实例 ID: 129   
      - 字节大小: 6      

   - 输出 (O > T)   
      - 实例 ID: 130   
      - 字节大小: 6   
{% endhint %}

<br>

**4. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.5-9 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/5-beckhoff/img_9.png>)

<br>

{% hint style="info" %}
   - 请参阅目标设备的手册以正确输入设置。   
      - 输入 (T > O) : 从属设备 > 主设备    
      - 输出 (O > T) : 主设备 > 从属设备   

   [适配器配置]   
   - Beckhoff EK-9500   
      - EK-1008 : 1byte (T > O)   
      - EK-2008 : 1byte (O > T)   

   [IO 组件信息]   
   [T > O]   
      - 大小: 6bytes   
      - 实例: 129   
      - 运行/空闲头: 不   

   [O > T]    
      - 大小: 6bytes   
      - 实例: 130   
      - 运行/空闲头: 32Bit   
{% endhint %}

<br>
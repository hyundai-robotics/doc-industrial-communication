#### 2.4.3.6 连接外部适配器设备 - Rockwell 自动化 (AB) 远程 IO

<br>

{% hint style="info" %}
   - 您可以通过 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置文件信息。

   - "[下载 EDS 文件工具 (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 请参考 Rockwell 自动化手册以获取设备的 IP 配置。
{% endhint %}

<br>

**1. 准备适配器设备的手册和 EDS 文件。**

<br>

![[figure 2.4.3.6-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_1.png>) 

<br>

![[figure 2.4.3.6-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_2.png>) 

<br>

**2. 使用 EZ-EDS 程序打开 EDS 文件并验证设备信息。**

<br>

![[figure 2.4.3.6-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_3.png>) 

<br>

![[figure 2.4.3.6-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_4.png>) 

<br>

{% hint style="info" %}
   - 在连接管理器中检查连接类型   
      - 示例：独占所有者

   - 检查实时传输格式中是否存在头   
      - 输入 (T > O) : 无头   
      - 输出 (O > T) : 32位运行/空闲头   

   - 单击 "创建 / 解码路径" 以验证实例 ID   
      - 输入 (T > O) : 101   
      - 输出 (O > T) : 100   
      - 配置 : 102   
{% endhint %}

<br>

**3. 检查设备手册中的 I/O 大小。**

<br>

{% hint style="info" %}
   - 验证要连接的设备的 I/O 配置。
{% endhint %}

<br>

![[figure 2.4.3.6-5 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_5.png>) 

<br>

{% hint style="info" %}
   - 验证要连接的设备的 I/O 配置。
{% endhint %}

<br>

![[figure 2.4.3.6-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_6.png>) 

<br>

![[figure 2.4.3.6-7 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_7.png>) 

<br>

**4. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.6-8 EtherNet/IP 设置]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_8.png>)

<br>

{% hint style="info" %}
   - 请参考目标设备的手册以正确输入设置。   
      - 输入 (T > O) : 从属 > 主   
      - 输出 (O > T) : 主 > 从   

   [适配器配置]   
   - Point I/O 1734-AENTR    
      - 状态 : 8字节 (T > O)    
      - 1734-IB8 : 1字节 (T > O)   
      - 1734-OB8E : 1字节 (O > T) + 1字节 (T > O, 状态)   

   [IO 组装信息]   
   [T > O]   
      - 大小: 10字节   
      - 实例: 101   
      - 运行/空闲头: 无   

   [O > T]    
      - 大小: 1字节   
      - 实例: 100   
      - 运行/空闲头: 32位   
{% endhint %}

<br>

![[figure 2.4.3.6-9 EtherNet/IP 设置]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/6-rockwell/img_9.png>)

<br>

{% hint style="info" %}
   - 请参考目标设备的手册以正确输入额外设置。   
      - 输入 (T > O) : 从属 > 主   
      - 输出 (O > T) : 主 > 从   

   [附加设置]   
      - 配置段 : 开   
      - 实例: 102   
      - 大小: 10字节    

   [配置段信息]    
      - (4字节) 1 : 头    
      - (2字节) 3 : 连接插槽 + 1   
      - (1字节) 0 : T > O 对齐 (字节)      
      - (1字节) 1 : T > O 每插槽数据大小      
      - (1字节) 0 : O > T 对齐 (字节)      
      - (1字节) 1 : O > T 每插槽数据大小      
{% endhint %}

<br>
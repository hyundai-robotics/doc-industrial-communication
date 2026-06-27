#### 2.4.3.2 连接外部适配器设备 - Wago 远程 IO

<br>

{% hint style="info" %}
   - 您可以使用 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置文件信息。

   - "[下载 EDS 文件工具 (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 请参考 Wago 手册获取设备的 IP 配置。
{% endhint %}

<br>

**1. 准备适配器设备的手册和 EDS 文件。**

![[figure 2.4.3.2-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_1.png>) 

<br>

**2. 检查设备手册中提供的实例 ID**

<br>

![[figure 2.4.3.2-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_2.png>) 

<br>

{% hint style="info" %}
   - 输入 (T > O)   
      - 104: 状态 + 模拟 + 数字   
      - 105: 状态 + 数字   
      - 106: 状态 + 模拟   
      - 107: 模拟 + 数字   
      - 108: 数字   
      - 109: 模拟   

   - 输出 (O > T)   
      - 101: 模拟 + 数字   
      - 102: 数字   
      - 103: 模拟   
{% endhint %}

<br>

**3. 使用 EZ-EDS 程序打开 EDS 文件并验证设备信息。**

<br>

![figure 2.4.3.2-3 EDS Info](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_3.png>) 

<br>

{% hint style="info" %}
   - 在连接管理器中检查连接类型   
      - 示例：排他性所有者

   - 检查实时传输格式中是否存在头部   
      - 输入 (T > O) : 无头部   
      - 输出 (O > T) : 32位运行/空闲头部   
{% endhint %}

<br>

**4. 检查设备手册中的 I/O 大小。**

<br>

{% hint style="info" %}
   - 验证要连接的设备的 I/O 配置。 
{% endhint %}

<br>

![[figure 2.4.3.2-4 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_4.png>) 

<br>

{% hint style="info" %}
   - 请参考每个插槽配置的手册，以确定总 I/O 大小。
{% endhint %}

<br>

![[figure 2.4.3.2-5 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_5.png>) 

<br>

![[figure 2.4.3.2-6 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_6.png>) 

<br>

**5. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.2-7 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/2-wago/img_7.png>)

<br>

{% hint style="info" %}
   - 请参考目标设备的手册以正确输入设置。   
      - 输入 (T > O) : 从设备 > 主设备   
      - 输出 (O > T) : 主设备 > 从设备   

   [适配器配置]   
   - Wago 750-366   
      - 状态 1字节 (T > O) (选择实例 ID 104、105、106 时)   
      - 753-436 : 1字节 (T > O)   
      - 753-536 : 1字节 (O > T)   

   [IO 组装信息]   
   [T > O]   
      - 大小: 2字节   
      - 实例: 105   
      - 运行/空闲头部: 无   

   [O > T]    
      - 大小: 1字节   
      - 实例: 101   
      - 运行/空闲头部: 32位   
{% endhint %}

<br>
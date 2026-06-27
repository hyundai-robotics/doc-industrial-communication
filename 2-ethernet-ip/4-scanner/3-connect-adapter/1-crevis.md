#### 2.4.3.1 连接外部适配器设备 - Crevis 远程 I/O

<br>

{% hint style="info" %}
   - 您可以使用 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置文件信息。

   - "[下载 EDS 文件工具 (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 有关示例中使用的远程 I/O 的 IP 设置，请参考下面的手册链接。

   - "[1.3.10.2 远程 I/O IP 设置](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/10-EtherNet-IP-Remote-IO/2-Settings-Remote-IO-IP.md)"
{% endhint %}

<br>

**1. 为适配器设备准备手册和 EDS 文件。**

![[figure 2.4.3.1-1 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_1.png>) 

<br>

![[figure 2.4.3.1-2 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_2.png>) 

<br>

![[figure 2.4.3.1-3 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_3.png>) 

<br>

**2. 使用 EZ-EDS 程序打开 EDS 文件并验证设备信息。**

<br>

![[figure 2.4.3.1-4 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_4.png>) 

<br>

{% hint style="info" %}
   - 在连接管理器中检查连接类型  
      - 示例：独占所有者

   - 检查实时传输格式中是否存在头部   
      - 输入 (T > O) : 无头部   
      - 输出 (O > T) : 32 位运行/空闲头部   

   - 点击 "创建 / 解码路径" 以验证实例 ID   
{% endhint %}

<br>

![[figure 2.4.3.1-5 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_5.png>) 

<br>

{% hint style="info" %}
      - 输入 (T > O) : 1   
      - 输出 (O > T) : 2   
{% endhint %}

<br>

**3. 检查设备手册中的 I/O 大小。**

<br>

{% hint style="info" %}
   - 验证要连接的设备的 I/O 配置。 
{% endhint %}

<br>

![[figure 2.4.3.1-6 Remote IO]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_6.png>) 

<br>

{% hint style="info" %}
   - 请参考手册中每个插槽配置以确定总 I/O 大小。
{% endhint %}

<br>

![[figure 2.4.3.1-7 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_7.png>) 

<br>

![[figure 2.4.3.1-8 IO Size]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_8.png>) 

<br>

**4. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.1-8 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/1-crevis/img_9.png>)

<br>

{% hint style="info" %}
   - 请参考目标设备的手册以正确输入设置。   
      - 输入 (T > O) : 从属 > 主设备   
      - 输出 (O > T) : 主设备 > 从属   

   [适配器配置]   
   - Crevis M9289   
      - M7002 : 无   
      - M2768 : 1字节 (O > T)   
      - M2768 : 1字节 (O > T)   
      - M12DF : 2字节 (T > O)   
      - M12DF : 2字节 (T > O)   
      - M2768 : 1字节 (O > T)   
      - M2768 : 1字节 (O > T)   

   [IO 组件信息]   
   [T > O]   
      - 大小：4字节   
      - 实例：1   
      - 运行/空闲头部：无   

   [O > T]    
      - 大小：4字节   
      - 实例：2   
      - 运行/空闲头部：32位   
{% endhint %}

<br>
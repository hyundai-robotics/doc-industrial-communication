#### 2.4.3.3 连接外部适配器设备 - Hilscher CIFX PCI EtherNet/IP 适配器

<br>

{% hint style="info" %}
   - 您可以使用 EZ-EDS 程序轻松验证 EtherNet/IP 适配器设备的配置信息。

   - "[下载 EDS 文件工具 (EZ-EDS)](https://www.odva.org/subscriptions-services/additional-tools/ez-eds-download/)"
{% endhint %}

<br>

{% hint style="info" %}
   - 请参阅 Hilscher 手册以获取设备的 IP 配置。
{% endhint %}

<br>

**1. 准备适配器设备的手册和 EDS 文件。**

![[figure 2.4.3.3-1 CIFX PCI]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_1.png>) 

<br>

**2. 使用 EZ-EDS 程序打开 EDS 文件并验证设备信息。**

<br>

![[figure 2.4.3.3-2 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_2.png>) 

<br>

{% hint style="info" %}
   - 检查连接管理器中的连接类型   
      - 示例：独占所有者

   - 检查实时传输格式中头部的存在   
      - 输入 (T > O) : 32 位运行/空闲头部   
      - 输出 (O > T) : 32 位运行/空闲头部   
{% endhint %}

<br>

![[figure 2.4.3.3-3 EDS Info]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_3.png>) 

<br>

{% hint style="info" %}
   - 检查 Param 中的实例 ID   
      - 输入 (T > O) : 101   
      - 输出 (O > T) : 100   
{% endhint %}

<br>

**3. 在设备手册中检查 I/O 大小。**

<br>

{% hint style="info" %}
   - 检查要连接的当前设备的 I/O 大小（参阅相应的 PCI 设备设置）   
{% endhint %}

<br>

**4. 根据适配器设备信息输入通信设置。**

<br>

![[figure 2.4.3.3-4 EtherNet/IP Settings]](<../../../_assets/2-ethernet-ip/4-scanner/3-connect-adapter/3-pci/img_4.png>)

<br>

{% hint style="info" %}
   - 请参阅目标设备的手册以正确输入设置。   
      - 输入 (T > O) : 从属 > 主设备   
      - 输出 (O > T) : 主设备 > 从属   

   [IO 组件信息]   
   [T > O]   
      - 大小：240 字节（在 PCI 设备中配置的值）   
      - 实例：101   
      - 运行/空闲头部：32位   

   [O > T]    
      - 大小：240 字节（在 PCI 设备中配置的值）   
      - 实例：100   
      - 运行/空闲头部：32位   
{% endhint %}

<br>
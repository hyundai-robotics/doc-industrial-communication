### 2.4.2 EtherNet/IP 扫描仪 (主控制器) 设置

<br>

完成 "[2.1 网络设置](../../2-ethernet-ip/1-network.md)" 和 "[2.2 许可证设置](../../2-ethernet-ip/2-license.md)" 中的程序后，请继续执行以下步骤。

<br>

**1. 触摸菜单以进入设置屏幕。**

<br>

**\[系统 > 2: 控制参数 > 11: 工业通信 > 3: EtherNet/IP 设置]**

<br>

![[figure 2.4.2-1 扫描仪设置]](<../../_assets/2-ethernet-ip/4-scanner/img_1.png>) 

<br>

![[figure 2.4.2-2 扫描仪设置]](<../../_assets/2-ethernet-ip/4-scanner/img_2.png>) 

<br>

{% hint style="info" %}
   [协议设置]

      - OFF : 关闭 EtherNet/IP   
      - Adapter : EtherNet/IP 适配器模式   
      - Scanner : EtherNet/IP 扫描仪模式   
      - Adapter + Scanner : EtherNet/IP 适配器 + 扫描仪模式   
{% endhint %}

<br>

{% hint style="info" %}
   [端口设置]

      - 通用控制器 LAN1 到 LAN3 可用（确保状态为 "OK"）
{% endhint %}

<br>

**2. 选择 "扫描仪" 模式并单击 "添加设备" 按钮以继续到下一个屏幕。**

<br>

![[figure 2.4.2-3 扫描仪添加设备]](<../../_assets/2-ethernet-ip/4-scanner/img_3.png>) 

<br>

**3. 输入与目标设备匹配的设置并保存。**

<br>

{% hint style="info" %}
   [设备设置]

      - 设备编号 : 设备连接顺序（I/O 数据分配的顺序）   
      - IP 地址 : 设备的 IP 地址   
      - 设备名称 : 设备的名称（仅用于识别，不影响通信）   
      - RPI (毫秒) : 请求的数据包间隔（I/O 数据更新周期）   
      - 连接类型   
            - 独占所有者 (I/O) : 在扫描仪和适配器之间建立双向 I/O 连接   
            - 仅输入 : 仅连接到适配器的输入信号   
            - 仅监听 : 仅在适配器已连接到另一个扫描仪时连接到输入信号   

      - 输入 (T > O) : 从设备 > 主设备 连接   
      - 输出 (O > T) : 主设备 > 从设备 连接   

      - 运行/空闲标头 : 选择是否包含 I/O 数据标头   
      - 实例编号 : I/O 数据交换的输入/输出组的实例编号   
      - I/O 大小 : I/O 数据的大小（以字节为单位）   
{% endhint %}

<br>

{% hint style="info" %}
   - 有关连接示例，请参阅以下手册。    
   - "[2.4.3.1 连接外部适配器设备 - Crevis 远程 I/O](3-connect-adapter/1-crevis.md)"

   - "[2.4.3.2 连接外部适配器设备 - Wago 远程 I/O](3-connect-adapter/2-wago.md)"

   - "[2.4.3.3 连接外部适配器设备 - Hilscher CIFX PCI EtherNet/IP 适配器](3-connect-adapter/3-pci.md)"

   - "[2.4.3.4 连接外部适配器设备 - Baumer OM-70](3-connect-adapter/4-baumer.md)"  
{% endhint %}

<br>

![[figure 2.4.2-4 扫描仪添加设备]](<../../_assets/2-ethernet-ip/4-scanner/img_4.png>) 

<br>

**4. 单击 "确认" 按钮以传输通信设置。**

<br>

![[figure 2.4.2-5 扫描仪设置]](<../../_assets/2-ethernet-ip/4-scanner/img_5.png>) 

<br>

**5. 检查状态以验证通信是否成功建立。**

<br>

![[figure 2.4.2-6 通信状态]](<../../_assets/2-ethernet-ip/4-scanner/img_6.png>) 

<br>

{% hint style="info" %}
   [通信状态检查]   

      - 许可证: 当前许可证状态   
      - 运行: 表示 EtherNet/IP 功能的操作状态   
      - 通信: 表示 EtherNet/IP 连接状态   
      - 错误: 表示 EtherNet/IP 错误状态    
{% endhint %}

<br>

{% hint style="info" %}
   [设备编号颜色]   

      - 绿色: 通信连接正常   
      - 红色: 通信连接不良（失败）   
{% endhint %}

<br>

![[figure 2.4.2-7 通信状态]](<../../_assets/2-ethernet-ip/4-scanner/img_7.png>) 

<br>

**6. 完成通信设置后，分配 I/O 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 I/O 块来使用输入/输出信号。请参阅 ("[5. 工业通信 I/O 读取和写入](../../5-io-block-allocation.md)")**
{% endhint %}
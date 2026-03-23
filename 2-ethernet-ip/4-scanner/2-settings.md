### 2.4.2 EtherNet/IP 扫描仪 (主设备) 设置

<br>

在完成 "[**2.1 网络设置**](../../2-ethernet-ip/1-network.md)" 和 "[**2.2 许可设置**](../../2-ethernet-ip/2-license.md)" 中的程序后，请继续进行以下步骤。

<br>

**1. 触摸菜单以进入设置屏幕。**

<br>

**\[系统 > 2: 控制参数 > 11: 工业通信 > 3: EtherNet/IP 设置]**

<br>

![[figure 2.4.2-1 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_1.png>) 

<br>

![[figure 2.4.2-2 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_2.png>) 

<br>

{% hint style="info" %}
   [协议设置]

      - 关闭 : 禁用 EtherNet/IP   
      - 适配器 : EtherNet/IP 适配器模式   
      - 扫描仪 : EtherNet/IP 扫描仪模式   
      - 适配器 + 扫描仪 : EtherNet/IP 适配器 + 扫描仪模式（使用同一局域网端口）
{% endhint %}

{% hint style="info" %}
   [端口设置]

      - 通用控制器 LAN1 到 LAN3 可用（确保状态为“OK”）
{% endhint %}

<br>

**2. 选择“扫描仪”模式并点击“添加设备”按钮以继续到下一个屏幕。**

<br>

![[figure 2.4.2-3 Scanner Add Device]](<../../_assets/2-ethernet-ip/4-scanner/img_3.png>) 

<br>

**3. 输入设置以匹配目标设备并保存。**

<br>

{% hint style="info" %}
   [设备设置]

      - 设备编号 : 设备连接顺序（I/O 数据分配顺序）   
      - IP 地址 : 设备的 IP 地址   
      - 设备名称 : 设备名称（仅用于识别；不影响通信）   
      - RPI (毫秒) : 请求的数据包间隔 (I/O 数据更新周期)   
      - 连接类型   
            - 独占所有者 (I/O) : 在扫描仪和适配器之间建立双向 I/O 连接   
            - 仅输入 : 仅连接到适配器的输入信号   
            - 仅监听 : 在适配器已经连接到另一台扫描仪时，仅连接到输入信号   

      - 输入 (T > O) : 从设备 > 主设备连接   
      - 输出 (O > T) : 主设备 > 从设备连接   

      - 运行/空闲头 : 选择是否包括 I/O 数据头   
      - 实例编号 : I/O 数据交换的输入/输出组实例编号   
      - I/O 大小 : I/O 数据大小（以字节为单位）   
{% endhint %}

<br>

{% hint style="info" %}
   - 有关连接示例，请参阅以下手册。    
   - "[**2.3.3.1 连接外部适配器设备 - Crevis 远程 IO**](3-connect-adapter/1-crevis.md)"

   - "[**2.3.3.2 连接外部适配器设备 - Wago 远程 IO**](3-connect-adapter/2-wago.md)"

   - "[**2.3.3.3 连接外部适配器设备 - Hilscher CIFX PCI EtherNet/IP 适配器**](3-connect-adapter/3-pci.md)"

   - "[**2.3.3.4 连接外部适配器设备 - Baumer OM-70**](3-connect-adapter/4-baumer.md)"  
{% endhint %}

<br>

![[figure 2.4.2-4 Scanner Add Device]](<../../_assets/2-ethernet-ip/4-scanner/img_4.png>) 

<br>

**4. 点击“确定”按钮以传输通信设置。**

<br>

![[figure 2.4.2-5 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_5.png>) 

<br>

**5. 检查状态以验证通信是否成功建立。**

<br>

![[figure 2.4.2-6 Communication Status]](<../../_assets/2-ethernet-ip/4-scanner/img_6.png>) 

<br>

{% hint style="info" %}
   [通信状态检查]   
      - 许可: 当前许可状态   
      - 运行: 指示 EtherNet/IP 功能的操作状态   
      - 通信: 指示 EtherNet/IP 连接状态   
      - 错误: 指示 EtherNet/IP 错误状态   

   - 设备编号颜色   
      - 绿色: 通信连接 OK   
      - 红色: 通信连接 NG (失败)   
{% endhint %}

<br>

![[figure 2.4.2-7 Communication Status]](<../../_assets/2-ethernet-ip/4-scanner/img_7.png>) 

<br>

**6. 完成通信设置后，分配 I/O 块。**

{% hint style="info" %}
   **完成通信设置后，可以通过分配 I/O 块使用输入/输出信号。请参阅 ("[**4. 工业通信 IO 块分配**](../../5-io-block-allocation.md)")**
{% endhint %}
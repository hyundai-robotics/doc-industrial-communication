## 3.1 EtherCAT 主控 IO 设置

<br>

**1. 点击菜单以进入设置屏幕。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 4: EtherCAT 主控设置]**

<br>

![[Figure 3.1-1 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_1.png>) 

<br>

{% hint style="info" %}
   - 在 EtherCAT 主控设置屏幕上检查所选控制器 LAN 端口号。 
{% endhint %}

**2. 连接控制器 LAN 端口和远程 IO 电缆等进行通信，并检查状态。**

<br>

![[Figure 3.1-2 Hardware Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_2.png>) 
![[Figure 3.1-3 Hardware Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_3.png>) 

<br>

{% hint style="info" %}
   - 请使用 LAN 电缆连接控制器和远程 IO。

   - 将远程 IO 的所有 DIP 开关设置为关闭。

   - 连接远程 IO 电源和现场电源 (24 V DC)。
{% endhint %}

<br>

**3. 在设置菜单中选择 "ON" 以使用 EtherCAT 主控。**

<br>

![[Figure 3.1-4 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_4.png>)

<br>

{% hint style="info" %}
   - 根据您的使用环境设置通信周期。

   - 支持 1 ms、2 ms 和 5 ms 的通信周期。
{% endhint %}

<br>

**4. 从设置菜单中的从站列表中选择与连接的远程 IO 模块相同的配置。**

<br>

![[Figure 3.1-5 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_5.png>)

<br>

{% hint style="info" %}
   - 检查输入和输出字节数。
{% endhint %}

<br>

{% hint style="info" %}
   - 输入模块  
   - M12DF: 数字 16 点  
   - M3534: 模拟 4 点  
{% endhint %}

{% hint style="info" %}
   - 输出模块  
   - M225F: 数字 16 点  
   - M226F: 数字 16 点  
   - M2768: 数字 8 点   
   - M4534: 模拟 4 点  
{% endhint %}

{% hint style="info" %}
   - 特殊模块  
   - M5112 : 输送系统 I/F 
{% endhint %}

<br>

![[Figure 3.1-6 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_6.png>) 

<br>

**5. 完成设置后重启控制器。**

![[Figure 3.1-7 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_7.png>) 

<br>

![[Figure 3.1-8 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_8.png>) 

<br>

{% hint style="info" %}
   - 设置完成后请重启控制器。
{% endhint %}

<br>

**6. 确认设置值已应用后，检查通信状态。**

![[Figure 3.1-9 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_9.png>) 

<br>

{% hint style="info" %}
   - 请检查通信连接状态并检查是否存在错误。
{% endhint %}

<br>

![[Figure 3.1-10 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_10.png>)

<br>

{% hint style="info" %}
   - 请检查远程 IO 模块上的 LED，以确认通信是否正确建立。
{% endhint %}

<br>

{% hint style="info" %}
   **如果通信过程中发生错误，请参阅 ("[3.2 EtherCAT 主控 IO 错误处理](../3-ethercat-master-io/2-Error-EtherCAT-Master.md)")。**
{% endhint %}

<br>

**7. 完成通信设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块使用输入/输出信号。请参阅 ("[5. 工业通信 IO 读写](../5-io-block-allocation.md)")。**
{% endhint %}
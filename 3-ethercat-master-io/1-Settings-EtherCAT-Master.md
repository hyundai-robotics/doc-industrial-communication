## 3.1 EtherCAT Master IO 设置

<br>

**1. 点击菜单进入设置屏幕。**
**\[System > 2: Control Parameters > 11: Industrial Communication > 4: EtherCAT Master Settings]**

<br>

![[Figure 3.1-1 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_1.png>) 

<br>

{% hint style="info" %}
   - 请检查在 EtherCAT 主设置屏幕上选择的控制器 LAN 端口号。 
{% endhint %}

**2. 连接控制器 LAN 端口与 Remote IO 电缆等进行通信并检查状态。**

<br>

![[Figure 3.1-2 Hardware Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_2.png>) 
![[Figure 3.1-3 Hardware Connection]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_3.png>) 

<br>

{% hint style="info" %}
   - 请使用 LAN 电缆连接控制器与 Remote IO。

   - 将 Remote IO 的所有 DIP 开关设置为 OFF。

   - 同时连接 Remote IO 电源和现场电源（24 V DC）。
{% endhint %}

<br>

**3. 在设置菜单中选择 EtherCAT 主使用的 "ON"。**

<br>

![[Figure 3.1-4 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_4.png>)

<br>

{% hint style="info" %}
   - 根据您的使用环境设置通信周期。

   - 支持 1 ms、2 ms 和 5 ms 的通信周期。
{% endhint %}

<br>

**4. 在设置菜单中从从属列表中选择与连接的 Remote IO 模块相同的配置。**

<br>

![[Figure 3.1-5 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_5.png>)

<br>

{% hint style="info" %}
   - 检查输入和输出字节计数。
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
   - M5112 : 输送机 I/F 
{% endhint %}

<br>

![[Figure 3.1-6 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_6.png>) 

<br>

**5. 完成设置后重新启动控制器。**

![[Figure 3.1-7 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_7.png>) 

<br>

![[Figure 3.1-8 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_8.png>) 

<br>

{% hint style="info" %}
   - 请在完成设置后重新启动控制器。
{% endhint %}

<br>

**6. 确认设置值已反映后，检查通信状态。**

![[Figure 3.1-9 EtherCAT Master Settings]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_9.png>) 

<br>

{% hint style="info" %}
   - 请检查通信连接状态并检查是否有错误。
{% endhint %}

<br>

![[Figure 3.1-10 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_10.png>)

<br>

{% hint style="info" %}
   - 请检查是否使用 Remote IO 模块上的 LED 正确建立通信。
{% endhint %}

<br>

{% hint style="info" %}
   **如果通信过程中发生错误，请参阅 ("[3.2 EtherCAT Master IO 错误处理](../3-ethercat-master-io/2-Error-EtherCAT-Master.md)").**
{% endhint %}

<br>

**7. 完成通信设置后分配 IO 块。**

{% hint style="info" %}
   **完成通信设置后，您可以通过分配 IO 块使用输入/输出信号。请参阅 ("[5. Industrial Communication IO 读写](../5-io-block-allocation.md)").**
{% endhint %}
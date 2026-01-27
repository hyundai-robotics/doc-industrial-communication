## 3.1 EtherCAT Master IO设置

<br>

**1. 触摸菜单来进入设置界面。**
**\[系统 > 2: 控制参数 > 11: 工业通信 > 4: EtherCAT Master设置]**

<br>

![[图 3.1-1 EtherCAT Master 设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_1.png>) 

<br>

{% hint style="info" %}
\.      在 EtherCAT Master 设置界面中，确认所选控制器的 LAN Port 编号。 
{% endhint %}

**2. 为了实现通信，连接控制器LAN端口和Remote IO的电缆等并确认状态。**

<br>

![[图 3.1-2 硬件连接]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_2.png>) 
![[图 3.1-3 硬件连接]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_3.png>) 

<br>

{% hint style="info" %}
\.      请用LAN电缆连接控制器和Remote IO。

\.      请将Remote IO的DIP Switch全部设置为OFF。

\.      请全部连接Remote IO电源和Field Power。（24V DC）
{% endhint %}

<br>

**3. 在设置菜单中，请将EtherCAT Master选择为“ON”（启用）。**

<br>

![[图 3.1-4 EtherCAT Master设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_4.png>)

<br>

{% hint style="info" %}
\.      根据使用环境设置通信周期。

\.      通信周期支持1ms、2ms、5ms。
{% endhint %}

<br>

**4. 在设置菜单的从站列表中，选择与所连接的 Remote IO 模块相同的配置。**

<br>

![[图 3.1-5 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_5.png>)

<br>

{% hint style="info" %}
\.      确认 Input、Output 字节数。
{% endhint %}

<br>

{% hint style="info" %}
\.      Input Module  
\.      M12DF：Digital 16点  
\.      M3534：Analog 4点  
{% endhint %}

{% hint style="info" %}
\.      Output Module  
\.      M225F：Digital 16点  
\.      M226F：Digital 16点  
\.      M2768：Digital 8点   
\.      M4534：Analog 4点  
{% endhint %}

{% hint style="info" %}
\.      Special Module  
\.      M5112 : Conveyer I/F 
{% endhint %}

<br>

![[图 3.1-6 EtherCAT Master设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_6.png>) 

<br>

**5. 设置完成后重启控制器。**

![[图 3.1-7 EtherCAT Master设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_7.png>) 

<br>

![[图 3.1-8 EtherCAT Master设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_8.png>) 

<br>

{% hint style="info" %}
\.      设置完成后，请重启控制器。
{% endhint %}

<br>

**6. 确认设定值是否已反映，并确认通信状态。**

![[图 3.1-9 EtherCAT Master设置]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_9.png>) 

<br>

{% hint style="info" %}
\.      请确认通信连接状态和是否出现错误。
{% endhint %}

<br>

![[图 3.1-10 Crevis M9386]](<../_assets/3-ethercat-master-io/1-Settings-Master/image_10.png>)

<br>

{% hint style="info" %}
\.      请通过Remote IO Module上的LED，确认通信是否正常开通。
{% endhint %}

<br>

{% hint style="info" %}
\.      **当通信状态发生ERROR时，请确认（“[**3.2 EtherCAT Master IO错误处理**](../3-ethercat-master-io/2-Error-EtherCAT-Master.md)”）。**
{% endhint %}

<br>

**7. 通信设置完成后分配IO Block。**

{% hint style="info" %}
\.      **通信设置完成后，可以通过分配IO Block来使用输入输出信号。请确认（“[**4. 工业通信IO Block分配**](../4-io-block-allocation.md)”）。**
{% endhint %}


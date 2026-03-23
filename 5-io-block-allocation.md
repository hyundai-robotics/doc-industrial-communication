# 5. 工业通信 IO 读取和写入

这是在完成工业通信设置后，为与控制器进行通信分配 IO 块的方法。

要使用工业通信 IO，必须将 IO 块分配到 fb0 - fb9 区域。

<br>

{% hint style="info" %}
   - 有关 fb 块的 IO 读取/写入方法，请参考以下手册。

      **\[控制器操作手册: 一般输入]**   
      **\[控制器操作手册: 一般输出]**   
{% endhint %}

<br>

**1. 选择 IO 块分配菜单。**
   触摸 **\[系统 > 2: 控制参数 > 2: 输入/输出信号设置 > 6: FB 块分配]** 菜单。

<br>

**2. 为所需 fb 区域指定工业通信类型。**
   指定后，触摸 **\[确定]** 按钮。

![[Figure 5-1]](<_assets/4-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[注意]**: 使用嵌入式 PLC 时，请检查 IO 属性和 DI/DO - X/Y。
{% endhint %}

{% hint style="warning" %}
**\[注意]**: 对于 EtherNet/IP 适配器，最大块大小为 120 字节，最多可以选择 2 个块。任何超过 2 的选择将被忽略。
{% endhint %}
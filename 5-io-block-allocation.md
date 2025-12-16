# 5. 工业通信IO读取及写入

这是工业通信设置完成后，与控制器通信所需的IO Block分配方法。

要使用工业通信IO，就必须分配到fb0 \~ fb9区域。

<br>

{% hint style="info" %}
\.      fb块的IO读取/写入方法，请参考以下说明书。

\.   **\[控制器操作说明书：通用输入]**   
\.   **\[控制器操作说明书：通用输出]**   
{% endhint %}

<br>

##### 1. 选择IO块分配菜单
   请触摸 **\[系统 > 2: 控制参数 > 2: 输入输出信号设置 > 6: FB 块分配]** 菜单。

<br>

##### 2. 在所需的fb区域指定工业通信类型
   指定后，请触摸 **\[OK]** 按钮。

![[图 5-1]](<_assets/4-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[注意]**：与内置PLC一起使用时，请确认IO属性、DI/DO - X/Y。
{% endhint %}

{% hint style="warning" %}
**\[注意]**: EtherNet/IP适配器的最大块大小为120 Bytes，最多可选择2个。超过2个的选择将被忽略。 
{% endhint %}

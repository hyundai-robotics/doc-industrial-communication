# 4. Read/Write IO Block of the Industrial Communication

This section shows how to allocate IO blocks for communication with the controller after completing industrial communication settings.

Those blocks should be allocated within the range from fb0 to fb9 to use industrial communication IO.

<br>

{% hint style="info" %}
\.      Please refer to the manual below for how to Read/Write IO of fb block.  

\.   **\[Controller Operation Manual : Public Input]**   
\.   **\[Controller Operation Manual : Public Output]**   
{% endhint %}

<br>

##### 1. Select the menu for allocating the IO blocks.
   Touch the menu **\[System > 2: Control Parameter > 2: Input/Output Signal Setting > 6: FB Block Allocation.]** 

<br>

##### 2. Designate the industrial communication type in the desired fb area.
   After designating it, touch the **\[OK]** button.

![[Figure 4-1]](<_assets/4-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[Caution]**: When used together with an embedded PLC, check the IO attributes and DI/DO - X/Y. 
{% endhint %}

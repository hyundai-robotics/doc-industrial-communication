# 5. Setting the Allocation of the Industrial Communication Digital IO (DIO) Block

This section shows how to allocate DIO blocks for communication with the controller after completing industrial communication settings.

Those blocks should be allocated within the range from fb0 to fb9 to use industrial communication IO.

<br>

##### 1. Select the menu for allocating the DIO blocks.
   Touch the menu **\[System > 2: Control Parameter > 2: Input/Output Signal Setting > 6: DIO Block Allocation.]** 

<br>

##### 2. Designate the industrial communication slot number in the desired fb area.
   After designating it, touch the **\[OK]** button.

![[Figure 5-1]](<_assets/5-DIO-Allocation/image_1.png>)


{% hint style="warning" %}
**\[Caution]**: When used together with an embedded PLC, check the IO attributes and DI/DO - X/Y. 
{% endhint %}

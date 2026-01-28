# 5. Industrial Communication IO Reading and Writing

This is the method for assigning IO blocks for the communication with the controller after completing industrial communication settings.

To use the industrial communication IO, the IO blocks should be assigned to the fb0 - fb9 area.

<br>

{% hint style="info" %}
   - For the IO reading/writing methods for fb blocks, please refer to the manual below.

      **\[Controller Operation Manual: General Input]**   
      **\[Controller Operation Manual: General Output]**   
{% endhint %}

<br>

**1. Select the IO block assignment menu.**
   Touch the **\[System > 2: Control Parameters > 2: Input/Output Signal Settings > 6: FB Block Assignment]** menu.

<br>

**2. Specify industrial communication type for the desired fb area.**
   After specifying it, touch the **\[OK]** button.

![[Figure 5-1]](<_assets/4-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[Caution]**: When using together with an embedded PLC, please check IO attributes and DI/DO - X/Y.
{% endhint %}

{% hint style="warning" %}
**\[Caution]**: For an EtherNet/IP adapter, the maximum block size is 120 bytes and up to 2 blocks can be selected. Any selection exceeding 2 will be ignored. 
{% endhint %}

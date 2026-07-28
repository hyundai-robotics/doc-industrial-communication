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

![[Figure 5-1]](<_assets/5-io-block-allocation/image_1.png>)


{% hint style="warning" %}
**\[Caution]**: When using together with an embedded PLC, please check IO attributes and DI/DO - X/Y.
{% endhint %}

{% hint style="info" %}

   **[fb Block Allocation Method]**

   - The size of one fb block is 120 bytes (960 points).   

   - Example of fb block allocation   
      - PCI slot 1: CC-Link Slave   
      - Configuration: Version2, 3 Stations, 8 Extension cyclic   
      - I/O Size   
         - RX/Y: 80 byte   
         - RWr/w: 192 byte   
         - Total: 272 byte   

      - I/O mapping is assigned in ascending order of fb block number   
      - fb2: PCI slot 1 ( ~ 120 byte)   
      - fb4: PCI slot 1 ( ~ 240 byte)   
      - fb5: PCI slot 1 ( ~ 272 byte)   

{% endhint %}
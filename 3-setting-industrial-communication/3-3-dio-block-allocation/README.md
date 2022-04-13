# 3.3 Setting the Industrial Communication DIO Block Allocation

This shows how to perform DIO block allocation for the communication with the controller after “[**3.1 Setting the Industrial Communication Firmware**](../3-1-firmware.md)” 및 “[**3.2 Setting the Addition of the Industrial Communication (Master and Slave)**](../3-2-addition-industrial-communication-master-slave/)” work is completed.

You can set the method to use the universal input and output signals of the controller. For the use, you can connect to None, PLC, or Fieldbus.

1. Touch the **\[2: Control Parameter > 2: Input/Output Signal Setting > 6: DIO Block Allocation]** menu.
2. Set the connection of the DIO block of the selected FB address and then touch the \[OK] button.
   * If Fieldbus is set, the board number will be the rotary switch number of the PCI communication card.
   * If PLC is to be used, refer to “[**3.3.1 Using Multiprog**](1-using-multiprog.md)”

![](<../../_assets/image (11).png>)

* **\[None]**: The DIO block of the selected FB address is not to be allocated. If nothing is to be selected for the initial setting value of the controller, None will be set.
* **\[PLC]**: The DIO block of the selected FB address will be allocated to the PLC for use. For the PLC operation, the MULTIPRO program will be used.
* **\[Fieldbus]**: The DIO block of the selected FB address will be allocated to the PCI communication card for use. If the DIO block is connected to the PCI communication card, the PCI board selection window will be enabled.

{% hint style="warning" %}
**\[Caution]**: The same communication card cannot be used both for PLC and Fieldbus at the same time. Data connection should be performed for one of the two.
{% endhint %}

#### 1.3.3.4 EtherNet/IP Adapter Settings

Please follow the "[**1.3.1 CIFX PCI Slot Settings**](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" procedure and then proceed with the method below.

<br>

{% hint style="info" %}
\.      **[EtherNet/IP Adapter EDS File Download]**

\.      Please refer to "[**5. Slave Device Description File**](../../../5-slave-config-file.md)".
{% endhint %}

<br>

**1. Using the TP, select an EtherNet/IP slave in the industrial communication firmware settings and reboot the robot controller.**

![[Figure 1.3.3.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_1.png>) 

<br>

**2. Check the current communication protocol readiness status in industrial communication monitoring menu.**

![[Figure 1.3.3.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_2.png>) 

<br>

{% hint style="warning" %}
**\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

**3. Touch the menu to enter the slave settings screen.**
**\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > EtherNet/IP Slave]**

![[Figure 1.3.3.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_3.png>) 

![[Figure 1.3.3.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_4.png>) 

<br>

**4. Description of each item**

{% hint style="info" %}
\.      [IP Setting]

\.      Fixed IP: User sets the IP address, subnet mask, and gateway information.

\.      Dynamic Allocation (DHCP): An IP address is assigned from the DHCP server.
{% endhint %}

{% hint style="info" %}
\.      [Input Upon Communication Error (Action in Bus Error)]

\.      Clear: Initializes all inputs to 0 when a communication error occurs.

\.      Hold: Maintains the last valid input value when a communication error occurs.
{% endhint %}

{% hint style="info" %}
\.      [Communication Error Allowable Time (Error Allowed Time)]

\.      If a communication error persists for the specified allowed time, a fieldbus error signal and alarm are output.
{% endhint %}

{% hint style="info" %}
\.      [Input Byte Count (Input Byte)]

\.      Input Byte Count: Sets the size of the data input from the master -> slave.

\.      O -> T: Originator(Master) -> Target (Slave)
{% endhint %}

{% hint style="info" %}
\.      [Output Byte Count (Output Byte)]

\.      Output Byte Count: Sets the size of the data output from the slave -> master.

\.      T -> O: Target (Slave) -> Originator (Master)
{% endhint %}

{% hint style="info" %}
\.      [Run / Idle Header]

\.      The CIFX-50 RE EtherNet/IP Adapter applied to the controller uses 32-bit Run/Idle header when exchanging IO with the scanner (default).

\.      Please set whether to use the input and output 32-bit Run/Idle Header appropriately according to the scanner specifications.
{% endhint %}

<br>

{% hint style="info" %}
\.        [Quick Connect]

\.        EtherNet/IP supports the Quick Connect function.

\.        If the Quick Connect function is required, please set the EtherNet/IP Adapter using Sycon.net.

\.        (1) Products that support the Quick Connection function for the master and slaves are required  
\.        (2) Quick Connect cannot be used when using Auto Negotiation  
\.        (3) Quick Connect cannot be used when using Auto MDI-X  
\.        (4) 100 Mbit/s, Full Duplex required  
{% endhint %}

<br>

**5. After completing the settings, check the communication status according to the procedure below.**

For the procedure to check the industrial communication status on the TP, refer to ("[**1.4 CIFX PCI Communication Monitoring**](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)").

![[Figure 1.3.3.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/3-EtherNet-IP/4-Slave_setting/image_5.png>)

<br>

**6. Assign IO blocks after completing the communication settings.**

{% hint style="info" %}
\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("[**4. Industrial Communication IO Block Assignment**](../../../4-io-block-allocation.md)").**
{% endhint %}
# 1.3.8.2 CC-Link Slave Settings

“[Please follow the "**1.3.1 CIFX PCI Slot Settings**" procedure and then proceed with the method below.](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      For CC-Link connector connection, please refer to the following.

\.      (“[\.      ("**1.2.2 Connector**")](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)”)
{% endhint %}

<br>

##### 1. Using the TP, select CC-Link slave in the industrial communication firmware settings and reboot the robot controller.

![[Figure 1.3.8.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_1.png>)

<br>

##### 2. Check the current communication protocol readiness status in industrial communication monitoring menu.

![[Figure 1.3.8.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_2.png>)

<br>

{% hint style="warning" %}
*\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

##### 3. Touch the menu to enter the slave settings screen.
*\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > CC-Link Slave]**

![[Figure 1.3.8.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_3.png>)

![[Figure 1.3.8.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/8-CC-Link/4-Slave_setting/image_4.png>)

<br>

##### 4. Description of each item

{% hint style="info" %}
\.      [Station Address]

\.      The CC-Link identifies the slave through the station address. (1–64).
{% endhint %}

{% hint style="info" %}
\.      [Communication Speed (Baudrate)]

\.      You can select from 156, 625, 2500, 5000, and 10000 Kbit/s.
{% endhint %}

{% hint style="info" %}
\.      [CC-Link Version]

\.      Version 1: IO Station available, Extension Cycle not available

\.      Version 2: IO Station not available, Extension Cycle available
{% endhint %}

{% hint style="info" %}
\.      [Occupied Station Count]

\.      IO Station: Occupies 1

\.      Remote Device: 1–4 selectable

\.      The size of the assigned IO byte area varies depending on the number of stations occupied.
{% endhint %}

{% hint style="info" %}
\.      [Extension Cycle]

\.      Available in Version 2

\.      Remote Device: You can select from Single (1x), Double (2x), Quadruple (4x), and Octuple (8x).

\.      The size of the assigned IO byte area varies depending on the Extension Cycle.
{% endhint %}

<br>

{% hint style="info" %}
\.      **\.      For the IO Byte area, please refer to the link below.**

\.      **(“[\.      **("**1.3.8.1 CC-Link Slave Specifications**")**](../../3-cifx-pci-settings-industrial-communication/8-CC-Link/1-Specification-CC-Link-Slave.md)”)**
{% endhint %}

<br>

##### 5. After completing the settings, check the communication status according to the procedure below.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[For the procedure to check the industrial communication status on the TP, refer to ("**1.4 CIFX PCI Communication Monitoring**").](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

<br>

##### 6. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("**4. Industrial Communication IO Block Assignment**").**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
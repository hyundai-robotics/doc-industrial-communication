# 1.3.7.4 DeviceNet Slave Settings

“[Please follow the "**1.3.1 CIFX PCI Slot Settings**" procedure and then proceed with the method below.](../../../1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/1-Settings-firmware.md)" 절차를 따라 설정 이후 아래 방법을 진행해 주십시오.

<br>

{% hint style="info" %}
\.      **\.      [DeviceNet Slave EDS File Download]**

\.      “[\.      Please refer to "**5. Slave Device Description File**."](../../../5-slave-config-file.md)" 참고해 주십시오.
{% endhint %}

<br>

{% hint style="info" %}
\.      For DeviceNet connector connection, please refer to the following.

\.      (“[\.      ("**1.2.2 Connector**")](../../../1-cifx-pci-communication/2-cifx-pci-mounting-settings-industrial-communication-card/2-Connector.md)”)
{% endhint %}

<br>

##### 1. Using the TP, select a DeviceNet slave in the industrial communication firmware settings and reboot the robot controller.

![[Figure 1.3.7.4-1 Firmware Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_1.png>)

<br>

##### 2. Check the current communication protocol readiness status in industrial communication monitoring menu.

![[Figure 1.3.7.4-2 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_2.png>)

<br>

{% hint style="warning" %}
*\[Caution]**: If a configuration file set using Sycon.net is downloaded to the corresponding PCI slot, the TP settings will be ignored.
{% endhint %}

<br>

##### 3. Touch the menu to enter the slave settings screen.
*\[System > 2: Control Parameters > 11: Industrial Communication > 2: PCI Slave Slot Settings > DeviceNet Slave]**

![[Figure 1.3.7.4-3 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_3.png>)

![[Figure 1.3.7.4-4 Slave Settings]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_4.png>)

<br>

##### 4. Description of each item

{% hint style="info" %}
\.      [Station Address = Mac ID]

\.     The DeviceNet identifies a slave through the station address (MAC ID) (1–63).
{% endhint %}

{% hint style="info" %}
\.      [Communication Speed (Baudrate)]

\.      You can select among 125, 250, and 500 Kbit/s.
{% endhint %}

{% hint style="info" %}
\.      [Input Byte Count (Input Byte)]

\.      Input Byte Count: Sets the size of the data input from the master -> slave.
{% endhint %}

{% hint style="info" %}
\.      [Output Byte Count (Output Byte)]

\.      Output Byte Count: Sets the size of the data output from the slave -> master.
{% endhint %}


<br>

##### 5. After completing the settings, check the communication status according to the procedure below.

TP 에서 산업용 통신 상태를 확인하는 절차는 (“[For the procedure to check the industrial communication status on the TP, refer to ("**1.4 CIFX PCI Communication Monitoring**").](../../../1-cifx-pci-communication/4-cifx-pci-monitoring-industrial-communication/README.md)”)참고해 주십시오.

![[Figure 1.3.7.4-5 Industrial Communication Monitoring]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/7-DeviceNet/4-Slave_setting/image_5.png>)

<br>

##### 6. Assign IO blocks after completing the communication settings.

{% hint style="info" %}
\.      **통신 설정 완료 후 IO Block 을 할당하여 입출력 신호를 사용할 수 있습니다.  (“[\.      **After completing communication settings, you can use input/output signals by assigning IO blocks. Please refer to ("**4. Industrial Communication IO Block Assignment**").**](../../../4-io-block-allocation.md)”)를 확인해 주십시오.**
{% endhint %}
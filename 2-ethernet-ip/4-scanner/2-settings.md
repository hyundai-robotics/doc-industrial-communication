### 2.4.2 EtherNet/IP Scanner (Master) Settings

<br>

After completing the procedures in "[**2.1 Network Settings**](../../2-ethernet-ip/1-network.md)" and "[**2.2 License Settings**](../../2-ethernet-ip/2-license.md)" please proceed with the following steps.

<br>

**1. Touch the menu to enter the settings screen.**

<br>

**\[System > 2: Control Parameter > 11: Industrial Communication > 3: EtherNet/IP Settings]**

<br>

![[figure 2.4.2-1 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_1.png>) 

<br>

![[figure 2.4.2-2 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_2.png>) 

<br>

{% hint style="info" %}
   [Protocol Settings]

      - OFF : EtherNet/IP disable   
      - Adapter : EtherNet/IP Adapter mode   
      - Scanner : EtherNet/IP Scanner mode   
      - Adapter + Scanner : EtherNet/IP Adapter + Scanner mode   
{% endhint %}

<br>

{% hint style="info" %}
   [Port Settings]

      - General-purpose controller LAN1 to LAN3 are available (Ensure the status is "OK")
{% endhint %}

<br>

**2. Select "Scanner" mode and click the "Add Device" button to proceed to the next screen.**

<br>

![[figure 2.4.2-3 Scanner Add Device]](<../../_assets/2-ethernet-ip/4-scanner/img_3.png>) 

<br>

**3. Enter the settings to match the target device and save.**

<br>

{% hint style="info" %}
   [Device Settings]

      - Device No. : Device connection order (sequence of I/O data allocation)   
      - IP Address : IP address of the device   
      - Device Name : Name of the device (for identification purposes only; does not affect communication)   
      - RPI (ms) : Requested Packet Interval (I/O data update cycle)   
      - Connection Type   
            - Exclusive Owner (I/O) : Establishes a bidirectional I/O connection between the Scanner and Adapter   
            - Input Only : Connects to the Adapter's input signals only   
            - Listen Only : Connects to the input signals only while the Adapter is already connected to another Scanner   

      - Input (T > O) : Slave > Master connection   
      - Output (O > T) : Master > Slave connection   

      - Run/Idle Header : Select whether to include the I/O data header   
      - Instance No. : Instance number of the Input/Output Assembly for I/O data exchange   
      - IO Size : Size of I/O data (in bytes)   
{% endhint %}

<br>

{% hint style="info" %}
   - For connection examples, please refer to the manuals below.    
   - "[**2.3.3.1 Connecting External Adapter Devices - Crevis Remote IO**](3-connect-adapter/1-crevis.md)"

   - "[**2.3.3.2 Connecting External Adapter Devices - Wago Remote IO**](3-connect-adapter/2-wago.md)"

   - "[**2.3.3.3 Connecting External Adapter Devices - Hilscher CIFX PCI EtherNet/IP Adapter**](3-connect-adapter/3-pci.md)"

   - "[**2.3.3.4 Connecting External Adapter Devices - Baumer OM-70**](3-connect-adapter/4-baumer.md)"  
{% endhint %}

<br>

![[figure 2.4.2-4 Scanner Add Device]](<../../_assets/2-ethernet-ip/4-scanner/img_4.png>) 

<br>

**4. Click the "OK" button to transmit the communication settings.**

<br>

![[figure 2.4.2-5 Scanner Settings]](<../../_assets/2-ethernet-ip/4-scanner/img_5.png>) 

<br>

**5. Check the status to verify if the communication is successfully established.**

<br>

![[figure 2.4.2-6 Communication Status]](<../../_assets/2-ethernet-ip/4-scanner/img_6.png>) 

<br>

{% hint style="info" %}
   [Communication Status Check]   

      - License: Current license status   
      - Run: Indicates the operational status of the EtherNet/IP function   
      - Communication: Indicates the EtherNet/IP connection status   
      - Error: Indicates the EtherNet/IP error status    
{% endhint %}

<br>

{% hint style="info" %}
   [Device Number Color]   

      - Green: Communication connection OK   
      - Red: Communication connection NG (Failed)   
{% endhint %}

<br>

![[figure 2.4.2-7 Communication Status]](<../../_assets/2-ethernet-ip/4-scanner/img_7.png>) 

<br>

**6. After completing the communication settings, allocate the I/O Blocks.**

{% hint style="info" %}
   **After the communication settings are complete, you can use the input/output signals by allocating I/O Blocks. Please refer to ("[**5. Industrial Communication IO Reading and Writing**](../../5-io-block-allocation.md)")**
{% endhint %}
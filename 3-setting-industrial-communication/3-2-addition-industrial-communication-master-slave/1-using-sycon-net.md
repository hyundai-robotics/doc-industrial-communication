# 3.2.1 Using Sycon.net

When you need to use the industrial communication of the Hi6 controller, you are required to set the communication using the “**Sycon.net**” program. The setting method is as shown below. (Perform installation by referring to Section “[**1.1 Sycon.net**](../../1-install-program/1-1-sycon-net.md)”)

1. Connect the LAN3 port of the Hi6Com (Collaborative robot: Hi6MiniCom) to a PC.
2. &#x20;**** Regarding the communication setting method, you should refer to “Sycon.net v1.0500\DVD\_2018-12-1\_1\_0500\Documentation\4. You can also refer to the files in “Training Material\EN.”
   *   Names of the files to refer to

       1\) EtherNetIP Scanner - Configuration and Testing TM 02 EN.pdf

       2\) PROFIBUS DP Master - Configuration and Testing TM 02 EN.pdf

       3\) PROFINET IO Controller - Configuration and Testing TM 02 EN.pdf

{% hint style="info" %}
1\.      This example shows how to set the netX Driver for connecting the Hi6 driver.

2\.      You can set the IP address according to the setting of the controller.

3\.      How to set the EtherCAT Master (Connection of the CIFX card)
{% endhint %}

![](<../../_assets/image (6).png>)

{% hint style="info" %}
4\.      “Double-click” on the connected CIFX card (Figure).

5\.      Perform setting in Driver -> Netx Driver.
{% endhint %}

![](<../../_assets/image (13).png>)

{% hint style="info" %}
6\.      In netX Driver -> TCP Connection, perform setting as shown below. (The ID address&#x20;

&#x20;        may change depending on the controller, so you need to check it.)
{% endhint %}

![](<../../_assets/image (20).png>)

{% hint style="info" %}
7\.      Click on Device Assignment -> Scan. (If nothing appears: Change the device&#x20;

&#x20;        selection from suitale  only -> all and then click on Scan again).

8\.      Select the set communication (check the channel), and then “Apply,” and then “OK.”
{% endhint %}

![](<../../_assets/image (2).png>)

{% hint style="warning" %}
**\[Caution]**: If the location of the Access path is not cifX(num)\_Ch0, change it in Access path at the bottom and then apply
{% endhint %}

{% hint style="info" %}
9\.      Perform the necessary settings and right-click on the CIFX figure -> Download.
{% endhint %}

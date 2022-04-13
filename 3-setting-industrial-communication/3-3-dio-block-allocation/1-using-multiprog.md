# 3.3.1 Using Multiprog

After industrial communication is set, the following setting is necessary to perform DIO data exchange through ProconOS if the DIO block of the Hi6 controller is allocated to PLC. (Perform installation by referring to Section “[**1.2 Multiprog**](../../1-install-program/1-2-multiprog.md)”)

1. Regarding how to use after installation, refer to the manual included in Multiprog. –

{% hint style="info" %}
1\.      This shows a simple example of how to set Hi6 Multiprog.

2\.      You can set the IP address according to the setting of the controller.

3\.      Create a project (Execute Multiprog -> Click on “File” -> “New Project” -> Project&#x20;

&#x20;         Wizard and then OK).
{% endhint %}

![](<../../_assets/image (21).png>)

{% hint style="info" %}
4\.      Create a project according to the sequence.

(1)    Create a project.
{% endhint %}

![](<../../_assets/image (15).png>)

{% hint style="info" %}
(2) Set the POU and program language.
{% endhint %}

![](<../../_assets/image (18).png>)

{% hint style="info" %}
(3) Set the resource and type. (If there is no “Hi6” in Type, it means that installation has been performed in the wrong way. Checking whether the installation is performed correctly is required.)
{% endhint %}

![](<../../_assets/image (1).png>)

{% hint style="info" %}
(4) Create a task.
{% endhint %}

![](<../../_assets/image (8).png>)

{% hint style="info" %}
5\.      Set the project property.

(1)    Set the hardware property: Double-click on IO\_Configuration -> Set the Input/Output property
{% endhint %}

![](<../../_assets/image (16).png>)

{% hint style="info" %}
* Connection of HI6 DIO input <-> Multiprog output / HI6 DIO output <-> Multiprog input has been performed.
*   Connection of CIFX input <-> Multiprog input / HI6 DIO output <-> Multiprog output has been performed.

    &#x20;

(2)    How to set IO: Set the name. -> Set the task. -> Select the Board /IO module. -> Select and set the driver parameter (Offset 0: Hi6 Controller FB0.0. Unit: Byte).
{% endhint %}

![](<../../_assets/image (9).png>)

{% hint style="info" %}
(3) Set the IP address: Resource: Right-click on Hi6 (varies depending on the created name), and then match the IP in Settings -> Parameter to Hi6.
{% endhint %}

![](<../../_assets/image (4).png>)

{% hint style="info" %}
6\.      Write a PLC program. (Perform programming according to the needs of the user.)

7\.      Program downloading: Online -> Project Control -> Click on Download
{% endhint %}

![](<../../_assets/image (17).png>)

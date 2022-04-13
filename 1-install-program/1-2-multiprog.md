# 1.2 Multiprog

This is a PLC program to be used for DIO data exchange after connecting the PCI communication card. (Using it after setting “**PLC**” in “[**3.3 Setting the Industrial Communication DIO Block Allocation**](../3-setting-industrial-communication/3-3-dio-block-allocation/)” is required.)

**1.**     Download “**Hi6 Multiprog**” from Hyundai Robotics’ home page ([www.hyundai-robotics.com](http://www.hyundai-robotics.com)) -> Customer Support -> Application Software.

**2.**     Proceed to the installation according to the instructions below.

{% hint style="info" %}
1. Decompress the MP5.51 Express.zip file.
2. Run the MULTIPROG 5.51.msi file.
   * Perform installation with the setup.exe file if an error occurs during installation**.**
3. Decompress the MP eCLR Addon.zip file.
4. Run the I486\_LE\_GCC3\_eCLR.exe file
5. Decompress the MULTIPROG 5.51 Build 653.zip file.
6. Run the “multiprog\_set\_batch\_express.bat” file (run as administrator) in the MULTIPROG 5.51 Build 653 folder.

![](<../_assets/image (10).png>)

&#x20;

*   Additional work should be performed as below if there is a problem with building a project. It is possible that the files in the MULTIPROG 5.51 Build 653 folder are not copied properly.&#x20;

    \-> Copy all files of the MULTIPROG 5.51 Build 653 folder into the same folder as the MULTIPROG installation path. Find the “Default installation” location below and then paste the files of the MULTIPROG 5.51 Build 653 folder into the location.

    * Default installation: Paste the copied files into C:\Program Files (x86)\PHOENIX CONTACT Software\MULTIPROG 5.51 Express Build 653 folder (overwrite 3 files).

&#x20;

\*\*How to check\*\*

\-> Check the following files at the default installation (or installation) location.


{% endhint %}

![](../_assets/image.png)

(If you want to use the Pro version, you should install it using “**Hi6 MultiProg Development Environment Installation Guide.pdf.**” However, as the license for it is needed, you need to purchase it separately by requesting to the main office of Hyundai Robotics. Without a license, please note that the Pro version can be used only for 30 days.)

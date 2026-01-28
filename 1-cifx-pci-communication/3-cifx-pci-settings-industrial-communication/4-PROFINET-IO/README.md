### 1.3.4 PROFINET IO

This chapter describes the characteristics of the PROFINET IO master (controller) and slave (device) and how to set them. 

<br>

**PROFINET IO Overview**

PROFINET IO is an Ethernet-based open industrial communication protocol that has progressively evolved from PROFIBUS-DP and industrial Ethernet.

![[Figure 1.3.4-1 PROFINET IO]](<../../../_assets/1-cifx-pci-communication/3-cifx-pci-settings-industrial-communication/4-PROFINET-IO/image_1.png>) 

<br>

It follows the Provider-Consumer model for data exchange and can be classified into the following three classes of products.

**IO Controller Class**
   * Products that correspond to existing PROFIBUS-DP class 1 masters and are types of products in which automation programs such PLCs are running.

   * An IO controller supplies output data to the IO devices set to it and consumes the input data from them.

<br>

**IO Device Class**
  * Products that correspond to existing PROFIBUS-DP slaves and are connected to IO controllers such as PLCs through PROFINET IO.

  * An IO device supplies output data to the IO controller, provides input data, and consumes output data.

<br>

**IO Supervisor Class**
   * Products that correspond to existing PROFIBUS-DP class 2 masters and include those programming devices, PCs, HMIs that are designed for network configuration and diagnosis.

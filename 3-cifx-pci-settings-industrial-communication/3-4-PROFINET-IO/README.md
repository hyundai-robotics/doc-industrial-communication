# 3.4 PROFINET IO

This chapter describes the characteristics of the PROFINET IO master (controller) and slave (device) and the methods to set them.

<br>

##### PROFINET IO Overview

PROFINET IO is an Ethernet-based, open industrial communication protocol developed progressively from PROFIBUS-DP and the industrial Ethernet.

![[Figure 3.4-1 PROFINET IO]](<../../_assets/3-Settings-Industrial-Communication/3.4-PROFINET-IO/image_1.png>) 

<br>

PROFINET IO follows the provider and consumer model for data exchange and can be divided into the three following classes of products.

##### IO Controller Class
   * The products of this class correspond to existing PROFIBUS-DP class 1 masters and are similar to PLCs inside, which are run by an automation program.

   * The IO controller supplies output data to the IO devices set for itself and consumes input data.

<br>

##### IO Device Class
  * The products of this class correspond to existing PROFIBUS-DP slaves. They are connected to IO controllers, such as PLCs, via PROFINET IO.
    
  * The IO device supplies output data, provides input data to the IO controller, and consumes the output data.

<br>

##### IO Supervisor Class
   * The products of this class correspond to existing PROFIBUS-DP class 2 masters and are similar to programming devices, PCs, HMIs, etc., which are designed for configuring and diagnosing networks. 

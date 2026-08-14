## 4.3 MRP Settings

BD671 can be configured as an MRP Client to use the cable redundancy function.
In addition to the basic PROFINET settings, configure the following settings to enable the MRP function.

1) Topology setting
<p align="center">
<img src="../_assets/4-pnio/mrp-topology.png"></img>
<em><p align="center">Topology </p></em>
</p>

2) MRP Client setting

<p align="center">
<img src="../_assets/4-pnio/mrp_set_client.png"></img>
<em><p align="center">MRP Client </p></em>
</p>

3) Watchdog Time Setting (Set to 200 ms or longer)

 - The Watchdog Time must be set to 200 ms or longer to allow the MRP Manager to perform network topology reconfiguration (see figure).

<p align="center">
<img src="../_assets/4-pnio/mrp_watchdog.png"></img>
<em><p align="center">Watchdog Time </p></em>
</p>



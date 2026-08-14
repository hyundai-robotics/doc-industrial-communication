## 4.2 PROFINET Status Monitoring

By selecting the **\[System > 2: Control Parameter > 11: Industrial Communication > 5: PROFINET Settings]** menu, you can monitor the PROFINET status by slot.

<p align="center">
<img src="../_assets/4-pnio/PROFINET_monitoring.png"></img>
<em><p align="center">PROFINET Status Monitoring Screen</p></em>
</p>

- Size: Indicates the set I/O size (unit: byte).
- Status: BAD (not in use or communication error), GOOD (communication normal)
- Counter: I/O update count (communication normal if it continuously increases)

<p align="center">
<img src="../_assets/4-pnio/profinet_LED.png"></img>
<em><p align="center">BD671(PROFINET) </p></em>
</p>

* The version information is indicated by the LED blinking pattern during boot-up.
    - MCU: 1 (Major), 5 (Minor)
    - DSP: 4 (Major), 6 (Minor)
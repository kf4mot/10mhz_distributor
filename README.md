# 10mhz_distributor
Copyright Julian White, 2020
Licensed under CERN-OHL-S version 2
**Work in progress**

A 10 Mhz 3 channel distribution amplifier and low pass filter designed to integrate in a BG7TBL GPSDO. A 5th. order LPF on both the input and outputs allows the input to come from either sine or square waves and produce a sine output of around 10 dBm.

*This text will be italic*

**Notes worth reading**

1. Schematic and BOM show The Qorvo TQP369182 as the amp. TQP369180 was the amp actually used on the first board. The extra gain of the 182 seems unnecessary when driven with a 5V square wave and I suspect the extra gain may cause oscillation. Bias resistors remain at 91Ω. Upgrade at your own risk and let me know how it goes if you try.
1. Pads for a optional attn. are on the input. Untested.
1. Pads for a optional isolation transformer are on the 3rd. output. Untested.
1. Item 3
   1. Item 3a
   1. Item 3b


http://github.com - automatic!

[Schematic](https://github.com/kf4mot/10mhz_distributor/blob/master/10mhz_distributor_r1.pdf)

[comment]: # (This actually is the most platform independent comment/needs blank line before)

![Completed](https://github.com/kf4mot/10mhz_distributor/blob/master/images/finished-gpsdo.jpg "Completed")

![BoardTop](https://github.com/kf4mot/10mhz_distributor/blob/master/images/board-assy-top.jpg)

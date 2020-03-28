# 10mhz_distributor
A 10 MHz 3 channel distribution amplifier and low pass filter designed to integrate in a BG7TBL GPSDO. A 5th. order LPF on both the input and outputs allows the input to come from either sine or square waves and produce a sine output of around 10 dBm.

*This text will be italic*

**Notes worth reading**

1. Schematic and BOM show The Qorvo TQP369182 as the amp. TQP369180 was the amp actually used on the first board. The extra gain of the 182 seems unnecessary when driven with a 5V square wave and I suspect the extra gain may cause oscillation. Bias resistors remain at 91Ω. Upgrade at your own risk and let me know how it goes if you try.
1. Pads for a optional attn. are on the input. Untested.
1. Pads for a optional isolation transformer are on the 3rd. output. Untested.
1. Jitter and delay are still untested, but assumed good enough for a inexpensive GPSDO. If you build it and have the lab to test please share your results.
1. Item x
   1. Item xa
   1. Item xb
   
 **Future Work**
 
 1.

[Licensed under CERN-OHL-S V2. Julian White, 2020](https://www.ohwr.org/project/cernohl/wikis/home)

[Schematic](https://github.com/kf4mot/10mhz_distributor/blob/master/10mhz_distributor_r1.pdf)

[comment]: # (This actually is the most platform independent comment/needs blank line before)

![Completed](https://github.com/kf4mot/10mhz_distributor/blob/master/images/finished-gpsdo.jpg "Completed")

![BoardTop](https://github.com/kf4mot/10mhz_distributor/blob/master/images/board-assy-top.jpg)

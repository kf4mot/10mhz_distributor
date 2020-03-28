# 10mhz_distributor
A 10 MHz 3 channel distribution amplifier and low pass filter designed to integrate into a BG7TBL GPSDO. A 5th. order LPF on both the input and outputs allows it to be driven with either sine or square waves and produce a sine output of around 12 dBm into a 50Ω load.
Power consumption is about 130 mA @12V.

**Notes worth reading**

1. Schematic and BOM show The Qorvo TQP369182 as the MMIC. TQP369180 was actually used on the first board. The extra gain of the 182 seems unnecessary when driven with a 5V square wave and it may cause oscillation based on past experience. Bias resistors remain at 91Ω. Upgrade at your own risk and let me know how it goes if you try it or any other MMIC.
1. Pads for a optional attn. are on the input. *Trace that shorts R2 should be cut.* **Untested.**
1. Pads for a optional isolation transformer are on the 3rd. output. **Untested.**
1. Jitter and delay/phase shift are untested, but assumed good enough for a inexpensive GPSDO. If you build it and have the lab to test please share your results.
1. I left the input BNC (J3) off of mine and ran a internal wire to the GPSDO output. The BNC could be added by those that want the option to loop the clock or any other suitable input back into the distribution amp. Or those that want to use this as a stand alone general purpose distribution amp.
1. The 50Ω input load (R11) is 0603 size because I happen to have it in my inventory. You could use a 1206 at the R1 position if prefered. Or probably left off altogether if you're driving with a sinewave and bypassing the input filter.
   
Attenuator table for 1% resistors
Attn. |R2 | R1, R3
------------ | ------------- | ---------
3 dB| 17.8Ω | 294Ω
6 dB| 37.4Ω | 150Ω
10 dB | 71.5Ω | 95.3Ω

[Attenuator Calc](https://www.pasternack.com/t-calculator-pi-attn.aspx)

[Schematic](https://github.com/kf4mot/10mhz_distributor/blob/master/hardware/10mhz_distributor_r1.pdf)

[Licensed under CERN-OHL-S V2. Julian White, 2020](https://www.ohwr.org/project/cernohl/wikis/home)

![Complete](https://github.com/kf4mot/10mhz_distributor/blob/master/images/finished-gpsdo.jpg "Complete")

![BoardTop](https://github.com/kf4mot/10mhz_distributor/blob/master/images/board-assy-top.jpg "Board Top")

![BoardTop 3D](https://github.com/kf4mot/10mhz_distributor/blob/master/images/10mhz_distributor-3d-view.jpg "Board Top 3D")

![](https://github.com/kf4mot/10mhz_distributor/blob/master/images/scope-in-out-10mhz.jpg "Input vs. Output")

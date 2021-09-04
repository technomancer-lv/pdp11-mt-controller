# pdp11-mt-controller
Magnetic tape drive controller that lets connect CM5300 tape drive to soviet made PDP-11 compatible computers.

Main idea of this project is to create a magnetic tape drive controller for soviet made PDP-11 compatible computers. There exists at least four different soviet controllers of this kind, but only a few has survived, not all work with standard MT device driver and none of them are documented well enough to make a replica. I'm planning to base my design on original DEC TM11 and TU10 devices that are very well documented with schematics and precise descriptions available online. Also, this kind of approach would make my controller fully compatible with standard MT device driver. Core of the controller will be a FPGA, mainly because this would make recreating and adapting a logic design easier. There should be made several modifications, for example, TM11 controller is Unibus based, but I need it to to work on a Qbus. Also, CM5300 tape drive control signals are a bit different than TU10 control signals, so tape drive interface should be adapted too.
FPGA logic is designed in Quartus v13.0.1
PCB is designed in P-CAD 2006

This project is in early and slow prototype stage. Prototype board is produced and electrically tested in one piece. FPGA is fully connected to all required signals. Board can be accessed over Qbus. Interrupts and DMA are working. Tape drive can be fully controlled.\
Updates about this project are posted in this twitter thread: https://twitter.com/nuclearlighter/status/1393282838120763399

**Next steps:**\
Tape drive errors\
Proper overall testing (XXDP tests)\
STM32 for configuration - proof of concept\
STM32 as an USB device - proof of concept\
Choose STM32 controller for use on new board\
Order a bus drivers from Russia (N530AP2)

**On future:**\
Next revision board\
Additional RK05 drive connector (next project)\
Maintenance panel mockup (for fun)\
STM32 MCU for FPGA configuration\
Possibly an USB interface for tape imaging directly to PC\
Simple firmware upgrade over USB od even from RT-11 over Qbus (for fun)\
Possibly a small run of boards if anyone will be interested\
Schematics for new board, BOM\
Some kind of an ASCII image standard for imaging a tape data\
Small boards for tape drive connectors with IDC connector for cable\
Maybe additional board for programming and debug connectors

**Special thanks:**\
**bitsavers.org** for providing all detailed documentation on TM11, TU10 and other DEC parts\
members of **phantom.sannata.org** russian retrocomputing forum for helping with materials, documentation and various sugestions\
members of **robotrontechnik.de** german retrocomputing forum for their archive of soviet block computer equipment documentation

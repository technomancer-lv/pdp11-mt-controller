# pdp11-mt-controller
Magnetic tape drive controller that lets connect CM5300 tape drive to soviet made PDP-11 compatible computers.

At the moment this is only an idea. I'm studying DEC TM11 manuals nd schematics, I'm trying to find as much as possible information about soviet made tape drive controllers. There were Q-bus based quad boards that soviets made for Elektronika-60 and DVK computers, but seems that no board are found in full working condition. Or there are no full schematics with onboard ROM dumps.

I'm developing prototype board, based on Altera FPGA to test basic things - Q-bus addressing, DMA and IRQ functionality, tape drive connectivity, available resources. There will be more info on this as soon as I'll finish prototype PCB and will make some simple logics design. Board is almost finished and I hope to order it with other boards in this year. If I'll succeed with the tape drive, it seems that this board could be used to also develop an RK05 compatible drive controller.

# The Mini V853s Board

## About the chip

A brief introduction is below, from [the docs on Allwinner's Development Community](https://v853.docs.aw-ol.com/en/)
```
[Allwinner V853-High-performance edge AI vision processing chip]

V853 is a new generation of high-performance, low-power processor SOC launched for the field of intelligent vision. It can be widely used in intelligent upgrade related industries such as intelligent door locks, intelligent attendance access control, network cameras, driving recorders, and intelligent desk lamps. .

V853 integrates Arm Cortex-A7 and RISC-V E907 dual CPU, built-in maximum 1T computing power NPU, uses Allwinner's self-developed Smart video engine, supports up to 5M@25fps H.265 encoding and 5M@25fps H.264 encoding and decoding, and at the same time Integrated high-performance ISP image processor to provide customers with professional-level image quality. V853 also supports 16-bit DDR3/DDR3L to meet the high bandwidth requirements of various products; supports 4lane MIPI-CSI/DVP/MIPI-DSI/RGB and other rich dedicated video input and output interfaces to meet the needs of various AI vision products; advanced The 22nm process has better power consumption and smaller chip area.
```

## What is the focus of this project?
Yes, as you can see, the chip is brandy new and powerful. All the developmemnt board is big and expensive (because they are designed to verify, not DIY).So we thinks that it would be very nice to design a low-cost and powerful board for us personal developers. The board is designed to be as easy as we can (That's why we not use an external DDR3), and the components on the board is large than the actual products (typically 0603). Besides, what we really want is cost down.

## How to use the project
Please clone it first. Then, we can open it and see the directories and files in it. The structure is described below:
|Path|Description|
|:-:|:-:|
|Hardware/|SCH, PCB, and some useful datasheet|
|System/|The patches we did to the allwinner SDK on the kernel|
|Software/|The upper-level libraries and applications|

### Make your own board
The SCH and PCB is designed by LCEDA Pro. You may install it on your PC and edit the SCH and PCB on your own, then make your PCB; otherwise simply send the Gerber files (If there is) to a PCB manufacturer and ... You know.

### Compile the System
This is on a todo list and some updates will be done ASAP.

### Develop the application
It seems that it's not the time to do that, but it can be done later.

## TODO List

- [x] Finish the SCH

- [ ] Finish the PCB
    - [x] Place components
    - [ ] Wire it
    - [ ] Check and fix

- [ ] Develop and build the Linux kernel driver

## Contributing
We welcome contributions. Just fork and pull!

## License
All under GPL-3.

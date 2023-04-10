# Tides - V1
A clone of the Mutable Instruments Tides version 1 module with the use of the STM32F103 Blue Pill board.

<img height="500" src="https://user-images.githubusercontent.com/97026614/230910245-861a7b17-5967-4f9c-9a85-5b213ca0f8cf.jpg"> <img height="500" src="https://user-images.githubusercontent.com/97026614/230910377-67708e92-2e86-4ca6-b515-2f7fa9436733.jpg">

<img height="500" src="https://user-images.githubusercontent.com/97026614/230910586-5f44e4d0-a1cd-44df-992c-efb6c34d0d89.jpg"> <img height="500" src="https://user-images.githubusercontent.com/97026614/230910798-77a06e8b-d52b-4964-bed8-b3031a3c6769.jpg">

## Module Build and PCBs
If you want to build the module yourself, I uploaded firmware, schematic, BOM and Gerber files for the PCB.

There are two different versions for the control board, an "original" and a "Thonk" version.
Reason is that for my own module, I am using specific potentiometers - 16K4 series from Supertech Electronics - and 3.5mm jack sockets - MJ-355 from Marushin - available at my local electronics shop.

<img width="300" alt="OrigCtrlPCBFront" src="https://user-images.githubusercontent.com/97026614/230913339-03c6ba1d-3a83-4cbc-a96a-c415498f99b9.png">

However, since most DIY projects for Eurorack modules out there are using potentiometers from ALPHA and so-called THONKICONN jacks, as they are provided by Thonk in the UK, I also created a version with footprints for those components.
Choose the one you need.

<img width="300" alt="CtrlPCBThonk" src="https://user-images.githubusercontent.com/97026614/230913456-7f74d3d0-3f92-4ab7-9388-9e2fb55da0b8.png">

The layout of the main PCB is slightly different for both versions, as I needed to relocate the board connection points due to the size difference of the jacks in both versions. Make sure to use the correct pair of Gerber files.

<img width="300" alt="MainPCB" src="https://user-images.githubusercontent.com/97026614/230913521-842da377-7302-4a35-ab89-c16e38aaa3ca.png">

I created the Gerber files with the online tool EasyEDA and ordered it at JLCPCB.
I cannot guarantee, if this set of zipped Gerber files works also for other providers, like e.g. PCBWay. I have not tried that. But I saw online, that others did it.

## Panel Layout
I added the information about hole coordinates for the front panel in the folder PanelLayout, referring to the component layout in the Gerber files.

## Additional Information about specific Components
Most of the components are through-hole, including the microchip part, thanks to the available Blue Pill board. There are a few SMD components, which I listed here.
- DAC8552 (DAC, 8-VSSOP package, the most challenging component due to its size)
- LM1117-3.3 (voltage regulator, SOT223 package)
- LM4040B25 and LM4040B10 (voltage regulators, SOT23 package)
- MMBT3904 (SMD version of the 2N3904 transistor, SOT23 Package)
- 0.1uF bypass caps for ICs (1608 package)

Concerning the resistor size, I am usually using small-size resistors, about half the length of the usual size, so they need less space on the PCB. If you want to use my Gerber files, you have to consider tht fact. You might still use normal size resistors and put them in a standing position on the boards. Should also work fine.

## Firmware
I shared the .hex files for the STM32F103 chip (bootloader and main) in the folder Firmware.

The upload process is the same, as for my Braids clone. You can check out my [Braids video](https://youtu.be/TBMySGm7jKk) about how to program the Blue Pill board.

## Alternative Firmware (Mutated Mutables)
Besides the adjusted original firmware from Mutable Instruments, I also added an alternative firmware from Tim Churches in the folder Firmware, called "Mutated Mutables".
The .hex files are also adjusted to work with the Blue Pill board and my schematics.

You find detailed information about the alternative firmware and functions on Tim Churches' website: [http://timchurches.github.io/Mutated-Mutables/](http://timchurches.github.io/Mutated-Mutables/)

## STM32F103 Version
CAUTION! There are three different versions of the Blue Pill board available.
The difference is the version of the ST32F103 microchip on the board.
The versions differ in the flash memory size:
- STM32F103C6: 32kB flash memory
- STM32F103C8: 64kB flash memory
- STM32F103CB: 128kB flash memory

The code size requires the 128kB version.
However, that version is currently (Feb2023) difficult to find, if available at all.

I gave it a try and bought the 64kB version.
Surprisingly, the programmer showed 128kB available flash memory, and the code could be loaded.
I tried it with several boards.
So it seems STM3F103C8 is ok for this module.

If you want to see more about the chip programming process, you can check out my [YouTube video](https://youtu.be/TBMySGm7jKk).

## Calibration
The calibration procedure is the same, as the one for the original module from Mutable Instruments.

1. Disconnect any signal from the FM input,
2. Connect the pitch CV output of a well-calibrated keyboard interface or MIDI-CV converter to the 1V/O input.
3. Set the COARSE and FINE knobs to 12 o'clock position.
4. Go to CAL. in the options list.
5. Push the encoder for 1s. The screen displays >C2.
6. Send a voltage of 1V to the 1V/O input.
7. Click on the encoder. The screen displays >C4.
8. Send a voltage of 3V to the 1V/O input.
9. Click on the encoder to finish calibration.

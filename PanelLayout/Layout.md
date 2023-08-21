## Panel Layout for PCB

The panel dimensions provided in the section "Original Design" below are based on my own module build, since I am not following the standard HP (1HP eq. 5.08mm) size. An alternative by building an HP-standard size panel can be found in the section "HP Standard Design" further below.

### Original Design
Coordinates given in the table fit to the layout of components given in the PCBc in folder GerberFiles.
The layout is the same for both versions.

Panel size: 60mm x 128.5mm

The numbers in the table are refering to the numbers in the picture below.
Coordinates origin is the lower left corner of the panel.


| No. | X-coord. [mm] | Y-coord. [mm] | Comment |
| --- | --- | --- | --- |
| 1 | 10 | 107 | Select Button Mode |
| 2 | 18 | 107 | LED |
| 3 | 18 | 100 | LED |
| 4 | 30 | 100 | Frequency Pot |
| 5 | 49 | 100 | FM Pot |
| 6 | 10 | 93 | Select Button Range |
| 7 | 18 | 93 | LED |
| 8 | 11 | 70 | Shape Pot |
| 9 | 30 | 70 | Slope Pot |
| 10 | 49 | 70 | Smoothness Pot |
| 11 | 11 | 50 | Shape CV Jack |
| 12 | 30 | 50 | Slope CV Jack |
| 13 | 49 | 50 | Smoothness CV Jack |
| 14 | 8 | 30 | Trigger Jack |
| 15 | 19 | 30 | Freeze Jack |
| 16 | 30 | 30 | 1Volt/Oct CV Jack |
| 17 | 41 | 30 | FM CV Jack |
| 18 | 52 | 30 | Level CV Jack |
| 19 | 8 | 15 | Clock Jack |
| 20 | 19 | 15 | High Out Jack |
| 21 | 30 | 15 | Low Out Jack |
| 22 | 41 | 15 | Unipolar Out Jack |
| 23 | 52 | 15 | Bipolar Out Jack |

<img height="1200" src="https://user-images.githubusercontent.com/97026614/231600963-cc30b80b-ffd1-4570-98a6-dfe5f1f9cb4b.png"> 

### HP Standard Design
For building the panel with a size following the HP standard, you can use the panel Gerber file provided in the folder "GerberFiles".
I ordered my own panel via such gerber file built out of PCB material.

Here are a few parameters of the panel.
| Parameter | Value |
| --- | --- |
| Width | 12HP |
| Pot hole diameter | 8mm |
| Jack hole diameter | 6.1mm |
| Tact switch hole diameter | 5.1 mm |
| LED hole diameter | 3.1mm|
| Mounting hole diameter | 3.2mm|

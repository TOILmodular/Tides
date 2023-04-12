# BOM

| Description | Value | Quantity | |
| --- | --- | --- | --- |
| Resistor 1/4W | 100R | 2 | |
| Resistor 1/4W | 270R | 1 | |
| Resistor 1/4W | 2.4K | 2 | |
| Resistor 1/4W | 3.3K | 3 | |
| Resistor 1/4W | 4.7K | 2 | |
| Resistor 1/4W | 10K | 5 | |
| Resistor 1/4W | 20K | 1 | |
| Resistor 1/4W | 27K | 1 | |
| Resistor 1/4W | 30K | 1 | |
| Resistor 1/4W | 33K | 5 | |
| Resistor 1/4W | 39K | 1 | |
| Resistor 1/4W | 100K | 16 | |
| Resistor 1/4W | 120K | 3 | |
| Resistor 1/4W | 220K | 2 | |
| Resistor 1/4W | 3.3M | 1 | |
| Resistor 1/4W | LEDR | 3 | see footnote *) |
| Resistor 1/4W | LEDG | 3 | see footnote *) |
| Capacitor Electrolytic | 47uF | 2 | |
| Capacitor Electrolytic | 22uF | 3 | |
| Capacitor Ceramic | 3.3uF | 1 | |
| Capacitor Ceramic | 0.47uF | 2 | |
| Capacitor Ceramic | 0.1uF | 7 | SMD (1608) |
| Capacitor Ceramic | 0.01uF | 3 | |
| Capacitor Ceramic | 1000pF | 3 | |
| Capacitor Ceramic | 220pF | 4 | |
| LED | 2-color, common cathode | 8 | |
| Transistor | MMBT3904 | 5 | SMD (SOT-23-3) |

| Op Amp | NJM4580 or TL072 | 1 | SMD (8-SOIC) |
| Op Amp | MCP6004 | 2 | SMD (14-SOIC) |
| DAC | PCM5100APW | 1 | SMD (20-TSSOP) |
| Microcontroller | STM32F373CCT6 | 1 | SMD (48-LQFP) |
| LED Driver | TLC59281DBQ | 1 | SMD (24-SSOP) |
| Oscillator Crystal | 8MHz | 1 | leg distance 4.8mm |
| Voltage Regulator | LD2981ABU33 | 1 | SMD (SOT-89-3) |
| Voltage Regulator | R-78E3.3-0.5 | 1 | |
| Voltage Regulator | LM4040B10 | 1 | SMD (SOT-23-3) |
| Inductor | 33uH | 1 | axial THT, if you use my PCB design |
| Ferrite Bead | BLM18R | 3 | SMD (1608) |
| Potentiometer | B10K | 7 | |
| Mono Jack | 3.5mm | 10 | |
| Switch | Tactile | 2 | e.g. Mouser: TL1105SPF160Q1RBLK |
| Header | 2.54mm Male 1x7 | 4 | Connector Main Board |
| Header | 2.54mm Female 1x7 | 4 | Connector Control Board |
| Header | 2.54mm Female 2x5 | 1 | Power Connector |

*) Depending on the LEDs used, they might be too bright. The resistor labeled as "LED" can be used to adjust the brightness by reducing the current from the common anode to each LED. The original design from Mutable Instruments does not include that resistor. So if you use the same LEDs, as in the commercial module, you can just bridge the resistor points with a wire. Otherwise try out different resistor values to adjust the LED brightness.


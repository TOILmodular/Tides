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
| Trimmer | 50K | 1 | multi-turn |
| Capacitor Electrolytic | 47uF | 2 | |
| Capacitor Electrolytic | 22uF | 3 | |
| Capacitor Ceramic | 3.3uF | 1 | |
| Capacitor Ceramic | 0.47uF | 2 | |
| Capacitor Ceramic | 0.1uF | 7 | SMD (1608) |
| Capacitor Ceramic | 0.01uF | 3 | |
| Capacitor Ceramic | 1000pF | 3 | |
| Capacitor Ceramic | 220pF | 4 | |
| LED | 2-color, common cathode | 3 | |
| Transistor | MMBT3904 | 5 | SMD (SOT-23-3) |
| Op Amp | TL074 | 1 | |
| Op Amp | MCP6004 | 1 | |
| Op Amp | MCP6002 | 1 | |
| DAC | DAC8552 | 1 | SMD (8-VSSOP) |
| Development Board | STM32F103 Blue Pill (128kB) | 1 | |
| Voltage Regulator | LM1117-3.3 | 2 | SMD (SOT-223) |
| Voltage Regulator | LM4040B10 | 1 | SMD (SOT-23-3) |
| Voltage Regulator | LM4040B25 | 1 | SMD (SOT-23-3) |
| Potentiometer | B10K | 5 | |
| Mono Jack | 3.5mm | 13 | |
| Switch | Tactile | 2 | e.g. Mouser: TL1105SPF160Q1RBLK |
| Header | 2.54mm Male 1x2 | 2 | Connector Main Board |
| Header | 2.54mm Male 1x4 | 1 | Connector Main Board |
| Header | 2.54mm Male 1x7 | 1 | Connector Main Board |
| Header | 2.54mm Male 1x11 | 1 | Connector Main Board |
| Header | 2.54mm Female 1x2 | 2 | Connector Control Board |
| Header | 2.54mm Female 1x4 | 1 | Connector Control Board |
| Header | 2.54mm Female 1x7 | 1 | Connector Control Board |
| Header | 2.54mm Female 1x11 | 1 | Connector Control Board |
| Header | 2.54mm Female 1x20 | 2 | Socket Connector for Blue Pill Board |
| Header | 2.54mm Male 2x5 | 1 | Power Connector |

*) Depending on the LEDs used, they might be too bright. The resistors labeled as "LEDR" and "LEDG" can be used to adjust the brightness by reducing the current to each LED. The original design from Mutable Instruments lists 100R resistors for both the red and green part of the 2-color LEDs. I changed the values to 1K for red and 4.7K for green (blue in my case) for the LEDs used in my module.

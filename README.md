# promicro_smol

`promicro_smol` is a compact shield PCB for the nRF52840 Supermini/Pro Micro used in DIY SlimeVR trackers. It has an IMU, magnetometer, two buttons, RGB LED, battery pads and voltage reading functionality. It is designed to be compatible with existing Chrysalis enclosures (not yet verified). Production files can be found in `/pcb/production/`.

## Why I Made This

This project started as a modification of Chrysalis to support operation at 1.8V logic and to add a few features. The main changes were to make the magnetometer support 1.8V logic, switch to a MOSFET-controlled RGB LED, add a battery voltage divider for better capacity measurement, and to make sure SWD pads are accessible through a board cutout. I made these changes ensuring the board is optimized for JLCPCB economic assembly.

## Pictures

![3D Model](./images/kicad_pdDzEOa1Xo.png)

### Schematic
[View Online](https://kicanvas.org/?repo=https%3A%2F%2Fgithub.com%2Fpicafe%2Fpromicro_smol%2Fblob%2Fmain%2Fpcb%2Fpromicro_smol.kicad_sch)
![Schematic Image](./images/kicad_0tHGa6QgOD.png)
### PCB
[View Online](https://kicanvas.org/?repo=https%3A%2F%2Fgithub.com%2Fpicafe%2Fpromicro_smol%2Fblob%2Fmain%2Fpcb%2Fpromicro_smol.kicad_pcb)


## Credits and Attribution

This work is derived from the [kounocom/Chrysalis](https://github.com/kounocom/Chrysalis) hardware project.

Files from `/pcb/Chrysalis-Footprints.pretty` are sourced from the Chrysalis project with and without modifications.

The upstream project is provided under CERN-OHL-S-2.0, and this repository includes the applicable license text in `LICENSE.md`.

## Bill of Materials


| Item         | Value / Part                                                                                                                                                                                                                                                                                                                          | Quantity |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- |
| MCU module   | ProMicro nRF52840 (can be found on Aliexpress)                                                                                                                                                                                                                                                                                        | 1        |
| IMU          | [LSM6DSVQTR (C17496470)](https://www.lcsc.com/product-detail/C17496470.html)                                                                                                                                                                                                                                                             | 1        |
| Magnetometer | [QMC6309 (C5439871)](https://www.lcsc.com/product-detail/C5439871.html)                                                                                                                                                                                                                                                               | 1        |
| N-FETs       | [HL3134KT (C52204685)](https://www.lcsc.com/product-detail/C52204685.html)                                                                                                                                                                                                                                                            | 5        |
| RGB LED      | [NH-B2020RGBA-HF (C2874116)](https://www.lcsc.com/product-detail/C2874116.html)                                                                                                                                                                                                                                                       | 1        |
| Push buttons | [Tactile Button, 160gf (C318884)](https://www.lcsc.com/product-detail/C318884.html), [Tactile Button, 160gf (C720477)](https://www.lcsc.com/product-detail/C720477.html)                                                                                                                                                              | 2        |
| Resistors    | [100R (C25076)](https://www.lcsc.com/product-detail/C25076.html), [5.1k (C25905)](https://www.lcsc.com/product-detail/C25905.html), [10k (C25744)](https://www.lcsc.com/product-detail/C25744.html), [3M (C23156)](https://www.lcsc.com/product-detail/C23156.html), [4.7M (C23163)](https://www.lcsc.com/product-detail/C23163.html) | 12       |
| Capacitors   | [100nF (C307331)](https://www.lcsc.com/product-detail/C307331.html), [10nF (C15195)](https://www.lcsc.com/product-detail/C15195.html), [2.2uF (C23630)](https://www.lcsc.com/product-detail/C23630.html)                                                                                                                              | 4        |

Total Cost for JLCPCB assembly (2 units, 0.8mm thickness, lead-free HASL): $40

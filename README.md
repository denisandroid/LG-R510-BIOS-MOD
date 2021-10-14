# <small>LG R510 (QL8) BIOS MOD</small>

<b>Input:</b>
1. Original Last InsydeH20 Bios 3.5 (QL8L3F22)
2. Original Bios Flasher
3. _

<b>Warning:</b>
1. I am not responsible, whatever you do with the laptop you do everything at your own peril and risk.
2. Attention: all changes in BIOS are saved in permanent flash memory.
3. Sometimes a menu lock occurs, if you scroll through the menu categories and return to the desired item, the error disappears.

<b>Photos:</b>

<img src="https://github.com/denisandroid/LG-R510-BIOS-MOD/blob/master/photo/1.jpg" width="330" height="200" alt="Photo 1">

<b>Changes:</b>
1. Password setting <b>(DELETED)</b>

   | Name                  | Possible values                 | Stably | Recommendation  |
   | --------------------- | ------------------------------- | ------ | --------------  |
   | Force Clear           | +,-                             | +/-    | Added, Does not work   |
   | Supervisor Password   | PASS                            | +      |                 |
   | User Password         | PASS                            | +      |                 |

2. Added menu <b>(UlinProject ModA)</b>

   | Name                    | Possible values                 | Stably | Recommendation            |
   | ---------------------   | ------------------------------- | ------ | --------------            |
   | IDE Controller          | +,-                             | +      | SataController Default(+) |
   | HDC Configure           | IDE, AHCI, RAID                 | IDE/ACHI (+), RAID (?) | |
   | AHCI Option ROM Support | +, -                            | ?      | |
   | SATA Port [0-5] HotPlug | +, -                            | +      ||
   | ACPI Table/Features Control | MENU                        | +      ||
   | PCI Express Root Port 1 | MENU                            | +      ||
   | Chipset Configuration   | MENU                            | +      ||
   | USB Configuration       | MENU                            | +      ||
   | Video Configuration     | MENU                            | +      ||
   | Boot Configuration      | MENU                            | +      ||
   | PCI Configuration       | MENU                            | +      ||
   | Internal Devices Configurations | MENU                    | +      ||

3. Added menu <b>(Platform Power Managment)</b>
 
   | Name                  | Possible values                 | Stably | Recommendation  |
   | --------------------- | ------------------------------- | ------ | --------------  |
   | Break Event           | ACPI S3, Wake on PME, Wake on Modem Ring, Quickly S4 Resume, Auto wake on S5 | + ||
   | P-States              | +, -                            |        ||
   | Boot performance mode | Max Battery, Max Performace     | ?      ||
   | Thermal Mode          | -, TM1, TM2                     | +      ||
   | CMP Support           | Auto, -                         | +      ||
   | SMRR Support          | Auto, -                         | +      ||
   | C-States              | +, -                            | +      ||
   | Enhanced C-States     | +, -                            | +      ||
   | C-State Pop Down Mode | +, -                            | +      ||
   | C4 Exit Timing Mode   | Default, Fast, Slow, Force Slow | +      | Default(Fast), I choose(Default/Slow)    |
   | Hard C4E              | +, -                            | +      ||
   | Enable C6             | +, -                            | +      ||
   | EMTTM                 | +, -                            | +      ||
   | Bi-directional PROCHOT# | +, -                          | +      ||
   | Dynamic FSB Switching  | +, -                           | +      | Default(+), I choose(-, max performance) |
   | Turbo Mode             | +, -                           | +      | Default(+), I choose(-)     |
   | ACPI 3.0 T-States      | +, -                           | +      | Default(-), I choose(+)  |
   | DTS                    | +, -                           | +      ||
   | DTS Calibration        | +, -                           | +      ||
   | Thermal Trip Points Setting | Fan On[40-75], Throttle On[40-90] | +++ | I choose(FanOn 40, Throttle 90) |

4. Changed menu <b>(Advanced)</b>

   | Name                  | Possible values                 | Stably | Recommendation  |
   | --------------------- | ------------------------------- | ------ | --------------  |
   | UlinProject ModA      | MENU                     | +++    | +++ Added             |
   | Internal Devices Configurations | MENU                  | +      | DELETED, See UlinMenu |

5. Added menu <b>(ACPI Table/Features Control)</b>

   | Name                    | Possible values                 | Stably | Recommendation            |
   | ---------------------   | ------------------------------- | ------ | --------------            |
   | FACP - C2 Latency       | +,-                             | ?      ||
   | FACP - C3 Latency       | +,-                             | ?      ||
   | S4 wake up from RTC     | +,-                             | ?      ||
   | APIC - IO APIC          | +,-                             | ?      ||
   | HPET - HPET support     | +,-                             | ?      ||
   | Base Address            | FED00000h-FED03000h             | ?      ||
   
6. Added menu <b>(PCI Express Root Port 1)</b>

   | Name                    | Possible values                 | Stably | Recommendation            |
   | ---------------------   | ------------------------------- | ------ | --------------            |
   | PCI Express Root Port 1 | +,-                             | ?      ||
   | VC1 Enable              | Auto,-                          | ?      ||
   | VC1/TC Mapping          | TC0-TC7                         | ?      ||
   | ASPM                    | +,-                             | +      | See Chipset Configuration |
   | Automatic ASPM          | Auto,Manual                     | +      | See Chipset Configuration |
   | ASPM L0s                | -,Root,Endpoint,RootAndEndpoint | ?      ||
   | ASPM L1s                | -,Root,Endpoint,RootAndEndpoint | ?      ||
   | URR | +,-                             | ?      ||
   | FER | +,-                             | ?      ||
   | NFER | +,-                             | ?      ||
   | CER | +,-                             | ?      ||
   | CTO | +,-                             | ?      ||
   | SEFE | +,-                             | ?      ||
   | SENFE | +,-                             | ?      ||
   | SECE | +,-                             | ?      ||
   | PME Interrupt | +,-                             | ?      ||
   | PME SCI | +,-                             | ?      ||
   | Hot Plug SCI | +,-                             | ?      ||

7. Added menu <b>(Chipset Configuration)</b>

   <b>Setup Warning:</b>
   
   <b>Setting items on this screen to incorrect values</b>
   
   <b>May cause your system to malfunction!</b>
   
   
   | Name                    | Possible values                 | Stably | Recommendation            |
   | ---------------------   | ------------------------------- | ------ | --------------            |
   | CRID | +,-                             | ?      ||
   | Port 80h Cycles | PCI BUS,LPC BUS      | ?      ||
   | DMI Link ASPM Control | +,-            | +      |I choose(max performance)|
   | Automatic ASPM | +,-                   | +      |I choose(max performance)|
   | ASPM L0s Support | +,-                 | ?      ||
   | ASPM L0sL1 Support | +,-               | ?      ||
   | PCI Latency Timer | 32-248             | +      ||
   | Memory Thermal Management | MENU       | +      ||

8. Added menu <b>(Memory Thermal Management)</b>

   | Name                    | Possible values                 | Stably | Recommendation            |
   | ---------------------   | ------------------------------- | ------ | --------------            |
   | TM Mode                 | -,TM,Catastrophic               | ?      ||
   | TS on DIMM              | +,-                             | ?      ||
   | TM Lock                 | +,-                             | ?      ||

9. Added menu <b>(USB Configuration)</b>

   | Name                    | Possible values                 | Stably | Recommendation            |
   | ---------------------   | ------------------------------- | ------ | --------------            |
   | EHCI 1       | +,-                             | ?      ||
   | EHCI 2       | +,-                             | ?      ||
   | UHCI 1       | +,-                             | ?      ||
   | UHCI 2       | +,-                             | ?      ||
   | UHCI 3       | +,-                             | ?      ||
   | UHCI 4       | +,-                             | ?      ||
   | UHCI 5       | +,-                             | ?      ||
   | Per-Port Control       | +,-                   | ?      ||
   | Usb Port0      | +,-                           | ?      ||
   | Usb Port1       | +,-                          | ?      ||
   | Usb Port2       | +,-                          | ?      ||
   | Usb Port3       | +,-                          | ?      ||
   | Usb Port4       | +,-                          | ?      ||
   | Usb Port5       | +,-                          | ?      ||
   | Express Card       | +,-                       | ?      ||
   | USB Pre-fetch Feature    | +,-                 | ?      ||
   | USB Pre-fetch Time       | 4ms/2ms             | ?      ||

9. Added menu <b>(Video Configuration)</b>

   | Name                    | Possible values                 | Stably | Recommendation            |
   | ---------------------   | ------------------------------- | ------ | --------------            |
   | PEG Aperture Size       | 64,128,256                      | +      | I choose (256)            |
   | ASPM                    | +,-                             | +      ||
   | Automatic ASPM          | Auto,Manual                     | +      ||
   | ASPM L0s                | -,Root,Endpoint,RootAndEndpoint | ?      ||
   | ASPM L1s                | -,Root,Endpoint,RootAndEndpoint | ?      ||
   | ASPM L0s Aggressiveness | Normal, Aggressive, Ultra-aggressive | ? ||
   | Render Standby          | +,-                             | ?      ||
   | IGD - Device2,Function1 | +,-                             | ?      ||
   | IGD - Pre-allocat Memory| 64,128,256                      | +      | I choose (256)            |
   | IGD - DVMT Size         | 64,128,256                      | +      | I choose (256)            |
   | Clock Chip Initialize   | -,48Mhz,64Mhz                   | ?      ||
   | Enabled CK SSC          | +,-                             | ?      ||
   | IGD - Boot Type         | VBIOS Default, CRT, LFP, CRT+LFP, TV, LFP-SDVO, EFP, TV-SDVO, CRT+LFP-SDVO, CRT+EFP | ?      ||
   | IGD - LCD Panel Type (LVDS)   | 640x480, 800x600, 1024x768, 1280x1024, 1400x1050 (LVDS1), 1400x1050(LVDS2), 1600x1200 LVDS             | ?      ||
   | IGD - TV          | VBIOS, NTSC, PAL, SECAM                             | ?      ||
   | IGD - PAVP Mode          | -,Lite,High                    | +/-      | -/Lite (Stable), High (After a while, the chip freezes.)  |
   | IGD - Gfx Low Power Mode          | +,-                   | ?      ||
   
10. Added menu <b>(Boot Configuration)</b>

   | Name                    | Possible values                 | Stably | Recommendation            |
   | ---------------------   | ------------------------------- | ------ | --------------            |
   | Numlock                 | +,-                             | +      ||
   | Zip Emulation Type      | FDD, HDD                        | +      ||

11. Added menu <b>(PCI Configuration)</b>

   | Name                    | Possible values                 | Stably | Recommendation            |
   | ---------------------   | ------------------------------- | ------ | --------------            |
   | PCI Slot3 IRQ Priority  | Auto, IRG3-11                   | ?      ||
   | PCI Slot4 IRQ Priority  | Auto, IRG3-11                   | ?      ||

12. Changed menu <b>(Internal Devices Configurations)</b>
   
   | Name                    | Possible values                 | Stably | Recommendation            |
   | ---------------------   | ------------------------------- | ------ | --------------            |
   | Mode                    | CIR, FIR                        | ?      ||
   | Base I/O Address        | 2E8, 2F8, 3E8, 3F8              | ?      ||
   | Interrupt               | IRQ3, IRQ4                      | ?      ||
   | DMA Channel             | 1,2,3,4                         | +      ||
   | HIGH SPEED              | Normal, High                    | +      | I choose (High) |
   
   

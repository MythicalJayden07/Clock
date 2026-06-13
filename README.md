

# 6-Digit 7-Segment Display Clock
This is a custom digital clock featuring a 6-digit 7-segment display packed into a clean, rectangular desktop case. I designed this to blend custom 3D-printed mechanics with a sleek, premium look by keeping the messy electronics hidden and using a real glass front panel.
## The Inspiration
I’ve always loved the raw, industrial look of 7-segment displays, but most DIY clocks you see online either look like a total rat's nest of bare wires or they’re stuck inside chunky 3D-printed plastic boxes that just feel a bit cheap.
I wanted to make something that actually looks like a premium desktop piece you'd buy at a store, while keeping that precise, retro-tech HH: MM :SS readout. The goal was to have a pristine glass front with zero visible screws or clunky printed bezels, but still have quick, toolless access to the PCB whenever I want to mess with the hardware.
## PCB Schematic
The brain of the clock. The schematic handles the multiplexing for the 6-digit display, power management, and the ATmega328P microcontroller layout to ensure clean signal lines without ghosting on the digits. <img width="1206" height="832" alt="Screenshot 2026-06-02 140145" src="https://github.com/user-attachments/assets/900a614b-34dc-4c84-9032-c73800e1fb0d" />

## PCB Layout
A custom, compact board designed to slide perfectly into the case alignment channels. Component placement was adjusted so it sits perfectly behind the front glass face. <img width="818" height="821" alt="Screenshot 2026-06-02 140114" src="https://github.com/user-attachments/assets/9d055057-896f-4a38-9488-c5507e0d3153" />
<img width="988" height="491" alt="Screenshot 2026-06-02 140105" src="https://github.com/user-attachments/assets/16f87ff8-6518-4f57-8010-bae86cca908a" />
<img width="1510" height="681" alt="Screenshot 2026-06-02 140057" src="https://github.com/user-attachments/assets/7dfc4a32-2d05-4414-8ff9-6c093416efc4" />

## CAD Enclosure Design
The rectangular housing featuring the integrated top hinge and embedded slots for the neodymium magnets. This makes the door snap shut tight!!
<img width="1141" height="385" alt="Screenshot 2026-06-02 140409" src="https://github.com/user-attachments/assets/d703e863-4572-4e16-a16b-acab284590a3" />
<img width="954" height="630" alt="Screenshot 2026-06-02 140358" src="https://github.com/user-attachments/assets/809a65a8-98b2-49ff-80ca-1cc76260727b" />
<img width="766" height="469" alt="Screenshot 2026-06-02 140341" src="https://github.com/user-attachments/assets/a38b6b7f-9457-4ed6-9aba-47ac7d919f2c" />
<img width="848" height="651" alt="Screenshot 2026-06-02 140332" src="https://github.com/user-attachments/assets/c02ae9e7-8038-43bf-92e2-91f7fe5d8b46" />

## Bill of Materials (BOM)
[ClockBOM.csv](https://github.com/user-attachments/files/28500980/ClockBOM.csv)


| Reference | Qty | Value | Footprint / Details | Part Link |
| :--- | :---: | :--- | :--- | :--- |
| **U1** | 1 | ATmega328P-P | Package_DIP:DIP-28_W7.62mm Microcontroller | [Buy Link](https://www.mouser.in/ProductDetail/Microchip-Technology/ATMEGA328P-PU?qs=K8BHR703ZXguOQv3sKbWcg%3D%3D) |
| **U2 - U7** | 6 | TPIC6B595 | Package_DIP:DIP-20_W7.62mm Power Shift Register | [Buy Link](https://www.mouser.in/ProductDetail/Texas-Instruments/TPIC6B595N?qs=JHHQeKcAU3Cy7hDGJZD9fw%3D%3D) |
| **U8** | 1 | L7805 | Package_TO_SOT_THT:TO-220-3_Vertical Regulator | [Buy Link](https://www.mouser.in/ProductDetail/STMicroelectronics/L7805CV?qs=9NrABl3fj%2FqplZAHiYUxWg%3D%3D) |
| **DS1 - DS4** | 4 | SA18-11EWA | 1.8" Kingbright Red 7-Segment Display | [Buy Link](https://www.mouser.in/ProductDetail/Kingbright/SA18-11EWA?qs=JpELLRhtMc01ud%252BhiiNcbQ%3D%3D) |
| **DS5, DS6** | 2 | SA08-11GWA | 0.8" Kingbright Green 7-Segment Display | [Buy Link](https://www.mouser.in/ProductDetail/Kingbright/SA08-11GWA?qs=E09Sz5t5voVFPaAyTwzbvg%3D%3D) |
| **D1** | 1 | 1N5401 | Diode_THT:D_DO-201AD_Horizontal Rectifier | [Buy Link](https://www.mouser.in/ProductDetail/Diotec-Semiconductor/1N5401?qs=OlC7AqGiEDkgsZqkfh5%2F5g%3D%3D) |
| **Q1** | 1 | 2N3904 | Package_TO_SOT_THT:TO-92_Inline NPN Transistor | [Buy Link](https://www.mouser.in/ProductDetail/onsemi/2N3904BU?qs=or4AE2qAS%252Bd0Jdpn%2F8ktKg%3D%3D) |
| **F1** | 1 | 2A | Fuse:Fuse_Bourns_MF-RG300 Resettable PTC | [Buy Link](https://www.mouser.in/ProductDetail/Bourns/MF-RG300-0?qs=Zco4Fs67ctclSu06fHwNtw%3D%3D) |
| **Y1** | 1 | 16Mhz | Crystal:Crystal_HC49-U_Vertical Oscillator | [Buy Link](https://robu.in/product/hc49-s-16mhz-crystal-oscillator-pack-of-5/) |
| **C1** | 1 | 470uf | Capacitor_THT:CP_Radial_D8.0mm 25V Electrolytic | [Buy Link](https://robu.in/product/470uf-25v-electrolytic-capacitor-pack-of-3/) |
| **C3** | 1 | 100uf | Capacitor_THT:CP_Radial_D8.0mm 25V Electrolytic | [Buy Link](https://robu.in/?s=100uf+25v+radial+electrolyte+capacitor&post_type=product) |
| **C2, C4-C12, C15** | 11 | 100n | Capacitor_THT:C_Disc 0.1uF Ceramic Disc | [Buy Link](https://robu.in/?s=104+0.1uf+ceramic+disc+capacitor&post_type=product) |
| **C13, C14** | 2 | 22pf | Capacitor_THT:C_Disc 22pF Ceramic Disc | [Buy Link](https://robu.in/?s=22pf+ceramic+disc+capacitor&post_type=product) |
| **D2 - D5** | 4 | LED | LED_THT:LED_D5.0mm Red Status Indicator | [Buy Link](https://robu.in/?s=5mm+red+led+pack&post_type=product) |
| **R1-R7, R9-R15, R17-R23, R26-R32** | 28 | 390R | Resistor_THT:R_Axial 1/4W Carbon Film | (https://robu.in/?s=390+ohm+quarter+watt+resistor&post_type=product) |
| **R8, R16, R24, R33, R35-R50** | 20 | 620R | Resistor_THT:R_Axial 1/4W Carbon Film | (https://robu.in/?s=620+ohm+quarter+watt+resistor&post_type=product) |
| **R51, R55** | 2 | 1k | Resistor_THT:R_Axial 1/4W Carbon Film | (https://robu.in/?s=1k+ohm+quarter+watt+resistor&post_type=product) |
| **R52** | 1 | 270R | Resistor_THT:R_Axial 1/4W Carbon Film | (https://robu.in/?s=270+ohm+quarter+watt+resistor&post_type=product) |
| **R53, R54** | 2 | 10k | Resistor_THT:R_Axial 1/4W Carbon Film | (https://robu.in/?s=10k+ohm+quarter+watt+resistor&post_type=product) |
| **J1, J4** | 2 | Male Pins | 2.54mm Breakaway Vertical Headers | [Buy Link](https://www.digikey.in/en/products/detail/amphenol-cs-fci/68000-402HLF/1493940?s=N4IgTCBcDaIGwA4AMKC0AWJYASAZAYiALoC%2BQA and https://www.digikey.in/en/products/detail/amphenol-cs-fci/68000-406HLF/1878471?s=N4IgTCBcDaIGwA4AMKC0AWJcASAZAYiALoC%2BQA ) |
| **J2, J3** | 2 | Sockets | 2.54mm Vertical Female Pin Sockets | [Buy Link](https://www.digikey.in/en/products/detail/3m/929974-01-04-RK/1094257 and https://www.digikey.in/en/products/detail/3m/929974-01-06-RK/1094259) |
| **Case Hardware** | 6 | Magnets | N52 Neodymium Disc Magnets (3mm x 2mm) | [Buy Link](https://www.amazon.in/dp/B0BN8PHN9B) |
| **Case Hardware** | 1 | Glass Sheet | Custom cut clear front panel window (2mm) |  |




```




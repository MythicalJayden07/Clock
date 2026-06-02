[ClockBOM.csv](https://github.com/user-attachments/files/28500934/ClockBOM.csv)# Clock

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
[Uploading Clock"Reference","Qty","Value","DNP","Exclude from BOM","Exclude from Board","Footprint","Datasheet","Check_prices","Price"
"C1","1","470uf","","","","Capacitor_THT:CP_Radial_D8.0mm_P3.50mm","","",""
"C2,C4,C5,C6,C7,C8,C9,C10,C11,C12,C15","11","100n","","","","Capacitor_THT:C_Disc_D5.0mm_W2.5mm_P5.00mm","","",""
"C3","1","100uf","","","","Capacitor_THT:CP_Radial_D8.0mm_P3.50mm","","",""
"C13,C14","2","22pf","","","","Capacitor_THT:C_Disc_D5.0mm_W2.5mm_P5.00mm","","",""
"D1","1","1N5401","","","","Diode_THT:D_DO-201AD_P15.24mm_Horizontal","http://www.vishay.com/docs/88516/1n5400.pdf","",""
"D2,D3,D4,D5","4","LED","","","","LED_THT:LED_D5.0mm","","",""
"DS1,DS2,DS3,DS4","4","SA18-11EWA","","","","Sa18:My_Big_SA18_Display","https://componentsearchengine.com/Datasheets/2/SA18-11EWA.pdf","",""
"DS5,DS6","2","SA08-11GWA","","","","Clock parts:My_Custom_SA08_Display","https://www.kingbrightusa.com/images/catalog/spec/SA08-11GWA.pdf","",""
"F1","1","2A","","","","Fuse:Fuse_Bourns_MF-RG300","","",""
"J1","1","Conn_01x02","","","","Connector_PinHeader_2.54mm:PinHeader_1x02_P2.54mm_Vertical","","",""
"J2","1","Conn_01x04_Socket","","","","Connector_PinSocket_2.54mm:PinSocket_1x04_P2.54mm_Vertical","","",""
"J3","1","Conn_01x06_Socket","","","","Connector_PinSocket_2.54mm:PinSocket_1x06_P2.54mm_Vertical","","",""
"J4","1","Conn_01x06_Pin","","","","Connector_PinHeader_2.54mm:PinHeader_1x06_P2.54mm_Vertical","","",""
"Q1","1","2N3904","","","","Package_TO_SOT_THT:TO-92_Inline","https://www.onsemi.com/pub/Collateral/2N3903-D.PDF","",""
"R1,R2,R3,R4,R5,R6,R7,R9,R10,R11,R12,R13,R14,R15,R17,R18,R19,R20,R21,R22,R23,R26,R27,R28,R29,R30,R31,R32","28","390R","","","","Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal","","",""
"R8,R16,R24,R33,R35,R36,R37,R38,R39,R40,R41,R42,R43,R44,R45,R46,R47,R48,R49,R50","20","620R","","","","Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal","","",""
"R51,R55","2","1k","","","","Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal","","",""
"R52","1","270R","","","","Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal","","",""
"R53,R54","2","10k","","","","Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal","","",""
"U1","1","ATmega328P-P","","","","Package_DIP:DIP-28_W7.62mm","http://ww1.microchip.com/downloads/en/DeviceDoc/ATmega328_P%20AVR%20MCU%20with%20picoPower%20Technology%20Data%20Sheet%2040001984A.pdf","",""
"U2,U3,U4,U5,U6,U7","6","TPIC6B595","","","","Package_DIP:DIP-20_W7.62mm","","https://www.snapeda.com/parts/TPIC6B595/Texas+Instruments/view-part/?ref=eda","None"
"U8","1","L7805","","","","Package_TO_SOT_THT:TO-220-3_Vertical","http://www.st.com/content/ccc/resource/technical/document/datasheet/41/4f/b3/b0/12/d4/47/88/CD00000444.pdf/files/CD00000444.pdf/jcr:content/translations/en.CD00000444.pdf","",""
"Y1","1","16Mhz","","","","Crystal:Crystal_HC49-U_Vertical","","",""
BOM.csv…]()


| Reference | Qty | Value | Footprint | Part Link |
| :--- | :--- | :--- | :--- | :--- |
| C1, C3 | 2 | 470uf / 100uf | Capacitor_THT:CP_Radial_D8.0mm_P3.50mm | [Mouser India](https://www.mouser.in/c/passive-components/capacitors/aluminum-electrolytic-capacitors/aluminum-electrolytic-capacitors-leaded/) |
| C2, C4, C5, C6, C7, C8, C9, C10, C11, C12, C15 | 11 | 100n | Capacitor_THT:C_Disc_D5.0mm_W2.5mm_P5.00mm | [DigiKey India](https://www.digikey.in/en/products/filter/ceramic-capacitors/60) |
| C13, C14 | 2 | 22pf | Capacitor_THT:C_Disc_D5.0mm_W2.5mm_P5.00mm | [DigiKey India](https://www.digikey.in/en/products/filter/ceramic-capacitors/60) |
| D1 | 1 | 1N5401 | Diode_THT:D_DO-201AD_P15.24mm_Horizontal | [Mouser India](https://www.mouser.in/ProductDetail/Vishay-General-Semiconductor/1N5401-E3-54?qs=AQlKX63v8RvNeuYg%252B06wMw%3D%3D) |
| D2, D3, D4, D5 | 4 | LED | LED_THT:LED_D5.0mm | [DigiKey India](https://www.digikey.in/en/products/filter/led-indication-discrete/105) |
| DS1, DS2, DS3, DS4 | 4 | SA18-11EWA | Sa18:My_Big_SA18_Display | [Mouser India](https://www.mouser.in/ProductDetail/Kingbright/SA18-11EWA?qs=JpELLRhtMc01ud%252BhiiNcbQ%3D%3D) |
| DS5, DS6 | 2 | SA08-11GWA | Clock parts:My_Custom_SA08_Display | [Mouser India](https://www.mouser.in/ProductDetail/Kingbright/SA08-11GWA?qs=E09Sz5t5voVFPaAyTwzbvg%3D%3D) |
| F1 | 1 | 2A | Fuse:Fuse_Bourns_MF-RG300 | [Mouser India](https://www.mouser.in/ProductDetail/Bourns/MF-RG300-0?qs=Zco4Fs67ctclSu06fHwNtw%3D%3D) |
| J1 | 1 | Conn_01x02 | Connector_PinHeader_2.54mm:PinHeader_1x02_P2.54mm_Vertical | [DigiKey India](https://www.digikey.in/en/products/filter/rectilinear-connectors-headers-male-pins/314) |
| J2 | 1 | Conn_01x04_Socket | Connector_PinSocket_2.54mm:PinSocket_1x04_P2.54mm_Vertical | [DigiKey India](https://www.digikey.in/en/products/filter/rectilinear-connectors-headers-receptacles-female-sockets/315) |
| J3 | 1 | Conn_01x06_Socket | Connector_PinSocket_2.54mm:PinSocket_1x06_P2.54mm_Vertical | [DigiKey India](https://www.digikey.in/en/products/filter/rectilinear-connectors-headers-receptacles-female-sockets/315) |
| J4 | 1 | Conn_01x06_Pin | Connector_PinHeader_2.54mm:PinHeader_1x06_P2.54mm_Vertical | [DigiKey India](https://www.digikey.in/en/products/filter/rectilinear-connectors-headers-male-pins/314) |
| Q1 | 1 | 2N3904 | Package_TO_SOT_THT:TO-92_Inline | [Mouser India](https://www.mouser.in/ProductDetail/onsemi/2N3904BU?qs=vX9vO70wSnuv0jYvI7Oweg%3D%3D) |
| R1-R7, R9-R15, R17-R23, R26-R32 | 28 | 390R | Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal | [Mouser India](https://www.mouser.in/c/passive-components/resistors/through-hole-resistors/?q=390%20ohm) |
| R8, R16, R24, R33, R35-R50 | 20 | 620R | Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal | [Mouser India](https://www.mouser.in/c/passive-components/resistors/through-hole-resistors/?q=620%20ohm) |
| R51, R55 | 2 | 1k | Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal | [Mouser India](https://www.mouser.in/c/passive-components/resistors/through-hole-resistors/?q=1k%20ohm) |
| R52 | 1 | 270R | Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal | [Mouser India](https://www.mouser.in/c/passive-components/resistors/through-hole-resistors/?q=270%20ohm) |
| R53, R54 | 2 | 10k | Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal | [Mouser India](https://www.mouser.in/c/passive-components/resistors/through-hole-resistors/?q=10k%20ohm) |
| U1 | 1 | ATmega328P-P | Package_DIP:DIP-28_W7.62mm | [IndiaMART Local](https://www.indiamart.com/proddetail/atmega328p-pu-microcontroller-ic-22352406397.html) / [Mouser](https://www.mouser.in/ProductDetail/Microchip-Technology/ATMEGA328P-PU?qs=9%252BKC7Al7BCpOnw089%252BX7wA%3D%3D) |
| U2, U3, U4, U5, U6, U7 | 6 | TPIC6B595 | Package_DIP:DIP-20_W7.62mm | [Mouser India](https://www.mouser.in/ProductDetail/Texas-Instruments/TPIC6B595N?qs=o3O7b%2F16kXp%2Fd9063WbX1w%3D%3D) |
| U8 | 1 | L7805 | Package_TO_SOT_THT:TO-220-3_Vertical | [Mouser India](https://www.mouser.in/ProductDetail/STMicroelectronics/L7805CV?qs=b7gC7679OOnSbhX93R2Wgw%3D%3D) |
| Y1 | 1 | 16Mhz | Crystal:Crystal_HC49-U_Vertical | [Mouser India](https://www.mouser.in/c/?q=16MHz%20crystal%20HC49-U) |
| Enclosure Hardware | 1 | Glass Sheet | Custom cut front panel face (2mm) | [Local Hardware/Glass Cutter]() |
| Enclosure Hardware | 4 | Neodymium Magnets | Tiny N52 disc magnets for door latches | [Amazon India](https://www.amazon.in/s?k=N52+neodymium+magnets+disc) |

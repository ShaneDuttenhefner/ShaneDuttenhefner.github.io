---
title: Component Selection
---

## Major Components
### OLED Display

**Solution** | **Pros** | **Cons**
-------------|----------|----------
![image](https://github.com/user-attachments/assets/23f383de-fb10-4f5c-bf63-eac755a74c98) <br> Option 1: NHD-C12832A1Z-FSW-FBW-3V3 <br> $12.78/each <br> [Link to product](https://www.digikey.com/en/products/detail/newhaven-display-intl/NHD-C12832A1Z-FSW-FBW-3V3/2059236)| -128x32 pixels <br> -36.00mm W x 12.00mm H screen <br> -White background with black text | -Smaller screen <br> -Smaller pixel count <br> -SPI <br> -Expensive
![image](https://github.com/user-attachments/assets/c4d26d8e-07fe-49e2-87f0-afc1fec357c6) <br> Option 2: NHD-C12832A1Z-NSW-BBW-3V3 <br> $12.82/each <br> [Link to product](https://www.digikey.com/en/products/detail/newhaven-display-intl/NHD-C12832A1Z-NSW-BBW-3V3/2059235) | -128x32 pixels <br> -36.00mm W x 12.00mm H screen <br> -Blue background with white text | -Smaller screen <br> -Smaller pixel count <br> -SPI <br> -Expensive
![image](https://github.com/user-attachments/assets/57250bf9-9072-4890-998a-d39ecc9d3044) <br> Option 3: NHD-C12864GG-RN-GBW <br> $13.32/each <br> [Link to product](https://www.digikey.com/en/products/detail/newhaven-display-intl/NHD-C12864GG-RN-GBW/1701323) | -128x60 pixels <br> -49.53mm W x 26.67mm H screen (Largest) <br> - I2C| -Grey background with black text <br> -Most expensive <br> -Parallel, 8-bit communication 
![image](https://github.com/user-attachments/assets/64518cf7-5174-46cd-ad9c-1c1793bce1c5) <br> Option 4: B085WCRS7C <br> $13.99/five <br> [Link to Product](https://www.amazon.com/Songhe-0-96-inch-I2C-Raspberry/dp/B085WCRS7C/) | -128x64 pixels <br>  -27mm x 27mm x 2 mm screen <br> -Less pins <br> -I2C | - Smaller screen <br> - White text on black background


**Choice:** Option 4: B085WCRS7C Display

**Rationale**: Option 4 will be the best to work with for this exhibit. The white text and black background may not be the best on the user’s eyes, but it should be one of the easiest to read off of. The screen and pixel count is large enough to get the level of detail we plan for our exhibit game. It uses an I2C interface which is the ideal choice for communication, only has four pins so harwiring it will be easier, and it is the cheapest option.


### 3.3V Regulator

**Solution** | **Pros** | **Cons**
-------------|----------|----------
![image](https://github.com/user-attachments/assets/714db880-d126-4c3a-bf43-cb2934ffc1db) <br> Option 1: TPS62172DSGR <br> $1.17/each <br> [Link to Product](https://www.digikey.com/en/products/detail/texas-instruments/TPS62172DSGR/2833456) | -3.3V and 500mA <br> -Simple circuit(No diodes required. Only inductor) <br> -Fixed Voltage output | - Extremely Small (1.9mm x 1.9mm) <br> -Eight pins make it harder to surface mount with the size
![image](https://github.com/user-attachments/assets/9386be08-d2ce-4632-9fd6-6180727e721f) <br> Option 2: LM2575T-3.3G <br> $2.99/each <br> [Link to Product](https://www.digikey.com/en/products/detail/onsemi/LM2575T-3-3G/1476700) | -Fixed 3.3V ouput <br> -1A output current <br> -Familiarity | -Through hole <br> -Requires more components such as diodes

**Choice** Option 1: TPS62172DSGR

**Rationale** Option 1 will be able to properly power the reest of the subsytems of the board as everything requires only 3.3V and a current of 500mA will supply everything just fine. The small size of it make prove difficult to solder, however that and its simple circuit will leave plenty of space open on the PCB for the other components.

### Summary of Components Selection

**Component** | **Pros** | **Cons**
-------------|----------|----------
![image](https://github.com/user-attachments/assets/64518cf7-5174-46cd-ad9c-1c1793bce1c5) <br> Option 4: B085WCRS7C <br> $13.99/five <br> [Link to Product](https://www.amazon.com/Songhe-0-96-inch-I2C-Raspberry/dp/B085WCRS7C/) | -128x64 pixels <br>  -27mm x 27mm x 2 mm screen <br> -Less pins <br> -I2C | - Smaller screen <br> - White text on black background
![image](https://github.com/user-attachments/assets/714db880-d126-4c3a-bf43-cb2934ffc1db) <br> Option 1: TPS62172DSGR <br> $1.17/each <br> [Link to Product](https://www.digikey.com/en/products/detail/texas-instruments/TPS62172DSGR/2833456) | -3.3V and 500mA <br> -Simple circuit(No diodes required. Only inductor) <br> -Fixed Voltage output | - Extremely Small (1.9mm x 1.9mm) <br> -Eight pins make it harder to surface mount with the size


## Micro Controller

### PIC Table
**PIC Info** | **Answer** 
-------------|-----------
Model | PIC18F47Q10-I/PT
Product Page URL | ![Link to product](https://www.microchip.com/en-us/product/PIC18F47Q10)
Datasheet URL | ![Link to product](https://ww1.microchip.com/downloads/en/DeviceDoc/PIC18F27-47Q10-Data-Sheet-40002043E.pdf)
Application Notes URL(s) | ![Link to product](https://www.microchip.com/en-us/product/PIC18F47Q10)
Vendor link | ![Link to product](https://www.digikey.com/en/products/detail/microchip-technology/PIC18F47Q10-I-PT/10187786)
Code Examples | TBD
External Resources URL(s) | TBD
Unit cost | $1.65
Absolute Maximum Current for entire IC | 350 mA
Supply Voltage Range | 1.8V to 5.5V
Maximum GPIO current(per pin) | 50mA
Supports External Interrupts? | Yes
Required Programming Hardware, Cost, URL | ![Link to product](https://www.microchip.com/en-us/development-tool/pg164100)
Works with MPLabX? | Yes
Works with Microchip Code Configurator? | Yes

**Role:** My role on the team is to program a display for the game of our exhibit. I will be responsible for the circuit board for an OLED display, with additional LEDs, that will provide the user with instructions for our game. The OLED will also receive data from the other boards of my team members to display the data they are recording and update the user on what they need to do to win as the game progresses.

### MPLab X Configuration

![image](https://github.com/user-attachments/assets/a50d2cd0-697b-4ce6-beb9-be1397f0112a)


### Choice and Rationale

For this project I have chosen the MICROCHIP PIC18F47Q10-I/PT because it is reliable, familiar, and satisfies all the requirements that a microcontroller needs for this project. This PIC supports I2C communication which is exactly what I need to communicate with my chosen OLED Display. UART is also available with this microcontroller which allows for my board to receive and send data from my teammate’s. In addition, the PIC had plenty of I/O pins for additional components such as debugging LEDs which I can use, along with PWM, to create indicator lights for the user as they play the game.


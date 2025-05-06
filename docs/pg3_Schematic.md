---
title: Schematic/PCB/BoM
---
##Schematic
![image](https://github.com/user-attachments/assets/c0701d0b-80d2-4ef5-8127-c38f42aca25f)


[Link to PDF of Schematic](https://github.com/user-attachments/files/20053123/Duttenhefner_Individual_Schematic_Design_2.pdf)

[Link to Cadence Zip File](https://github.com/user-attachments/files/20053138/Duttenhefner_Individual_Schematic.zip)

The schematic above show the simple circuitry required to control and OLED display using a PIC microcontroller powered by 3.3V. The power regulator is able to take in a range of voltages, in this case 12, and output the proper 3.3 volts required to power the rest of the board. A switch is used in the circuit to allow the board to take power from either a barrel jack or from the daisy chain headers. A five pin header is used here to connect to the microcontroller's Masterclear and program pins for re-programming it. The micro controller in this schematic is wired to all of the OLED's SPI pins along with pull-down resistors which allow for communication and control over this subsytem. With the OLED properly connected, we are able tp create the visual element needed for the game. The three LEDs are also connected to the PIC with current limiting resistors. With this, the LEDs can be used to debug the code and then later be used as additional visual elements for the game. The PIC is able to read through Rx and send messages throug Tx via the connections to the eight pin headers for the daisy chain.

## PCB
### Front
![image](https://github.com/user-attachments/assets/e5d4a562-118d-424c-9431-4cf6b415dcf4)

### Back
![image](https://github.com/user-attachments/assets/11014e46-cf6f-41b2-bea6-05dd10164aab)

[Link to Gerber Zip File](https://github.com/user-attachments/files/20053429/ShaneDuttenhefner_302.zip)




## Bill of Materials
![image](https://github.com/user-attachments/assets/4cbbdf10-de8d-458f-a1de-ea301fe021ee)
[Link to PDF of BoM](https://github.com/user-attachments/files/20053341/Duttenhefner_314_BoM.pdf)

## Purchase Request Form:
### Request Form 1
![image](https://github.com/user-attachments/assets/261b9f24-dbde-4085-9d30-e8c879b74f80)

[PDF of Purchase Request Form 1](https://github.com/user-attachments/files/19044818/Duttenhefner_EGR-314-Purchase-Request-2025_DIGI-KEY.pdf)

## Request Form 2
![image](https://github.com/user-attachments/assets/c40a6fb2-4211-4a00-ac0d-c6721ad36809)

[PDF of Purchase Request Form 2](https://github.com/user-attachments/files/20053358/Duttenhefner_314_BoM.pdf)




##Power Budget

![image](https://github.com/user-attachments/assets/c0b12ffb-e191-4eec-aa4f-1b222106c010)



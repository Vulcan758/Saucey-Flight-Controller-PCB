# Saucey-Flight-Controller-PCB
This is a design repository for an ESP32 based flight controller (FC), "Saucey", that I made. 


![Screenshot from 2024-10-21 20-56-30](https://github.com/user-attachments/assets/f89a6778-a77d-4090-91f1-0a533f3f61ec)

## Technical Specifications
The FC uses an ESP32 S3 WROOM 1 module as the micrcontroller (MCU). It contains a 3.3 volt linear regulator (AMS1117 was used here) to power the MCU and the inertial measurement unit (IMU). The IMU used here is a MPU6050. This board is to be programmed through USB C. There is no onboard USB-Serial converter chip (such as CH2102) as ESP32 S3 can be programmed directly with its built USB-Serial converter on pins 18 and 19. A status LED is also availiable on board for testing and debugging. The FC board has 4 half bridge SI2306 logic level MOSFETs meant to drive coreless motors via JST connectors. This can however drive/ignite model rocket motors, LEDs and other low voltage output devices.

The goal of this project was to design a smart flight controller board with a credit card size form factor.

## PCB Schematic

![0db240ba_1](https://github.com/user-attachments/assets/151f8761-880f-4179-ab0c-047402e5c54c)


## PCB Layout

![Screenshot from 2024-10-22 01-10-28](https://github.com/user-attachments/assets/2e6ad8a5-7c12-44a7-ad89-3843deb2944c)

### Top Layer

With ground pour

![Screenshot from 2024-10-22 01-11-43](https://github.com/user-attachments/assets/bbe8179c-3f9e-44dd-81ed-4fa8ff9ae25d)

Without ground pour

![Screenshot from 2024-10-22 01-11-12](https://github.com/user-attachments/assets/2bf73304-44e5-4904-b02f-186e4f51650a)

### Bottom Layer

With ground pour

![Screenshot from 2024-10-22 01-11-51](https://github.com/user-attachments/assets/4094051c-3261-4401-9715-a6846a6328de)

Without ground pour

![Screenshot from 2024-10-22 01-11-23](https://github.com/user-attachments/assets/74e1dd20-0868-438e-bc13-f01d71359af0)


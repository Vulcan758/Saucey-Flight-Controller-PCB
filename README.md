# Saucey-Flight-Controller-PCB
This is a design repository for an ESP32 based flight controller (FC), "Saucey", that I made. 


![Screenshot from 2024-10-21 20-56-30](https://github.com/user-attachments/assets/f89a6778-a77d-4090-91f1-0a533f3f61ec)

## Technical Specifications
The FC uses an ESP32 S3 WROOM 1 module as the micrcontroller (MCU). It contains a 3.3 volt linear regulator (AMS1117 was used here) to power the MCU and the inertial measurement unit (IMU). The IMU used here is a MPU6050. This board is to be programmed through USB C. There is no onboard USB-Serial converter chip (such as CH2102) as ESP32 S3 can be programmed directly with its built USB-Serial converter on pins 18 and 19. A status LED is also availiable on board for testing and debugging. The FC board has 4 half bridge SI2306 logic level MOSFETs meant to drive coreless motors via JST connectors. This can however drive/ignite model rocket motors, LEDs and other low voltage output devices.

The goal of this project was to design a smart flight controller board with a credit card size form factor.

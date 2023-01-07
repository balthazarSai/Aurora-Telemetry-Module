# Aurora Telemetry Module
After a lot of hard work, I have created my first prototype telemetry module for model rocketry. In this repository you can find all the kicad files, the gerber files as well as the BOM that I used to produce this.

## Technical Specifications
The AURORA V1 Telemetry module has the following sensors and specifications:
```
- DIMENSIONS        : 50mm x 50mm (without antenna assembly)
- MPU               : STM32F446RET6
- HSE               : 16MHz
- Sensors:
    > IMU           : BMI270
    > ALTIMETER     : MPL3115A2
    > BAROMETER     : MPL3115A2
    > TEMPERATURE   : MPL3115A2 & HDC1080
    > HUMIDITY      : HDC1080
    > MAGNETOMETER  : LIS3MDL
    > ACCELEROMETER : H3LIS200DLTR
    > GYROSCOPE     : I3G4250DTR
- Connectivity: 
    > USB C
    > MOLEX 2 PIN BATTERY CONNECTOR
    > TC2030-NL SWD 
- Storage:
    > On board MicroSD
    > 125Mbit NAND Flash
- Radio             : RFM96W-433S2 (433MHz)

OPERATING VOLTAGE   : 3.3v
MAXIMUM Vinput      : 24v
OPERATING CURRENT   : 650mA
FUSE SUSTAINED      : 750mA
FUSE BLOW(1s)       : 1.2A
```

<img src="https://github.com/balthazarSai/Aurora-Telemetry-Module/blob/main/Manufacturing/AURORAV1.jpg" width="600">

##  Software
I am currently working on the software implementation for this module, I will be updating this repo as I go and pushing finalised code as I go.
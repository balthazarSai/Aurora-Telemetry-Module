# Aurora Telemetry Module
The Aurora V1 is an experimental telemetry module for model rockets. I designed it after deciding that I wanted to experiment with different algorithms for analysing the telemetry data from a rocket to create an active control model. At its current stage the module is capable of logging a variety of data and transmitting back to the ground station (apporximate range depending on settings but can theoretically do 20km+ line of sight). The module also has redundant on board memory storage in case of transmission failures by using a microSD card as well as a NAND Flash chip more than capable of holding the generated data for about 1-2hrs of operation without clearing (estimated values more detailed ones will be added after software review).

## Pipeline
Here is an estimated pipeline of when I plan to release/work on the next versions of the PCB and the functionality I want to add on each version update. I will be updating this table based on my progress.

| Version       | Functionality | Status        |
| ------------- |:-------------:|:-------------:|
| AURORA V1     | Telemetry     |  **Released**     |
| AURORA V2     | V1 + GPS      |  Planned Q3 2023|
| AURORA V3     | V2 + Recovery |      -        |

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

## Manufacturing
I used JLCPCB to produce the protoype version of this board, the Bill of Materials provided has some of the vendor codes provided based on their availability at the time of ordering.

##  Software
I am currently working on the software implementation for this module, I will be updating this repo as I go and pushing finalised code as I go.
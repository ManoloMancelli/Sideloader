# Sideloader 1.5.1

![1](docs/img/Sideloader.png)

SteamVR Firmware based off of excellent [HadesVR](https://github.com/HadesVR/HadesVR)

# Custom Hardware Version - Gyro Side
![1](docs/img/custom_hardware_version.JPG)

## Wiring the IMU and MCU
The IMU needs to be connected to the MCU for power and communication.
The MCU connects to your computer via USB to send the IMU readings to SteamVR.

In case of an Arduino Pro Micro, you need to connect the following pins:
```
Pro Micro       IMU
VCC         ->  VCC  
GND         ->  GND  
SDA(pin 2)  ->  SDA  
SCL(pin 3)  ->  SCL  
```

### 1.4.2 Programming your MCU

As previously mentioned, we recommend you use an Arduino Pro Micro and an IMU supported by the FastIMU Library.
FastIMU is an awesome package that supports many commonly used IMUs and comes with a pre-written Arduino sketch that works with Relativty.

First, you will need to install the Arduino IDE and connect your MCU to your computer via the USB connector.

Once you have it connected and verified your Arduino IDE can work with your MCU, download FastIMU from the library manager.

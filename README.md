# Bluepill-MPU6050

Firmware of Blue Pill (STM32F103C8) communication with MPU6050 accelerometer. Developed with STM32CubeIDE.

## First step: wire up
Getting MPU6050 gyro and accelerometer data via I2C protocol. Data visualization via Serial.

### I2C
```
- SDA: PB9
- SCL: PB8
```
### Serial
```
- RX: PB7
- TX: PB6
- Baud Rate: 115200
```

## Second step: CubeMX configuration :wrench:
STM32CubeIDE project starts with basic settings:

### CubeMX: Pinout & Configuration 
```
- SYS: Debug -> Serial Wire
- RCC: HSE -> Crystal/Ceramic
```

### CubeMX: Clock Configuration
```
- PLL Source Mux: HSE
- *PLLMul: x9
- System Clock Mux: PLLCLK
- APB1 Prescaler: /2
```

## Reference
- [MPU-6000 and MPU-6050 Register Map and Descriptions Revision 4.0](https://cdn.sparkfun.com/datasheets/Sensors/Accelerometers/RM-MPU-6000A.pdf)
- [Getting Started With STM32 and Nucleo Part 2: How to Use I2C to Read Temperature Sensor TMP102](https://youtu.be/isOekyygpR8)
- [How to interface mpu6050 gy 521 with stm32](https://controllerstech.com/how-to-interface-mpu6050-gy-521-with-stm32/)
![bluepill](https://os.mbed.com/media/uploads/hudakz/stm32f103c8t6_pinout_voltage01.png)

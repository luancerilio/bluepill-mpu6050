# Bluepill-MPU6050

Firmware of Blue Pill board (STM32F103C8) communication with MPU6050 accelerometer. Developed with STM32CubeIDE.

#### Basic Configuration :wrench:
Project starts with basic settings:

##### CubeMX: Pinout & Configuration 
```
- SYS: Debug -> Serial Wire
- RCC: HSE -> Crystal/Ceramic
```

##### CubeMX: Clock Configuration
```
- PLL Source Mux: HSE
- *PLLMul: x9
- System Clock Mux: PLLCLK
- APB1 Prescaler: /2
```

## Reference: Blue Pill pinout

![bluepill](https://os.mbed.com/media/uploads/hudakz/stm32f103c8t6_pinout_voltage01.png)

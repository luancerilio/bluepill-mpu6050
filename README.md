# STM32-CubeIDE

A bunch of applications developed with Blue Pill board (STM32F103C8) and CubeIDE (STMicroelectronics), using HAL.

#### Basic Configurations :wrench:
Every project starts with basic settings like:

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

## Blue Pill pinout

![bluepill](https://os.mbed.com/media/uploads/hudakz/stm32f103c8t6_pinout_voltage01.png)
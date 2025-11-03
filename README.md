# stm32f405rgt6-Simple-Test-Board

## Architecture

<img src="image.png" alt="Architecture" width="400"/>

## Design

For this simple test board, the pins and peripherals that will be used are:
- Serial Wire Debug
- High Speed External Crystal Oscillator
- USB Differential Pair
- I2C
- UART

<img src="mcu-pin-layout.png" alt="Architecture" width="600"/>


| Subsystem     | Component               |
| ------------- | ----------------------- |
| MCU           | STM32F405RGT6           |
| Power         | MP2359DJ                |
| USB           | USB Type C              |
| Debug         | SWD (Serial Wire Debug) |
| Clock         | 8 MHz Crystal           |
| Communication | I2C, UART               |


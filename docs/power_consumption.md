# Power Consumption

![alt text](image.png)



From datasheet Table 20 and Figure 24:
- Run mode
- 168 MHz
- TA = 25 °C
- Peripherals disabled

Icore = 40 mA (approx)

From datasheet Table 28.

Rates:
- AHB1, GPIOA = 2.70 uA/MHz 
- AHB1, GPIOB = 2.50 uA/MHz
Currents:
- I_GPIOA = 2.70 uA/MHz * 168 MHz = 0.453 mA (approx)
- I_GPIOB = 2.50 uA/MHz * 168 MHz = 0.420 mA
- I_AHB1 = I_GPIOA + I_GPIOB = 0.873 mA (approx)
 
Rates:
- AHB2, USB OTG_FS = 26.45 uA/MHz
Currents:
- I_USB_OTG_FS = 26.45 uA/MHz * 168 MHz = 4.444 mA (approx)
- I_AHB2 = I_USB_OTG_FS = 4.444 mA

Rates:
- APB1, USART3 = 2.74 uA/MHz
- APB1, I2C1 = 2.67 uA/MHz
Currents:
- I_USART3 = 2.74 uA/MHz * 42 MHz = 0.115 mA (approx)
- I_I2C1 = 2.67 uA/MHZ * 42 MHz = 0.112 mA (approx)
- I_APB1 = I_USART3 + I_I2C1 = 0.227

Total core and peripherals:
I_total = 0.873 + 4.444 + 0.227 = 5.54 mA




References:
- Table 20. Typical and maximum current consumption in Run mode, code with data processing  running from flash memory (ART accelerator enabled) or RAM
- Figure 24. Typical current consumption versus temperature, Run mode, code with data processing running from Flash (ART accelerator ON) or RAM, and peripherals OFF
- Table 28. Peripheral current consumption
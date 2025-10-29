# PWM Generation and Input Capture on B-L475E-IOT01A1


## Overview

- **PWM Output:**  
  - **Timer:** TIM2 Channel 1  
  - **Pin:** Port D13 (GPIOA_PIN_5)  
  - Generates a PWM waveform with a configurable frequency and duty cycle via user button.

- **Input Capture:**  
  - **Timer:** TIM2 Channel 4  
  - **Pin:** Port D4 (GPIOA_PIN_3)  
  - Measures the PWM signal’s frequency and duty cycle using input capture interrupts.

The captured results are printed via **USART1** using `HAL_UART_Transmit()`.

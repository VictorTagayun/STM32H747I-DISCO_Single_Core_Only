# STM32H747I Single Core Only

## Introduction and Purpose

** How to disable 
** STM32H747I is a Dual core Cortex-M7 and Cortex-M4 MCU.  
** The STM32H747I-DISCO Discovery kit is a complete demonstration and development platform for STMicroelectronics STM32H747XIH6 microcontroller, designed to simplify user application development.   
** Use CubeMX to init all peripherals  


## Setup GPIO and BOOT Sequence 

Reset all pins and setup the GPIOs on LED   
In main.c of M7, comment out all the codes under Boot_Mode_Sequence_1 and Boot_Mode_Sequence_2  

That's it! M4 will be in sleep mode!

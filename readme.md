# STM32H747I Single Core Only

## Introduction and Purpose

** How to disable STM32H747I M4 core and run ony M7 core.   
** STM32H747I is a Dual core Cortex-M7 and Cortex-M4 MCU.  
** The STM32H747I-DISCO Discovery kit is a complete demonstration and development platform for STMicroelectronics STM32H747XIH6 microcontroller, designed to simplify user application development.   
** Use CubeMX to init all peripherals  


## Setup GPIO and BOOT Sequence 

Reset all pins and setup the GPIOs on LED   
In main.c of M7, comment out all the codes under Boot_Mode_Sequence_1 and Boot_Mode_Sequence_2  

https://github.com/VictorTagayun/STM32H747I-DISCO_Single_Core_Only/blob/694da5be8427cd47b99b376b3ea9ae12e60b4f18/STM32H747I-DISCO_SingleCore/CM7/Core/Src/main.c#L83
https://github.com/VictorTagayun/STM32H747I-DISCO_Single_Core_Only/blob/694da5be8427cd47b99b376b3ea9ae12e60b4f18/STM32H747I-DISCO_SingleCore/CM7/Core/Src/main.c#L103


That's it! M4 will be in sleep mode!

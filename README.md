# NFC
This directory contains a set of source files that implement a simple example based on 
ST25R3916

@note Care must be taken when using HAL_Delay(), this function provides accurate delay (in milliseconds)
      based on variable incremented in SysTick ISR. This implies that if HAL_Delay() is called from
      a peripheral ISR process, then the SysTick interrupt must have higher priority (numerically lower)
      than the peripheral interrupt. Otherwise the caller ISR process will be blocked.
      To change the SysTick interrupt priority you have to use HAL_NVIC_SetPriority() function.



@par Hardware and Software environment  

  - This example runs on STM32L476RG and STM32L03R8 devices.
    
  - This application has been tested with STMicroelectronics:
    STM32L4xx-Nucleo RevC
    STM32L0xx-Nucleo RevC
    boards and can be easily tailored to any other supported device 
    and development board.

  - STM32LXxx-Nucleo, STM32L0xx-Nucleo RevC Set-up    
    - Connect the Nucleo board to your PC with a USB cable type A to mini-B 
      to ST-LINK connector (CN1).
    - Please ensure that the ST-LINK connector CN2 jumpers are fitted.


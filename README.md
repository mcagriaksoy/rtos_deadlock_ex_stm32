# rtos_deadlock_ex_stm32
A classic restaurant deadlock example and solution on STM32 Nucleo G4 series board using FreeRTOS

 * This code block demonstrates a classic restaurant deadlock example and solution on STM32 Nucleo G4 series board using FreeRTOS.
 * The restaurant has four customers and four chopsticks, and each customer needs two chopsticks to eat.
 * The customers are represented by tasks, and the chopsticks are represented by mutexes.
 * The code uses the xSemaphoreTake and xSemaphoreGive functions to acquire and release the chopsticks.
 * The code also uses the vTaskDelay function to simulate the eating and thinking time of the customers.
 * The code avoids deadlock by using a priority inheritance protocol, which allows a lower priority task to inherit the priority of a higher priority task that is waiting for the same resource.
 * The code also uses the configUSE_MUTEXES and configUSE_INHERITED_PRIORITY macros to enable the priority inheritance feature in FreeRTOS.
 * The code is based on the GitHub repository [mcagriaksoy/rtos_deadlock_ex_stm32](https://github.com/mcagriaksoy/rtos_deadlock_ex_stm32), which provides more details and instructions on how to run the code on the STM32 Nucleo G4 board.

Platform Project
================

The 'Platform' project configures the hardware of the evaluation board
and is a CMSIS-RTOS2 based software template that can be further expanded.

This implementation contains the following configured interface drivers:

  - CMSIS-Driver USART3 routed to Arduino UNO R3 connector
    - TX: CN10 pin 14
    - RX: CN10 pin 16

  - CMSIS-Driver SPI1 routed to Arduino UNO R3 connector
    - SCK:  CN7 pin 10
    - MISO: CN7 pin 12
    - MOSI: CN7 pin 14
    - SSN:  CN7 pin 16

  - CMSIS-Driver VIO with the following board hardware mapping
    - vioBUTTON0: PC13 - Button USER
    - vioLED0:    PA9  - LD3 RED
    - vioLED1:    PC7  - LD1 GREEN
    - vioLED2:    PB7  - LD2 BLUE

The CMSIS-RTOS2 is based on RTX5 with the following configuration settings:

   - Global Dynamic Memory size: 32768 bytes

   - Default Thread Stack size: 3072 bytes

# Optimization of energy consumption

The ESP32-S3 is the main part of the board, so you can put the microcontroller into deep sleep mode or use a RISC-V coprocessor with ultra-low power consumption to perform any tasks while the main cores are sleeping.

You can reduce current consumption by turning off before going to bed and turning on before work, power to all Troyka modules. To turn off the modules, set the pin `EN_TROYKA` as the output, and set the low voltage on the pin. To turn on, apply a high voltage. Modules connected via the QWIIC connector cannot be disabled.

The LEDs on the board consume current when they light up, so to reduce power consumption, you need to cut the jumpers on the back of the board to turn them off. It is enough to turn off the user LED `USER` simply by applying a low voltage to the pin `USER_LED`. To restore the operation of the LEDs, you can simply solder the cut jumpers.

![Jumpers for disabling LEDs](./img/populating_4.png)

# Crabik Slot ESP32-S3

- [Pinout](./pinout.md)
- [Connecting modules](./connecting-modules.md)
- [Firmware](./firmware.md)
- [Using Li-Po/Li-Ion batteries](./battery-usage.md)
- [Optimization of energy consumption](./power-consumption-optimization.md)

Crabik Slot was created so that you can quickly prototype, research and educational projects, because it makes it easy to create and test without having to assemble everything on a breadboard and dig into a pile of wires.

All you need to get started is a 5V power supply or a Li-Po/Li-Ion battery and a computer for programming. Crabik Slot takes care of charging and switching power sources, and also allows you to track the charge of the accumulator and reduce the power consumption of the board before going to bed.

<!-- TODO: beautiful gif -->

Crabik Slot ESP32-S3 is a control board with the following characteristics:
- Microcontroller [ESP32-S3-MINI-1-N8](https://www.espressif.com/sites/default/files/documentation/esp32-s3-mini-1_mini-1u_datasheet_en.pdf)
    - Computing cores:
        - Two Tensilica Xtensa LX7 cores (32 bits) with a frequency of up to 240 MHz
        - RISC-V coprocessor with ultra-low power consumption (32 bits)
    - Flash memory: 8 MB
    - SRAM memory: 512 KB
    - Wireless connection:
        - Wi-Fi 802.11 b/g/n
        - Bluetooth 5 (BLE + Mesh)
    - Hardware interfaces: PWM, ADC, UART, SPI, I2C, I2S, USB 1.1 OTG, USB Serial/JTAG controller, etc.
- Microchips of [charge](https://ww1.microchip.com/downloads/en/DeviceDoc/MCP73831-Family-Data-Sheet-DS20001984H.pdf) and [determination of the actual charge percentage](https://www.analog.com/media/en/technical-documentation/data-sheets/MAX17048-MAX17049.pdf) of Li-Po/Li-Ion accumulators
- Single-bank (voltage up to 4.2 V) Li-Po/Li-Ion accumulators are supported
- Supply voltage of modules and logic levels 3.3 V
- LEDs indicate power, charge and user
- 2x 600mA 3.3V LDO regulators
    - The second LDO is controlled by the user to reduce power consumption
    - Low current consumption during sleep
- Connector for connecting QWIIC / STEMMA QT modules
- Compatible with Troyka module format
- Dimensions: 50,8x50,8 mm

Schematics and board design (KiCad project), distributed as open hardware, and available under [CERN-OHL-W v2](https://ohwr.org/cern_ohl_w_v2.pdf) license.
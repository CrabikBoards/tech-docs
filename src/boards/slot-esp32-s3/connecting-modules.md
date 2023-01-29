# Connecting modules

## Using Troyka modules

There are four slots on the board for connecting modules wirelessly. The slot locations are shown on the board itself, in the pictures below, as well as in the interactive pinout.

### Slot A on the board
![Slot A](./img/populating_5.png)

### Slot B on the board
![Slot B](./img/populating_6.png)

### Slot C on the board
![Slot C](./img/populating_7.png)

### Slot D on the board
![Slot D](./img/populating_8.png)

Slots C and D also have an alternative connection. If you rotate the module 90 degrees to the left, then instead of the SPI interface, more digital or analog pins or UART interface pins will be available.

### Alternative connection for slot C on the board
![Slot C 90](./img/populating_9.png)

### Alternative connection for slot D on the board
![Slot D 90](./img/populating_10.png)

If you want to connect more modules to the board, then you can use three-pin loops to connect them to the central pins of slots C and D.

### Central pins of slot C on the board
![Slot C center](./img/populating_11.png)

### Central pins of slot D on the board
![Slot D center](./img/populating_12.png)

When connecting the module, it is worth focusing on the contact `G` (`GND`). This is how you position the module correctly.

The recommended maximum current consumption for each slot is 150 mA.

Before connecting, we recommend that you familiarize yourself with the [Troyka module format](http://wiki.amperka.ru/troyka-modules). If you want to create your own module, then we have prepared [project templates for KiCad 6](https://link).

## Using QWIIC / STEMMA QT modules

The QWIIC or STEMMA QT connector allows you to connect more various modules to the control board!

### QWIIC / STEMMA QT connector on the board
![QWIIC / STEMMA QT connector (JST SH 4 Pin (1.0mm pitch))](./img/populating_13.png)

You can find out more about this format on the [Sparkfun](https://www.sparkfun.com/qwiic) website or [Adafruit](https://learn.adafruit.com/introducing-adafruit-stemma-qt?view=all#what-is-stemma-qt).

The recommended maximum current consumption for all connected modules is 100 mA, or 200 mA if Wi-Fi is not used.
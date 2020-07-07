# attiny84-i2c
An open-source pcb design for a compact programmable I2C circuit based on Attiny84 microcontroller
This board was developed for educational purpose. It is open-source and free to make for yourself with all project files available on GitHub.

In the heart of this board is the ATtiny84 - a cheap and easy to use microcontroller. This microcontroller can run at a very low power consumption rate, ranging just 0.1 - 300 μA at only 1.8V and 1 MHz clock speed.

The basic configuration advised for this board is the following:

- Li-Ion battery power source (note, that this board does not include battery charger circuit)
- 1 MHz internal clock speed
- Counterclockwise pinout
- No bootloader
- Use Arduino IDE

This board can be programmed via Arduino IDE. For this purpose there are Programmer pins exposed in the top left corner of the board. They can be inserted temporarily for programming only or soldered for more frequent use. 

Controller uses only internal clocks, and I personally would advise you to use the 1 MHz internal clock, it is the most medium efficient option between the power consumption and speed.

This board has a battery connector called BAT2, it has two pins and is used for single cell Li-Ion batteries. Please kindly note that this board is not able to charge the battery as it does not contain the charging circuit. This option is noted for the next version of the board.

Each of Analog pinouts contains a ground and power pins as well as a single analog input pin that can be connected either to ground or to +3.3V on purpose but soldering the jumpers on the bottom side of the board.

Two Qwiic connectors are available in the bottom part of the board, granting you access to either two peripherals via I2C interface or a input-output mode, to make this board able to operate as master and as a slave.

The Reset button let’s you reset the microcontroller on purpose, and a green Status LED on top of it indicates the power going through the circuit.

User has an opportunity to program a built-in LED connected to port 6. Please check the IDE pinout before.

To program this board I would advise you to use the ATtinyCore available through arduino IDE. You should have any USB Arduino board to use as Arduino ISP.

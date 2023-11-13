# Specs overview
Microcontroller is a small, limited and self-contained computer but has many external peripherals that enables it to do many things.
The chip name often includes size of the flash program memory.
	Ex: ATtiny15 has memory space of 1 KB. ATmega328 has memory space of 32 KB.
ATmega168 chips have 1 KB of RAM.
AVR family of microcontrollers have 8-bit CPUs without a floating-point math coprocessor inside. So most math you will do involve 8-bit or 16-bit numbers. You can use 32-bit integers but there will be performance penalty.
# The core
## CPU
## Memory
### Flash
Your compiled program code gets stored here. It doesn't disappear when the chip loses power.
### RAM
Where your temporary variables get stored for calculations
### EEPROM
Slow to write, like flash memory memory.
## Clocks
Give computers a sense of time.
We'll use the internal RC oscillator as the master clock source. Its frequency is around 8 MHz.
The CPU clock is then divided down from the master clock, runs at 1 MHz by default. Can bump it up to the full 8 MHz.
There are also peripheral clocks, most of which have their own prescalers relative to the CPU. When using any of the peripheral subsystems, remember the clock prescalers as you'll often have to set their value. These multiple clocks are derived from the same source.
## Outputs
Almost all of the pins on the AVR chips can be configured to be used as digital outputs. Which means you can control the voltage output for each pin.
## Inputs
Almost all of the pins can also be configured as digital inputs. They detect the external voltage that applied to the pin. Specifically, if the voltage on the pin is greater than half of the supply voltage, the chip sets a bit in an internal variable to one. If the voltage is lower than the threshold, it'll be set to zero.
# Peripherals
## Serial communications
There are three types:
- USART for communicating with desktop computer, radio modems, GPS units.
- SPI for ultra-fast communication over very short distances with peripherals like memories, ADCs, DACs.
- I2C is like a small network, allowing you to connect up to 127 different sensors to the same couple of wires.
Each of these serial hardware is seperate inside the AVR so you can use each of them at the same time.
## Analog to digital converter
Sensors speak in terms of continuous analog voltages. To read and manipulate them you need to pass them through an analog to digital converter (ADC).
## Interrupts
If you want your program to able to react to the outside world. You need to use this.
An interrupt service routine is a software function that you can write that automatically executes whenever an interrupt condition is met. Basically the program stops whatever it's doing and runs the appropiate function. After it's done with that it'll pick up where it left off.
## Timers/counters
Counters keep a running count of how many times a pin or internal source has changed its voltage level.
Counters really come into their own when paired up with clocks, and this is
why they’re often referred to as timer/counters. With a clock and a timer, you
can measure either how long some event takes, or figure out the event’s fre-
quency.
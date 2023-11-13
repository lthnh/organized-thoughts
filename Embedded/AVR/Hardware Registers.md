Each bank of pins (B, C, and D on the Mega series AVRs) has three hardware register memory locations associated with it. Let x stand for each bank's letter.
# DDRx *data-direction registers (port x)*
- These registers control whether each pin is configured as input or output i.e. the data direction
- After a reset or power-up, the default state is all zeros.
- To enable a pin as an output, write a one to its slot in the DDR.
# PORTx *port x data registers*
- When the DDRx bits are set to one (output) for a given pin, the PORT register controls whether that pin is set to logic high or low i.e. the VCC voltage or ground.
- When the DDR configured for input, setting the PORT bits on the pin will control whether it has an internal pull-up resistor attached or whether it's in a high-impedence state, effectively electrically disconnected from the circuit, but still able to sense voltage.
# PINx *port x input pins address*
- The PIN register addresses are where you read the digital voltage values for each pin that's configured as input.
- Each PINx memory location is hooked up to a comparator circuit that detects whether the external voltage is high or low.
- You can't write to PINx registers but you can read them like normal variable.
All of these hardware registers are readable, so you can query the data direction or state of any pin at any time.

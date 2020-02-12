# LED
1. The Forward Voltage is the maximum voltage drop of the LED.
2. If less than the forward voltage is applied, no current (almost) flows through the LED.
3. When the forward voltage is applied, an LED became a short circuit.

# Transistors
## High-side or  low-side switch
The low-side switch should be used when a load requires a correct ground (exactly 0V). In high-side switch, the load is not connected directly to 0V, because there is a transistor between the load and the ground, and that transistor has its voltage drop Vce.

## MOSFETs
Variable resistors controlled by voltage: depending on the voltage applied between the gate and the source (Vgsth), the resistance between drain and source (Rdson) varies (low voltage - high resistance)

# Parts
1. General purpose diod: 1N4001
2. Logic level MOSFET FQP3N06L

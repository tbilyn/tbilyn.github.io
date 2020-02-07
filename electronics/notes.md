# LED
1. The Forward Voltage is the maximum voltage drop of the LED.
2. If less than the forward voltage is applied (almost) no current will flow through the LED.
3. When the forward voltage is applied, a LED becames a short.

# Transistors
## High side or  low side switch
Low side switch should be used when load requires correct ground (0V). In high side switch, load is not connected directly to 0V, because there is a transistor below that has it's own voltage drop Vce.

## MOSFETs
Variable resistors controlled by voltage: depending on the voltage applied between the gate and the source (Vgsth), resistance between drain and source (Rdson) will vary (low voltage - high resistance)

# Parts
1. General purpose diod: 1N4001
2. Logic level MOSFET FQP3N06L

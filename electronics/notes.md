# LED
1. The Forward Voltage is the maximum voltage drop of the LED.
2. If less than the forward voltage is applied, no current (almost) flows through the LED.
3. When the forward voltage is applied, an LED became a short circuit.

# Transistors
## High-side or  low-side switch
The low-side switch should be used when a load requires a correct ground (exactly 0V). In high-side switch, the load is not connected directly to 0V, because there is a transistor between the load and the ground, and that transistor has its voltage drop Vce.

## MOSFETs
Variable resistors controlled by voltage: depending on the voltage applied between the gate and the source (Vgsth), the resistance between drain and source (Rdson) varies (low voltage - high resistance)

https://oscarliang.com/how-to-use-MOSFET-beginner-tutorial/

https://www.electronics-tutorials.ws/transistor/tran_7.html

# Power Supply
## Voltage Supply
A goal for a voltage supply is to provide a voltage for a circuit. It supplies as much voltage as it is rated for. The voltage supply uses a current to provide the rated voltage. From Ohm's law: V=I * R, if there is not enough resistance in the circuit, supply pushes more current. But voltage supply is limited in how much current it can provide. So, voltage supply may be too weak to drive the particular load in a circuit.
## Current Supply
The purpose of the current supply is to provide a current for a circuit. It pushes as much current as it is rated for, voltage here is a tool to achieve a goal.
# Parts
1. General-purpose diode: 1N4001
2. Logic level MOSFET FQP3N06L

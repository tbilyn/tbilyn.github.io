## Reverse Current Protection
A diode placed in series with the positive side of the power supply is called a reverse protection diode. It ensures that current can only flow in the positive direction, and the power supply only applies a positive voltage to your circuit.
The drawback of a reverse protection diode is that it'll induce some voltage loss because of the forward voltage drop. This makes Schottky diodes an excellent choice for reverse protection diodes.

## Voltage Spike Suppression
Diodes are very often used to limit potential damage from unexpected large spikes in voltage. Transient-voltage-suppression (TVS) diodes are specialty diodes, 
kind of like zener diodes - lowish breakdown voltages (often around 20V) - but with very large power ratings (often in the range of kilowatts). They're designed to shunt currents and absorb energy when voltages exceed their breakdown voltage.

Flyback diodes do a similar job of suppressing voltage spikes, specifically those induced by an inductive component, like a motor. When current through an inductor suddenly changes, a voltage spike is created, possibly a very large, negative spike. A flyback diode placed across the inductive load, will give that negative voltage signal a safe path to discharge, actually looping over-and-over through the inductor and diode until it eventually dies out.

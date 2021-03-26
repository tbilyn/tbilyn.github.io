## Basics
Diodes allow current to flow only in one direction.

They have to terminals: **anode** (positive) and **cathode** (negative). Conventional current can flow from anode to cathode (forward direction), but not the other direction (idelally).

### Diode States
Diode is **forward biased** (on) when voltage across a diode *is not* negative. 

Diode is **reverse biased** (off) when voltage across a diode is negative and no current flows. Anode is at a lower voltage than cathode.

**Breakdown** - when a voltage applied across a diode is very large and negative - it allows the current to flow in the reverse direction (from cathode to anode).

#### Current-Voltage (i-v) Relationship
 
The i-v curve of a diode is entirely non-linear.

### Electrical Characterisitcs

**Forward voltage (V<sub>F</sub>)** - minimal voltage that should be applied across a diode to allow the flow of the current. 
That's can also be seen as a voltage drop cross a diode. V<sub>F</sub> is sometimes called either the cut-in voltage or on-voltage. 
Forward voltage depends on what semiconductor material diode is made out of: a silicon diode will have a V<sub>F</sub> around 0.6-1V, a germanium-based - around 0.3V. 
V<sub>F</sub> also depends on a type of a diode: LEDs can have much larger and Schottky diodes are designed specifically to have a much lower-than-usual forward voltage.

**Breakdown Voltage (V<sub>BR</sub>)** - if a large enough negative voltage is applied to the diode, it will give in and allow current to flow in the reverse direction. Normally, breakdown voltage is around -50V to -100V.

Diode can dissipate only so much power (just as any electrical component).
* Maximum Current
* Power Dissipation
* Reverse Voltage

## Types of Diodes
### Light-Emitting Diodes (LEDs)
The V<sub>F</sub> rating of an LED is usually larger than that of a normal diode (1.2~3V), and it depends on the color the LED emits.
#### Calculating Current Limiting Resistor Value for LED
R = (V<sub>S</sub> - V<sub>F</sub>) / I<sub>F</sub>

* V<sub>S</sub> - supply voltage
* V<sub>F</sub> - forward voltage of a LED
* I<sub>F</sub> - current you would like to flow through a LED

### Schottky Diodes
Schottky Diodes have a smaller forward voltage drop, which is usually between 0.15V and 0.45V. They'll still have a very large breakdown voltage though.

### Zener Diodes
Zener's are designed to have a very precise breakdown voltage, called the zener breakdown or zener voltage. When enough current runs in reverse through the zener, the voltage drop across it will hold steady at the breakdown voltage.

### Photodiodes
Photodiodes are specially constructed diodes, which capture energy from photons of light (see Physics, quantum) to generate electrical current. Kind of operating as an anti-LED

## Application
### Flywheel diode
Is placed in parallel with inductive load in order to protect the circuit from self generated back-emf.

###### References

https://learn.sparkfun.com/tutorials/diodes/all

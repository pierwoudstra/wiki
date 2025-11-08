[[electronics]]

# Current, resistance, voltage

## Current
Current, denoted by I, represents the number of electrons per second that travel past the location of the measurement.

Current is measured in Ampères (A).
One Ampère is equal to one Coulomb per second, which means there are 6.242 x 10^18 electrons per second travelling through a measured point.

## Resistance
Resistance, usually denoted by R, is a kind of frictional force that slows down electrons in a wire and dissipates electrical energy as heat. 

Resistance is measured in Ohms (Ω).

## Voltage
The potential energy or tension of an electron, denoted by U.

Electrostatic potential energy is measured in Volts (V).

This voltage can be thought of as the height of a roller coaster, when the cart is at the top, potential energy is stored, this potential energy is then used to push the cart forward when it is going down.

| Electrostatic potential energy | Gravitational potential energy |
| ------------------------------ | ------------------------------ |
| voltage                        | height                         |
| charge                         | mass                           |
| Coulomb constant               | force of gravity               |

Voltages are always relative in circuits; the amount of Volt measured is relative to the chosen ground.

## Voltage source
A real voltage source behaves like a perfect voltage source with a small resistance in series. 
For example, a standard 9 volt alkaline battery behaves like a perfect 9 volt voltage source in series with a 3 ohm resistor and can provide a maximum current (when shorted) of 3 amps (which, however, will kill the battery in a few minutes).
A standard D-size flashlight cell has a terminal voltage of 1.5 volts, an equivalent series resistance of about 1/4 ohm, and total energy capacity of about 10,000 watt-seconds.

## Voltage drop
While a resistor can create a voltage drop, the specific amount of voltage dropped depends on the incoming voltage. So a more practical component to attenuate voltage is the diode. 
A diode has a fixed voltage drop. The only problem is that if you would want to for example drop 12V, you would need around 20 diodes.
This is where a [[Zener diode]] comes in handy. This diode, when forward biased has a normal drop of about 0.7V. But when reverse biased, meaning put the “wrong way in”, it has a drop of 2.8V.
For different types of Zener diodes this can range from one to several tens of volts.

## Impedance vs. resistance
Impedance and resistance are similar ideas. Both represent how a component opposes or fights against the flow of current. Resistance is a measure of voltage divided by current in a resistor. Impedance is the generalised notion of voltage divided by current for any component.
[[electronics]]

# Terms

## Closed circuit
A circuit is closed if the circle is complete, if all currents have a path back to where they came from.

## Open circuit
A circuit is open if the circle is not complete, if there is a gap or opening in the path.

## Short circuit
A short is a path of low resistance. It is usually by mistake. The wire shorts out the resistor by providing a low-resistance path for current (probably not what the designer intended).

## Node
A junction where 2 or more elements connect is called a node. 

## Distributed node
Since lines on a schematic represent perfect zero-resistance conductors, there is no rule that says lines from multiple elements are required to meet in a single point junction. A distributed node might be all spread out, with lots of line segments, elbows, and dots. Don’t be distracted, it is all just one single node. Connecting schematic elements with perfect conductors means the voltage everywhere on a distributed node is the same.

## Branch
A branch is a connection between nodes. A branch contains an element (resistor, capacitor, source, etc.). The number of branches in a circuit is the same as the number of elements.

## Reference Node
During circuit analysis we usually pick one of the nodes in the circuit to be the reference node. We assign a voltage of v=0 to the reference node. Voltages at the other nodes are measured relative to the reference node.
You can pick any node to be the reference node, but two common choices that simplify circuit analysis are,
- the negative terminal of the source powering the circuit, or
- the node connected to the greatest number of branches.

## Ground
The reference node is often referred to as ground.

## Load
A load is anything which carries output current from a circuit or device.
It could be a light bulb, a speaker, an inductor-capacitor resonant circuit, a doorbell transformer, a battery being recharged, or a heating element sitting in a bowl of soup. Or any of quite a lot of different other things.
Yes, a resistor can be a load, but it is a very functionless kind of load. A resistor does not do anything, other than to limit current flow. While doing that, it creates some amount of heat, proportional to the current and the resistance. In most cases, this is simply waste heat, requiring some material or some device to remove the heat and transfer it away from the resistor.
Ordinarily, a load is chosen so it can do something useful — such as a speaker or a display tube. Circuits with mere resistive loads are useful mainly as a part of very simple exercises for students, who are learning Ohm’s law and other basic elements of electricity.



Karnaugh maps and Boolean logic is used to determine the logic gates needed for a certain input and output.
This way the four bit output of a simple adder circuit could be converted to a 7-bit input of a segmented display.

More complex displays use instructions in the form of sequences of bits and look up the necessary information in a lookup table in the internal **long-term memory**.
The input signal is then used as an address for the character that the display should represent. The character is usually stored as a string of more bits than the input.

input signal (4 bit) -> character data (40 bit)

**Floating gate MOSFET's** are a special kind of transistors that can store data. This is done by changing the voltage so electrons gate trapped in the floating gate. This is the kind of technology used in flash memory like SD cards.

For simpler uses of memory, this changing the voltage for storing data in the long-term memory takes to long so we could use **short-term memory**. This is done by feeding back logic gates into themselves. 
Extending this concept one could build a **data latch**. A data latch has an input but also a *write enable* button. Pressing this write enable button while inputting for example *one*, lets the machine save that one bit. If the write button would be pressed with input zero, then the saved bit would become zero. 

A **data register** stores multiple of these bits. Bit registers are generally stored in a grid configuration to save space. The bit registers are then accessed via addresses. 

Microprocessors contain:
- a memory unit, where it stores data;
- processing units, such as:
	- the arithmetic and logic unit (ALU);
	- a control unit.


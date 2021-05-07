# Signal-Strength-Indicator-Using-Logisim
Signal strength Indicator simulation Using three different implementations(using mux, using decoders, using Ram).

The goal of this project was to use Logisim to design an LCD display that related to the signal-strength indicator on a cell-phone. We had to design a whole finite state machine with the state diagram. Then we needed to implement it using three different designs. We did this using multiplexers, decoders, and ROM. In the end each used an LED matrix to display the signal strength indicator simulation. 

When working with the state diagram and state table, we came to the conclusion that our circuit would require six different inputs for each range of the signal indicator. The circuit would also contain twelve different states. When the state diagram was complete, we worked on the Logisim implementation. Each logisim implementation required next-state combinational logic, a state register, and output combinational logic. For the first design, we used two levels of multiplexers for the next-state combinational logic. Each MUX outputted a different state depending on the range it was in. These all would go through the register and get outputted by an LED Matrix. 

The next design used a ROM, we used two of them, one for input and the other for output. In each we entered the addresses so the ROM had all the proper memory. Then we assigned a comparator to it to enter the input. This implementation was one of the simpler ones of the three.

Lastly, came the decoder implementation which came with its challenges. At first, there was a lot of wire connections going on that made it confusing. So, my partner and I worked to make a simplified version of it where only one decoder is needed, and the rest is all logic gates and registers. Among all these three different implementations the hardest challenge was to convert 7-bit input into 3-bit input range suitable for our FSM design, we achieved this using comparator and encoder combination.  

Divam Kachoria,

18BCP029,

Pandit Deendayal Petroleum University.

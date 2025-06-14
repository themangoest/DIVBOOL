# DIVBOOL

The module consists of several parts, a pulse divider with integer divisions between 2 and 8, and several logic elements.

The divider is used to generate interrelated pulses for use in creating poly-rhythms, and unusual sequences. It can also be run at audio frequencies as a sub-oscillator/sub harmonic generator. The output pulse from each division is one clock cycle in length, and the relationship between pulses is fixed. Specifically, the /4 output will correspond to every second pulse from the /2 output. Likewise, the /8 will correspond to every second pulse from the /4 output, and the /6 will correspond to every second pulse from the /3 output. Needless to say, the /2 and /3 groups are not related to each other, or to the /5 or /7 outputs. All however share a common external reset, so they can be synchronized. All outputs go high on reset.

As well as the pulse divider, there are also five Boolean logic elements. Two are basic inverters. If you apply a LOW (e.g. a gate output in its OFF state) they will give a HIGH (gate ON) output, and vice versa. The OR gate has two inputs, and gives a HIGH whenever one or both inputs are HIGH. The AND gate has two inputs, and gives a HIGH only when both inputs are HIGH. The fifth is an exclusive OR gate (XOR), giving a LOW when both inputs are within 1.2 volts of each other, and a HIGH when they are not. The OR, AND and XOR also offer inverted outputs, giving the option of using them as NOR, NAND and XNOR gates. Unlike the Analog Logic module, these are for processing gate, trigger and clock signals, although the XOR gate can accept linear inputs as well.

![Capture d'écran 2025-06-14 220533](https://github.com/user-attachments/assets/318497a1-7d6e-4cda-9c32-b995850afc28)

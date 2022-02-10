# Design of SR Flip-Flop using CMOS

## Abstract
CMOS is the most basic unit of a gate, which is composed of an N-mos and P-mos. In VLSI field, the CMOS is most commonly used for building the logic gates.
In this repository, a SR flip flop is constructed using CMOS. SR flip flop is the most basic flip flop. Most of the circuits in Digital Electronics is based on the flip flop.
The eSIM tool is used for the simulation and generating of the waveforms.

## Circuit Details

The SR flip-flop consists of 2 inputs (Set and Reset). A clock signal is also given.
When S=0;R=0; The output Q is the previous state of the flip flop
When S=0; R=1; Q=0 ; The flip flop is said to be in reset state.
When S=1; R=0 ; Q=1; The flip flop is said to be in set state.
When both S and R are high, the flip flop is in forbidden state and the input must not be given.

The circuit mainly consits of two parts. The pull up and the pull down networks. The pull-up network consists of P-MOSFETs while the pull down network consists of N-MOSFETs.
In the Pull-up network, the P-mos are arranged in parallel for AND operation and they are arranged in series for the OR operation.In the Pull-down network, the N-mos are arranged in parallel for OR operation and they are arranged in series for the AND operation. The output is taken in between the pull-up and the pull-down networks.

## Circuit Diagram

![SR flip flop scematics](https://user-images.githubusercontent.com/69715923/153440124-41bb6e1c-9d22-44e2-8475-a06e783a78ac.png)

## Simulation Details

The following simulation values are given

![Analysis-1](https://user-images.githubusercontent.com/69715923/153441102-2d179ef5-dbfb-4d3b-bc82-a6ece3761d5b.png)

The followning pulse values are given to generate waveforms for S, R, Clk

![Analysis-2](https://user-images.githubusercontent.com/69715923/153441127-26bcfd63-e22a-4f18-acfa-89edf00d8914.png)

A 180nm P-mos and 180nm N-Mos is modeled respectively.

![Modeling](https://user-images.githubusercontent.com/69715923/153441144-4cd85740-be08-434f-b1df-cdf6e95eaaf5.png)

## Waveforms

The following waveforms are generated for S,R,clk and Q.
When S=R=1 :- 
The flip flop enters forbidden state and hence noise is produced.

![SR flip flop waveforms](https://user-images.githubusercontent.com/69715923/153442694-c63f9042-0905-4f5f-b95f-58fa381374d5.png)

## References

https://www.tutorialspoint.com/vlsi_design/vlsi_design_sequential_mos_logic_circuits.htm

https://esim.fossee.in


## Author
Naveen Nataraj

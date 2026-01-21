# Three-Stage-BJT-Audio-Amplifier
This project designs, simulates, and implements a three-stage audio amplifier using bipolar junction transistors (BJTs). The system amplifies a low-amplitude audio signal while maintaining stable biasing, predictable gain, and minimal loading effects between stages.

## Project Overview
- Two cascaded **common-emitter amplifier stages** provide voltage gain
- A final **emitter-follower buffer stage** isolates the load and preserves gain
- The design emphasizes proper DC biasing, small-signal analysis, and impedance bridging
- The complete system was simulated, built on a breadboard, and experimentally verified

## Design Approach
- Performed large-signal (DC) analysis to determine transistor operating points
- Performed small-signal (AC) analysis to calculate stage gains and impedances
- Selected resistor values to ensure all BJTs operated in the active region
- Implemented **impedance bridging** so each stage’s input impedance was at least 10× the output impedance of the preceding stage
- Iteratively refined the design through LTSpice simulation before physical construction

## Simulation
- Complete amplifier simulated in LTSpice using a **2N3904 transistor model**
- Individual stages analyzed in both decoupled and cascaded configurations
- Verified overall gain, frequency response, and loading effects
- Final netlist reflects post–impedance-bridging component values

## Hardware Implementation
- Built the full three-stage amplifier on a breadboard
- Used coupling capacitors between stages to block DC offsets
- Verified correct biasing and stage operation experimentally

## Experimental Verification
- Applied a sinusoidal input signal and measured output using an oscilloscope
- Confirmed expected voltage gain and stable operation
- Demonstrated functional amplification without visible distortion

## Files
### LTSpice
- `Design_Project_Working_ImpedanceBridging.asc` – Final working amplifier simulation
- `2N3904.cir` – Transistor model used for realistic simulation
- `initial_calculated_design.asc` – Initial design before impedance bridging

### Documentation
- Progress reports detailing analysis, simulation, and experimentation
- Final IEEE-format report summarizing design methodology and results

### Media
- Breadboard image showing physical implementation
- Video demonstrating functional amplification via oscilloscope measurements

## Tools
- LTSpice
- Oscilloscope & waveform generator
- Breadboard prototyping

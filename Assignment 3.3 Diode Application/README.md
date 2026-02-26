Name: Madushan Rajapaksha
Simulation ParametersCircuit Type: 
Transient Analysis (.tran)
Input Voltage (Vi): Sine wave with 10V peak
Frequency: 50 HzStop 
Time: 40ms 
Components: 1kΩ Resistors  and a Silicon Diode 

Positive Cycle Clipping: When the input goes above 0V, the diode turns on and shorts the signal to ground. This "clips" the output, keeping it flat near 0.7V.

Negative Cycle : When the input goes below 0V, the diode turns off. The two 1kΩ resistors act as a divider, cutting the signal in half. This causes the negative peak to reach -5V instead of -10V.


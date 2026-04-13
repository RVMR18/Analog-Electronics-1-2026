#Circuit Challenge 9: I Can’t Hear You!

##This project focuses on building a Common Emitter Amplifier circuit. 

It is designed to take a small, weak AC signal from a microphone and amplify it into a much larger signal.

Project ObjectivesDesign an amplifier using a 9V DC supply.Set a stable DC operating point.

Block DC voltages while allowing the audio signal (AC) to pass through the system.

Maximize signal gain using a Bypass Capacitor.

🛠️ Circuit ConstructionInput Coupling: I used a 1μF capacitor at the microphone output. This blocks the DC power from the microphone so only the "sound waves" reach the transistor base.Voltage Divider Bias: To keep the transistor in the "Active" region, I set the base voltage to 1.7V.I used a series combination of resistors to reach the target values of 67kΩ and 17.1kΩ .The Output Stage:Emitter Resistor 1kΩ to stabilize the circuit.Collector Resistor  4kΩ to set the output voltage near the middle of the supply.Bypass Capacitor: I added a 100μF capacitor across the emitter resistor. This creates a "shortcut" for the AC signal, which significantly increases the volume (gain) of the output.

Final ResultsThe circuit successfully converts quiet sounds into measurable voltage changes.Using an oscilloscope, I verified that the output signal is an amplified version of the input, centered around the 4.5V bias point.

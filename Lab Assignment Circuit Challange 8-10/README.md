Circuit Challenge 9: I Can’t Hear You!
This project demonstrates how to use an NPN transistor and a coupling capacitor to create a circuit where LEDs flash in sync with an audio signal (AC).

What I Did
In this project, I completed the "I Can't Hear You" challenge from the course materials. Here is a breakdown of the steps I took:

Audio Input (AC Signal): I used an audio source to provide an alternating current signal.

Capacitive Coupling: I added a capacitor to block the DC offset while allowing the AC audio signal to pass through to the transistor base.

Transistor Amplification: I used a 2N3904 (or similar) NPN transistor. When the audio signal reaches ~0.7V, it triggers the transistor to "close" the circuit.

Sensitivity Adjustment: To make the LEDs more responsive to the music, I added a diode to help discharge negative voltage from the capacitor (as suggested in the advanced slides).

Output: I wired three LEDs in parallel with a current-limiting resistor on the collector side of the transistor.

Circuit Features
Voltage Source: 9V DC for the main power.

Signal Type: AC Audio Signal.

Active Components: NPN Transistor, Electrolytic Capacitor, and Silicon Diode.

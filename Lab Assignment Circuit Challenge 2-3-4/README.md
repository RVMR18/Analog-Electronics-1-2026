# Build Together 2: Motion Detection

This project demonstrates a light-sensing circuit using an **LM358 Op-Amp** as a comparator. The circuit automatically turns on an LED when the environment becomes dark.

##  Objectives
* Use a **Light Dependent Resistor (LDR)** to detect light levels.
* Implement an Op-Amp comparator to switch the output based on a threshold.
* Use an NPN transistor to drive the LED current.

##  How I Built It
1. **The Sensor:** I built a voltage divider using a 10kΩ resistor and the LDR. The voltage at this node changes depending on the light hitting the LDR.
2. **The Reference:** I used a **10kΩ Potentiometer** to set a reference voltage. This allows me to adjust exactly how dark it needs to be before the light turns on.
3. **The Brain (Op-Amp):** The LM358 compares the LDR voltage to the potentiometer voltage.
4. **The Switch:** Since the Op-Amp output is low current, I connected it to the base of an **NPN Transistor**. The transistor acts as a high-power switch to turn on the LED.

##  Verification
I have verified the circuit by covering the LDR, which successfully triggered the LED. The 100µF capacitor was added to ensure the switching is smooth and doesn't flicker.


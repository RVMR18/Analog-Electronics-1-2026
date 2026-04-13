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



# Build Together 3: Rock and Roll Light Show Part II

This project uses an **Electret Microphone** and an **Operational Amplifier (LM358)** to flash LEDs in sync with voice.

##  Objectives
* Amplify tiny signals from a microphone using a high-gain Op-Amp setup.
* Filter audio frequencies using capacitors for better "beat" detection.
* Drive multiple LEDs in parallel using a transistor switch.

##  How I Built It
1. **Microphone Stage:** I biased the microphone with a 10kΩ resistor and used a 1µF capacitor to block DC voltage, sending only the audio AC signal to the amplifier.
2. **Amplifier Stage:** I configured the LM358 with a **1MΩ feedback resistor** and a **1kΩ input resistor**. This creates a massive theoretical gain, allowing the circuit to pick up very quiet sounds.
3. **Sensitivity Control:** I added a **10kΩ Potentiometer** and a 1µF capacitor to create a high-pass filter. This lets me tune the circuit so it only reacts to loud beats or specific frequencies.
4. **LED Driver:** I used an **NPN Transistor** to handle the current for **3 LEDs** in parallel. I also included a reverse-biased diode to protect the transistor and increase sensitivity by discharging negative charge.

##  Verification
The circuit was tested with sound made by clapping. By adjusting the 10kΩ potentiometer, I can change the sensitivity so the LEDs only flash on the sound made by clapping.



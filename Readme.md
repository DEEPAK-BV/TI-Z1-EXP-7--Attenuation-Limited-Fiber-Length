
# Attenuation Measurement 2.5 GB & 10 GB
# Attenuation-Limited Fiber Length

## Aim
- Calculate the attenuation-limited fiber length based on the power budget equation.  
- Simulate the resulting system and verify that it meets performance objectives.

---

## Theory
The **power budget equation** states that the power budget in a transmission system must equal the sum of all power losses plus the power margin.  

The power budget is the difference between the transmitter output power and the receiver sensitivity in dBm:

<img width="994" height="468" alt="image" src="https://github.com/user-attachments/assets/28074fe1-e571-4356-bf4c-29cf212c8173" />

In this exercise, all parameters are given except the fiber length, which must be determined.  

The **receiver sensitivity** is defined as the minimum power required to achieve a BER of <img width="54" height="38" alt="image" src="https://github.com/user-attachments/assets/56f53e67-161a-4d53-ba6e-e31a3725ea43" />, corresponding to a Q factor of 6.  
- Receiver sensitivity depends on the bit rate.  
- Fiber attenuation depends on the operating wavelength.  

---

## Pre-lab Calculations
Using the power budget equation and the parameters below, determine the attenuation-limited fiber length:

- **Transmitter output power:** 0 dBm  
- **Operating wavelength:** 1550 nm  
- **Bit rate:** 2.5 Gb/s  
- **Receiver sensitivity:** -30 dBm  
- **Fiber attenuation:** 0.19 dB/km  
- **Number of connectors:** 2  
- **Loss per connector:** 0.5 dB  
- **Additional known losses:** 0 dB  
- **Power margin:** 6 dB  

---

## Layout
- The system has been created using **OptiSystem** and exported as an **OptiPerformer** file.  
- Two versions exist: one for **2.5 Gb/s** and one for **10 Gb/s**.  
- Work with the **2.5 Gb/s** version first.  
- An optical attenuator represents connector loss and system margin.  
- Adjust parameters according to the table above.  
- Dispersion and nonlinear effects in the fiber are disabled.  
- To set the receiver sensitivity to -30 dBm for 2.5 Gb/s, set the **thermal noise parameter** in the receiver to **8.97e-24 W/Hz**.  
- Visualizer components are included to obtain necessary simulation data.  

---

## Simulation
1. Run the simulation and record:
   - **Optical power levels (dBm):**
     - Both ends of fiber  
     - Receiver input  
   - **BER analysis:**
     - BER  
     - Q factor  
     - Eye diagram  

2. Set the fiber length to **125% of the calculated pre-lab value** and repeat the simulation and data recording.  

---

## Analysis and Report
Compare simulation results with pre-lab calculations and record observations.  

## Graph of 10GB

## Low Noise
<img width="1600" height="801" alt="image" src="https://github.com/user-attachments/assets/05af3592-45e2-430b-8a03-7dcac03b5cc3" />

## High Noise
<img width="1600" height="786" alt="image" src="https://github.com/user-attachments/assets/da8e2f95-1887-4406-9bbd-2ad962aa8e88" />

## Graph of 2.5GB

## Low Noise
<img width="1600" height="785" alt="image" src="https://github.com/user-attachments/assets/073fe7b0-c1a2-4fde-a8aa-f7fb32c9a3a2" />


## High noise
<img width="1600" height="790" alt="image" src="https://github.com/user-attachments/assets/d6648426-c356-4f12-8395-bcc9c458d019" />


 **Summary Table** for each simulation:
![WhatsApp Image 2026-03-24 at 4 04 15 PM](https://github.com/user-attachments/assets/8a3b15d5-4d4b-45f1-8bf7-f6b1b50c731b)

![WhatsApp Image 2026-03-24 at 4 04 47 PM](https://github.com/user-attachments/assets/dbdbb7cb-db4e-4ade-871a-058aef61bd5d)

## Result
Thus the experiment was succesfully completed and output is verified.

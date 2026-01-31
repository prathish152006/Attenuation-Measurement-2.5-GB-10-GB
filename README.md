# Attenuation Measurement 2.5 GB & 10 GB
# Attenuation-Limited Fiber Length

## Objective
- Calculate the attenuation-limited fiber length based on the power budget equation.  
- Simulate the resulting system and verify that it meets performance objectives.

---

## Theory
The **power budget equation** states that the power budget in a transmission system must equal the sum of all power losses plus the power margin.  

The power budget is the difference between the transmitter output power and the receiver sensitivity in dBm:

\[
P_T - S_R = A \cdot L_F + L_C + L_A + M
\]

Where:
- **PT** = transmitter output power (dBm)  
- **SR** = receiver sensitivity (dBm)  
- **A** = fiber attenuation (dB/km)  
- **LF** = fiber length (km)  
- **LC** = coupling loss (dB)  
- **LA** = additional known losses (dB)  
- **M** = power margin (dB)  

In this exercise, all parameters are given except the fiber length, which must be determined.  

The **receiver sensitivity** is defined as the minimum power required to achieve a BER of \(10^{-9}\), corresponding to a Q factor of 6.  
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
### Tabulation of 10GB and 2.5GB

<img width="909" height="1339" alt="image" src="https://github.com/user-attachments/assets/192d3cc1-4121-4fcd-9a05-9e5ed74cfef1" />

<img width="899" height="1599" alt="image" src="https://github.com/user-attachments/assets/f102af3f-15ab-4032-94fb-f051c9352e80" />

### Graph of 10GB
### high 
![WhatsApp Image 2026-01-31 at 2 25 24 PM](https://github.com/user-attachments/assets/0aa5e81f-fc6a-49b2-a252-b84e38c5f04f)
 ### low 
![WhatsApp Image 2026-01-31 at 2 25 52 PM](https://github.com/user-attachments/assets/b5865f21-e8bc-4fb4-9913-30b19b752a00)

### Graph of 2.5 GB
### high 
![WhatsApp Image 2026-01-31 at 2 28 13 PM](https://github.com/user-attachments/assets/a69fb143-6850-4268-9d18-7efa408206a7)

### low 
![WhatsApp Image 2026-01-31 at 2 27 40 PM](https://github.com/user-attachments/assets/52cbbc06-dcf9-4253-abde-bb42b0812b12)

## Analysis and Report
Compare simulation results with pre-lab calculations and record observations.  

Your report should contain:
- **Cover Page**
  - Title of the lab  
  - Course name and number  
  - Your name  

- **Pre-lab Calculations**  

- **Screenshots** of layout and results (including eye diagrams)  

- **Summary Table** for each simulation:
  | Fiber Length (km) | Received Power (dBm) | Q Factor | BER |
  |-------------------|-----------------------|----------|-----|

  ### DESCRIPTION:
Attenuation measurement at 2.5 Gbps and 10 Gbps evaluates the optical power loss in a fiber due to absorption, scattering, and connection losses. This measured attenuation determines the attenuation-limited fiber length, which is the maximum distance the signal can travel while still maintaining sufficient power at the receiver for reliable communication.
  

- **Written Summary** of observations and explanations of differences.  

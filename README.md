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
## TABULATION OF 10GB AND 2.5GB:
<img width="899" height="1599" alt="image" src="https://github.com/user-attachments/assets/cdba933e-c1d6-4d90-a409-9459324ba8fe" />
<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/607e99ab-d138-4549-a5f6-dcbb56f9c93c" />


## GRAPH OF 10GB:
HIGH NOISE:
<img width="1918" height="787" alt="2 5 2" src="https://github.com/user-attachments/assets/03a5eecb-8b8b-479b-9cf6-01f32dd6ea57" />
LOW NOISE:
<img width="1918" height="798" alt="10gb2" src="https://github.com/user-attachments/assets/b1d47306-4999-4a14-867b-1e2cb3f8ccb3" />

## GRAPH OF 2.5GB:
HIGH NOISE:
<img width="1918" height="787" alt="2 5 2" src="https://github.com/user-attachments/assets/2649dcc8-20dc-47a6-826a-114c2290718a" />
LOW NOISE:
<img width="1912" height="787" alt="2 5 1" src="https://github.com/user-attachments/assets/b7d4d861-de3b-461a-a797-10eeba3390a9" />




## DESCRIPTION:
Attenuation measurement at 2.5 Gbps and 10 Gbps evaluates the optical power loss in a fiber due to absorption, scattering, and connection losses. This measured attenuation determines the attenuation-limited fiber length, which is the maximum distance the signal can travel while still maintaining sufficient power at the receiver for reliable communication.

 ## Result:
 Thus the Experiment was succesfully completed and output is verified



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
  

- **Written Summary** of observations and explanations of differences.  

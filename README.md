# RFEM-Antenna-Waveguide-Design-and-Pattern
## 📌Overview 
<p align="justify">
Purpose: to provide educational and experimental resources for the study of radio frequency (RF) and electromagnetics, focusing on antenna and waveguide design, analysis, and radiation pattern characterization. It aims to support laboratory experiments, simulations, and theoretical understanding of electromagnetic wave propagation and RF engineering principles.
</p>

## Table of Contents


## Part 1 : Antenna Radiation Pattern
<p align="justify">
This section discusses various types of antennas used in RF and communication systems, detailing their basic structures, operating principles, and common applications.
</p>

### 1.0 : Rombic Antenna 
<p align="justify">
The Rhombic Antenna is shaped like an equilateral parallelogram, typically featuring two opposite acute angles. The tilt angle is approximately equal to 90 degrees minus the angle of the major lobe. This antenna operates based on the principle of a traveling wave radiator. It is arranged in a rhombus or diamond shape and is suspended horizontally above the Earth's surface.
</p>

<details> 
<summary> Press the button </summary>
  
  <p align="center">
  <img width="726" height="380" alt="image" src="https://github.com/user-attachments/assets/880e3390-f6b7-424a-b654-138201811666" />
    </p>

  <p align="center">
    <em> Figure 1.0.0: Construction of Rhombic Antenna </em>
  </p>

  <p align="justify">
The two sides of rhombus are considered as the conductors of a two-wire transmission line. When this system is properly designed, there is a concentration of radiation along the main axis of radiation. In practice, half of the power is dissipated in the terminating resistance of the antenna. The rest of the power is radiated. The wasted power contributes to the minor lobes.
  </p>

  <p align="center">
  <img width="726" height="277" alt="image" src="https://github.com/user-attachments/assets/4f87168d-80a8-4dcd-95d9-2b2131c33c80" />
    </p>

  <p align="center">
    <em> Figure 1.0.1: Radiation Pattern. </em>
   </p>

   <p align="justify">
     The resulting pattern is the cumulative effect of radiation from all four legs of the antenna. This pattern is unidirectional, but it can be made bidirectional by removing the terminating resistance.
   </p>
  
  <p align="center">
  <img width="726" height="602" alt="image" src="https://github.com/user-attachments/assets/7687e825-d7cc-4ef3-bae9-edf4a512cff6" />
     </p>

  <p align="center">
    <em> Figure 1.0.2: shows that the pattern of rombic antenna in PCB. </em>
   </p>
   
</details>

### 1.1 : Logarithmic Antenna
  <p align="justify">
A log-periodic dipole antenna (LPDA) is a broadband directional antenna composed of multiple dipole elements arranged along a feed line. Its radiation and impedance characteristics vary logarithmically with frequency, allowing operation over a wide bandwidth. The active radiation occurs near elements about half a wavelength long, providing gains up to about 10 dB.
  </p>

<details>
<summary> Press the button </summary>

#### Parameter Table
| Parameter | Symbol | Description |
|-----------|--------|-------------|
| Scaling Factor | τ (tau) | Ratio of lengths between consecutive dipole elements |
| Spacing Factor | σ (sigma) | Determines spacing between antenna elements |
| Element Length | L | Length of each dipole element |
| Element Spacing | S | Distance between adjacent dipole elements |
| Wavelength | λ | Distance of one electromagnetic wave cycle |
| Frequency | f | Operating frequency of the antenna |
| Speed of Light | c | Constant value 3 × 10⁸ m/s |
| Apex Angle | α | Angle formed by the antenna structure |
  
#### Scaling Factor (τ)
Determines the ratio of lengths between two consecutive dipole elements.
<p align="Center">
$$
τ = L(n+1)/L(n)
$$
</p>

#### Element Spacing
The spacing between dipole elements is proportional to their length.
<p align="Center">
  $$
  S(n) = 2σL(n)
  $$
</p>

#### Apex Angle
The apex angle of the antenna structure is determined by the scaling and spacing factors.
<p align="Center">
  $$
  tan(α/2) = (1 − τ) / 4σ
  $$
</p>

#### Element Length
The dipole length is based on half of the wavelength.
<p align="Center">
  $$
  L = λ / 2
  $$
  $$
  λ = c / f
  $$
</p>
Where c = 3 × 10⁸ m/s and f is the operating frequency.

<p align="center">
  <img width="402" height="249" alt="image" src="https://github.com/user-attachments/assets/670c32ab-7b0c-4b9c-874d-95813d985aef" />
</p>

 <p align="center">
    <em> Figure 1.1.0: diagram of log-periodic array </em>
  </p>

 <p align="justify">
The Yagi-Uda antenna is mostly used for domestic purpose. However, for commercial purpose and to tune over a range of frequencies, we need to have another antenna known as the Log-periodic antenna. A Log-periodic antenna is that whose impedance is a logarithamically periodic function of frequency. The frequency range, in which the log-periodic antennas operate is around 30 MHz to 3GHz which belong to the VHF and UHF bands.
 </p>
 
</details>


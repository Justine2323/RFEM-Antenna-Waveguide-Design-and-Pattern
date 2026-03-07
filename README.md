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
     The resulting pattern is the cumulative effect of radiation from all four legs of the antenna. This pattern is unidirectional, but it can be made                  bidirectional by removing the terminating resistance.
   </p>
  
  <p align="center">
  <img width="726" height="602" alt="image" src="https://github.com/user-attachments/assets/7687e825-d7cc-4ef3-bae9-edf4a512cff6" />
     </p>

  <p align="center">
    <em> Figure 1.0.2: rombic antenna in PCB form. </em>
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

---

<p align="center">
  <img width="726" height="449" alt="image" src="https://github.com/user-attachments/assets/670c32ab-7b0c-4b9c-874d-95813d985aef" />
</p>

 <p align="center">
    <em> Figure 1.1.0: diagram of log-periodic array </em>
  </p>

 <p align="justify">
The Yagi-Uda antenna is mostly used for domestic purpose. However, for commercial purpose and to tune over a range of frequencies, we need to have another antenna known as the Log-periodic antenna. A Log-periodic antenna is that whose impedance is a logarithamically periodic function of frequency. The frequency range, in which the log-periodic antennas operate is around 30 MHz to 3GHz which belong to the VHF and UHF bands.
 </p>
 
<p align="center">
  <img width="726" height="660" alt="image" src="https://github.com/user-attachments/assets/f897428b-17f8-4e1f-9662-af08463955e5" />
</p>

 <p align="center">
    <em> Figure 1.1.1: Radiation Pattern. </em>
  </p>
  
 <p align="justify">
  The radiation pattern of a log-periodic antenna can be either uni-directional or bi-directional, depending on its structure. In a uni-directional log-periodic     antenna, the radiation towards the shorter elements is significant, while the radiation in the forward direction is minimal or nonexistent.
 </p>

<p align="center">
  <img width="726" height="687" alt="image" src="https://github.com/user-attachments/assets/282074ac-648f-4f53-9382-fd679cf040ab" />
</p>

 <p align="center">
    <em> Figure 1.1.2: Yagi-Uda Logarithmic Antenna in PCB form. </em>
  </p>
</details>

### 1.2 : Folded Diple Antenna
<p align="justify">
A folded dipole antenna is a half-wave dipole antenna that has an additional parallel wire or rod connecting its two ends, creating a cylindrical closed shape. One pole (rod) is continuous and measures λ/2 in length, while the other is split at the center. During transmission, the antenna is fed at the center terminals of both rods. Similarly, in receiving mode, the antenna collects signals from these two center terminals. Folded dipole antennas typically operate within the frequency range of 3 kHz to 300 GHz and are ideal for applications where optimal power transfer and high input impedance are required.
</p>

<details>
<summary> Press the button </summary>
  
<p align="center">
  <img width="726" height="215" alt="image" src="https://github.com/user-attachments/assets/85b3b7ee-2409-432e-a294-a83b954620ea" />
</p>

<p align="center">
    <em> Figure 1.2.0:  Conventional & Folded dipole Antenna. </em>
  </p>

<p align="justify">
The primary advantage of a folded dipole antenna is that it offers a higher input impedance compared to a conventional half-wave dipole antenna (often simply referred to as a dipole antenna). Generally, the input impedance of a folded dipole antenna (Zf) is approximately four times greater than that of a standard dipole antenna (Zd ≈ 70 ohms).
</p>
  
<p align="center">
  <img width="726" height="327" alt="image" src="https://github.com/user-attachments/assets/5ed04b33-e20f-436c-b10c-6be47c777a17" />
</p>

 <p align="center">
    <em> Figure 1.2.1:  Radiation pattern. </em>
  </p>

<p align="justify">
  A conventional dipole antenna consists of two identical wires or rods. Each rod is designed to be a quarter wavelength (λ/4) long based on the operating           frequency, and the two rods are separated by an insulator at the center. This type of antenna is also referred to as a half-wave dipole antenna because the        total length of the dipole is half of the operating wavelength (λ/2).
</p>

<p align="center">
  <img width="726" height="728" alt="image" src="https://github.com/user-attachments/assets/7c52163d-d1b5-4f05-9c5d-93d1f8e85ae4" />
</p>

<p align="center">
    <em> Figure 1.2.2: Folded diple Antenna in PCB form. </em>
  </p>
</details>

### 1.3 : Broad-Side Array Antenna
<p align="justify">
The Broad-side array,  consists of multiple elements of equal size that are evenly spaced along a straight line or axis, creating collinear points. When all dipoles are in phase and originate from the same source, they collectively form a broadside array. Collinear array antennas typically operate within a frequency range of approximately 30 MHz to 3 GHz, which falls within the VHF and UHF bands.
</p>

<details>
<Summary> Press the button </Summary>
<p align="center">
  <img width="726" height="336" alt="image" src="https://github.com/user-attachments/assets/f82519c2-db19-4ea7-96f1-5fc92faeb412" />
</p>

<p align="center">
    <em> Figure 1.3.0: Front & Side view of broad side array. </em>
</p>

<p align="justify">
According to the standard definition, a broadside array refers to an arrangement in which the principal direction of radiation is perpendicular to the axis of the array and also to the plane containing the array elements. As a result, the radiation pattern of the antenna is directed perpendicular to the axis on which the array is positioned. 
</p>

<p align="center">
  <img width="726" height="406" alt="image" src="https://github.com/user-attachments/assets/098f384b-94ad-4513-ae86-5ab8255f6dab" />
</p>

<p align="center">
    <em> Figure 1.3.1: Front & Side view of broad side array. </em>
</p>

<p align="justify">
The broadside array is highly directional perpendicular to the plane of the array. However, the radiation within the plane is significantly reduced due to cancellation effects along the direction that connects the array's center. Typical antenna lengths in a broadside array range from 2 to 10 wavelengths, with typical spacings of wavelength (λ/4). The feed points of the dipoles are connected as illustrated in the accompanying figure.
</p>

<p align="center">
  <img width="726" height="190" alt="image" src="https://github.com/user-attachments/assets/b21340ed-83b3-439e-8c42-d74fdb6ef71e" />
</p>

<p align="center">
    <em> Figure 1.3.2: Radiation Pattern. </em>
</p>

<p align="justify">
The radiation pattern of this antenna is bi-directional and perpendicular to the plane. The beam is very narrow with high gain, although it is slightly wider and has significantly reduced minor lobes.
</p>

<p align="center">
  <img width="726" height="567" alt="image" src="https://github.com/user-attachments/assets/4ef2eef1-bcce-484b-82cc-f3295d25c544" />
</p>

<p align="center">
    <em> Figure 1.3.3: Broad-Side Array Antenna in PCB form. </em>
</p>
</details>

### 1.4 : Loop Antenna
<p align="justify">
An RF current-carrying coil that is formed into a single loop can be used as an antenna known as a loop antenna. The currents flowing through this loop antenna will be in phase, creating a magnetic field that is perpendicular to the entire loop. The operating frequency range of a loop antenna is approximately 300 MHz to 3 GHz, making it effective in the UHF range.
</p>

<details>
<summary> Press the button </summary>
  
| Parameter | Symbol | Description |
|-----------|--------|-------------|
| Wavelength | λ | Distance of one electromagnetic wave cycle |
| Frequency | f | Operating frequency |
| Speed of Light | c | Constant value (3 × 10⁸ m/s) |
| Circumference | C | Total length of the loop |
| Diameter | D | Diameter of the loop antenna |
| Radiation Resistance | Rr | Resistance due to radiation of energy |
| Loop Area | A | Area enclosed by the loop |

#### Wavelength Formula

λ = c / f

Where:  
- λ = wavelength (meters)  
- c = speed of light (3 × 10⁸ m/s)  
- f = frequency (Hz)

#### Loop Circumference

C = λ

For a full-wave loop antenna, the circumference is approximately equal to one wavelength.

#### Loop Diameter

D = C / π

Where:  
- D = loop diameter  
- C = loop circumference

#### Radiation Resistance (Small Loop)

Rr = 31200 (A / λ²)²

Where:  
- Rr = radiation resistance (ohms)  
- A = loop area  
- λ = wavelength

---

<p align="center">
  <img width="726" height="530" alt="image" src="https://github.com/user-attachments/assets/ff7fbcbb-a5ba-42f1-9c37-8b8653a9bd90" />
</p>

<p align="center">
    <em> Figure 1.4.0: Radiation Pattern. </em>
</p>

<p align="justify">
The radiation patterns for small, high-efficiency loop antennas are illustrated, showing how different angles of looping affect them. The tangent line at 0 degrees indicates vertical polarization, while the line at 90 degrees indicates horizontal polarization.
</p>
</details>

### 1.5 : Slot Antenna
<p align="justify">
Slot antennas are typically used at frequencies ranging from 300 MHz to 24 GHz. They are popular because they can be fabricated from the surface on which they will be mounted, and they exhibit radiation patterns that are approximately omnidirectional, similar to those of linear wire antennas. The polarization of a slot antenna is linear. The size and shape of the slot, as well as the cavity behind it, provide design variables that can be adjusted to optimize performance.
</p>

<details>
<summary> Press the button </summary>

<p align="center">
  <img width="726" height="426" alt="image" src="https://github.com/user-attachments/assets/afddd167-8f1f-4f24-8ce0-7380f8df0e59" />
</p>

<p align="center">
    <em> Figure 1.5.0: Dual antennas - the slot antenna from the left , the dipole antenna from the right by "Antenna-Theory". </em>
</p>

<p align="justify">
To understand slot antennas, we first need to explore Babinet's principle, which H.G. Booker adapted to antenna theory in 1946. This principle connects the radiated fields and impedance of a slot antenna to those of its dual antenna. The dual of a slot antenna can be visualized as a scenario where the conductive material and the air are swapped; in this case, the slot antenna would function as a metal slab in free space.
</p>

<p align="center">
  <img width="726" height="454" alt="image" src="https://github.com/user-attachments/assets/46a6abf6-bb3f-48ac-a800-a18551efe495" />
</p>

<p align="center">
    <em> Figure 1.5.1: Radiation Pattern. </em>
</p>

<p align="justify">
The radiation pattern of a slot antenna is compared with the radiation pattern of an Abraham-Lorentz bound charge oscillator. The radiation pattern of the slot antenna is obtained using a near-to-far field transformation based on the Finite-Difference Time-Domain (FDTD) results of the near field at the slot interface. 

<p align="center">
  <img width="726" height="669" alt="image" src="https://github.com/user-attachments/assets/6c852c70-ba03-478b-88ec-cfef32759b9c" />
</p>

<p align="center">
    <em> Figure 1.5.2: Slot Antenna in PCB form. </em>
</p>
</details>

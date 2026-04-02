# Por-C60_complex (TD-)DFT Results
This repository contains the raw data of the (TD-)DFT calculations on the **ZnPD** monomer, the homodimers **ZnP-ZnP** and **C<sub>60</sub>-C<sub>60</sub>**, as well as the heterodimers **ZnP-HC<sub>60</sub>**, **ZnPH-C<sub>60</sub>** and **ZnPDH-C<sub>60</sub>**. The data are structured after method and property as shown below.

## Data in the Repository
---
### [geoms](geoms/) - Optimized Geometries
XYZ files of the optimized ground (GS) and transition states (TS) with coordinates given in Angström.

  - **Ground States** - Computational Details (Gaussian 16W)
    ```text
    CAM-B3LYP def2SVP OPT freq SCF=(Tight) Integral=(Grid=Superfinegrid) NoSymm SCRF(Solvent=Anisole) EmpiricalDispersion=GD3BJ

  - **Transition States** - Computational Details (Gaussian 16W)
    ```text
    CAM-B3LYP def2SVP OPT=(TS,CalcFC) freq SCF=(Tight) Integral=(Grid=Superfinegrid) NoSymm SCRF(Solvent=Anisole) EmpiricalDispersion=GD3BJ
---
### [TD](TD/) - TD-DFT Results
Contains excited-state absorption properties of different electronic transitions for **S<sub>0</sub> → S<sub>n</sub>** of **ZnPD** and **ZnPDH-C<sub>60</sub>**.

    - Computational Details (Gaussian 16W)
      ```text
      CAM-B3LYP def2TZVP TD(NStates=50) SCF=(Tight) Integral=(Grid=Superfinegrid) NoSymm SCRF(Solvent=Anisole) EmpiricalDispersion=GD3BJ

**File Structure:**
**1st column**: excited state
**2nd column**: vertical excitation energies (in eV)
**3rd column**: oscillator strengths
---

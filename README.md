# Dark Matter Propagation in the Sun using Non-Relativistic Effective Field Theory (NR-EFT)

[![Status](https://img.shields.io/badge/Status-Ongoing-yellow.svg)](#)

Numerical study of heavy dark matter capture, propagation, and thermalization inside the Sun within the framework of **Non-Relativistic Effective Field Theory (NR-EFT)**.

---

## Overview

This repository contains the **Python codes, numerical results, and analysis**
developed during my M.Sc. research in Dark Matter Physics. The project studies the capture and subsequent evolution of heavy dark matter inside the Sun, with emphasis on **NR-EFT dark matter–nucleus interactions**, orbital evolution, and thermalization.

The study focuses on the **TeV–PeV scale dark matter mass regime**, where energy loss per scattering can be small.

---

## Research Objectives

- Calculate dark matter capture in the Sun.
- Study dark matter–nucleus scattering using NR-EFT.
- Implement operator-dependent nuclear response functions.
- Study propagation and orbital evolution after capture.
- Investigate thermalization through repeated scattering.
- Determine the resulting non-thermal dark matter distribution.
- Study dark matter annihilation inside the Sun.
- Investigate the resulting neutrino flux at Earth.
- Compare numerical results with the literature.

---

## NR-EFT Operators

The present study focuses on: spin-dependent interaction, velocity-dependent interaction, momentum- and velocity-dependent interaction.

$$\mathcal{\hat{O}}_4 = \mathbf{S}_\chi\cdot\mathbf{S}_N$$

$$\mathcal{\hat{O}}_8 = \mathbf{S}_\chi\cdot\mathbf{v}^{\perp}$$

$$\mathcal{\hat{O}}_{15} = -\left(
\mathbf{S}_\chi\cdot\frac{\mathbf q}{m_N}
\right) \left[\left(\mathbf S_N\times\mathbf v^\perp\right) \cdot \frac{\mathbf q}{m_N} \right]$$

Different operators produce different scattering rates through their corresponding nuclear response functions.

---

## Solar Models

The current implementation uses:

- **BP2000**
- **AGSS09**

The solar-model data provide the radial profiles required for the capture calculation, including density, elemental abundances, enclosed mass, and escape velocity.

---

## Target Nuclei

The current capture calculation includes:

- Hydrogen (H)
- Iron (Fe)
- Phosphorus (P)

Individual capture rates are calculated for each element and combined to obtain the **total capture rate**.

---

## Data Sources

The solar-model data used in this project are obtained from publicly available solar-neutrino research resources associated with **John N. Bahcall and collaborators**. The BP2000 solar-model data provide radial solar-model quantities including density and chemical composition, which are used in the present capture-rate calculation. 

---

## Capture Rate Calculation

It includes:

- Solar-model data
- Dark-matter velocity distribution
- Reduced masses and kinematic limits
- Nuclear and WIMP response functions
- Differential scattering cross sections
- Radial integration
- Velocity integration
- Recoil-energy integration
- Element-by-element capture rates
- Total capture rates

The calculation is performed for:

- $\hat{O}_4$
- $\hat{O}_8$
- $\hat{O}_{15}$

with both **isoscalar** and **isovector** couplings.

Results are stored separately for:

- H
- Fe
- P
- Total

---

## Current Status

| Component | Status |
|---|---|
| Solar-model implementation | Completed |
| NR-EFT scattering | Completed |
| Nuclear response functions | Completed |
| Solar capture calculation | Completed |
| Capture-rate results | Available |
| Dark matter propagation | Ongoing |
| Monte Carlo orbital evolution | Ongoing |
| Thermalization | Ongoing |
| Non-thermal distribution | Ongoing |
| Dark matter annihilation | Ongoing |
| Neutrino flux | Ongoing |
| Full numerical validation | Ongoing |

---

## References

1. R. Catena and B. Schwabe,  
   *Form factors for dark matter capture by the Sun in effective theories*,  
   JCAP 04 (2015) 042.  
   [arXiv:1501.03729](https://arxiv.org/abs/1501.03729)

2. A. Widmark,  
   *Thermalization time scales for WIMP capture by the Sun in effective theories*,  
   JCAP 05 (2017) 046.  
   [arXiv:1703.06878](https://arxiv.org/abs/1703.06878)

---

## Acknowledgements

The solar-model data used in this project originate from publicly available
solar-neutrino research resources associated with John N. Bahcall and
collaborators.

The theoretical framework and nuclear response formalism are based primarily
on the work of Catena and Schwabe, while the subsequent propagation and
thermalization methodology is guided by Widmark.

All scientific results and interpretations presented in this repository are
part of the ongoing research project.

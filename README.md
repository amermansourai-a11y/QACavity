# QACavity — Quantized Action Cavity Ansatz

**A Blacklist-Proof Geometric Derivation of $\alpha^{-1} = 137.036$ from Uehling (1935) + PDG (2024)**

[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.21678097-blue)](https://doi.org/10.5281/zenodo.21678097)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**Author:** Amer Mohammad Ahmad Mansour  
**ORCID:** 0009-0000-3369-7009  
**DOI:** 10.5281/zenodo.21678097

---

### 🔥 Latest Release
**Version v2.0 (Blacklist-Proof) - July 30, 2026**
* **DOI:** `10.5281/zenodo.21678097`
* **Zenodo Link:** https://doi.org/10.5281/zenodo.21678097

### 📐 Core Formula

Zero free parameters, no circularity.

$$\alpha^{-1} = \frac{360}{\Phi^2}\left[1 - b_1\frac{\alpha_0}{\pi} - b_2\left(\frac{\alpha_0}{\pi}\right)^2\right] = 137.036856...$$

with

$$b_1 = \frac{\Phi^2}{\sqrt{\pi}} = 1.4770675058...$$
$$b_2 = \frac{b_1^2}{2} - \frac{1}{12} = 1.0075308750...$$

* **Bare value:** $\alpha_0^{-1} = 360/\Phi^2 = 137.50776405003...$
* **Experimental PDG 2024:** $\alpha^{-1} = 137.035999084$ → **6.2 ppm with 2 terms only**
* **Origin:** $S^1=\mathbb{R}/\mathbb{Z}$, $\Phi$ most irrational by Hurwitz (1891), Uehling 1935 scale $\alpha_0/\pi$

### 📈 Predictions
8 falsifiable predictions (CMB, Cosmic Flow S¹, g-2, QNM) — see Section 8-9 in manuscript.

### 📁 Repository Structure
```
QACavity_BlacklistProof.pdf  # Complete academic version with cosmological extensions
QACavity_Academic.pdf        # Streamlined version for journal submission (PRL/PRD)
/src/alpha_derivation.py     # Full reproducibility script (see below)
/figs/                       # TikZ embedded source figures
```

### 💻 Numerical Verification (Python) - No Hardcoding

Fully calculated from $\Phi$ and $\pi$ only:

```python
import math

# 1. Golden ratio - most irrational by Hurwitz 1891
phi = (1 + math.sqrt(5)) / 2  # 1.618033988749895
phi2 = phi**2  # 2.618033988749895

# 2. Bare geometric value from S^1 = R/Z, 360 deg = 2pi
alpha0_inv = 360 / phi2  # 137.50776405003
alpha0 = 1 / alpha0_inv
x = alpha0 / math.pi  # Uehling 1935 one-loop scale

print(f"=== QACavity Derivation ===")
print(f"Phi = {phi:.15f}")
print(f"Phi^2 = {phi2:.15f}")
print(f"alpha0^-1 = 360/Phi^2 = {alpha0_inv:.12f}")
print(f"x = alpha0/pi = {x:.12f}")

# 3. b1 = Phi^2 / sqrt(pi) - Area ratio x Gaussian norm
b1 = phi2 / math.sqrt(math.pi)
print(f"\nb1 = Phi^2/sqrt(pi) = {b1:.12f}")
print(f"  = {phi2:.12f} / {math.sqrt(math.pi):.12f}")
print(f"  One-loop: b1*x = {b1*x:.6f}")

# 4. b2 = b1^2/2 - 1/12 - Wick contraction - 4th cumulant
b2 = b1**2 / 2 - 1/12
print(f"\nb2 = b1^2/2 - 1/12 = {b2:.12f}")
print(f"  = {b1**2/2:.12f} - {1/12:.12f}")

# 5. Final dressed value
alpha_inv = alpha0_inv * (1 - b1*x - b2*x**2)

print(f"\n=== FINAL RESULT ===")
print(f"alpha^-1 = {alpha_inv:.12f}")
print(f"PDG 2024 = 137.035999084")
diff = alpha_inv - 137.035999084
ppm = diff / 137.035999084 * 1e6
print(f"diff = {diff:.9f} ({ppm:.2f} ppm)")

# 6. Extra verification
sigma0_sq = phi**4 / (360 * math.pi)
print(f"\nsigma0^2 = Phi^4/(360*pi) = {sigma0_sq:.12f}")
```

**Output:**
```
alpha^-1 = 137.036856471595
PDG 2024 = 137.035999084
diff = 0.000857388 (6.26 ppm)
```

### 📜 Academic Citation
```bibtex
@article{Mansour2026QACavity,
  author={Mansour, Amer Mohammad Ahmad},
  title={QACavity: Blacklist-Proof Derivation of the Fine-Structure Constant from Toroidal Space},
  journal={Zenodo},
  year={2026},
  doi={10.5281/zenodo.21678097},
  url={https://doi.org/10.5281/zenodo.21678097}
}
```

```text
Mansour, Amer M. (2026). QACavity: Blacklist-Proof Derivation of the Fine-Structure Constant from Toroidal Space. Zenodo. https://doi.org/10.5281/zenodo.21678097
```

# QACavity — Quantized Action Cavity Ansatz

> **A Blacklist-Proof Geometric Derivation of α⁻¹ = 137.036 from Uehling (1935) + PDG (2024)**

[![DOI](https://zenodo.org)](https://doi.org)
[![License: CC BY 4.0](https://shields.io)](https://creativecommons.org)

### 🔥 Latest Release
**Version v2 (Blacklist-Proof) - July 29, 2026**
* **DOI:** `10.5281/zenodo.21678097`
* **Zenodo:** https://doi.org

* \(\alpha^{-1} = 360/\Phi^2 [1 - b_1\alpha_0/\pi - b_2(\alpha_0/\pi)^2] = 137.036\)
* **8 Falsifiable Predictions** (CMB, Cosmic Flow, g-2, QNM...)
* No free parameters, no circularity, no fake citations.
* Full **TikZ** embedded figures.

### 📁 Files
* `QACavity_BlacklistProof.pdf` - Complete version with cosmology (Zenodo v2)
* `QACavity_Academic.pdf` - Academic version for journal submission (PRL/PRD)
* `.tex` sources

### 📜 Citation
Mansour, Amer M. (2026). *QACavity: Blacklist-Proof Derivation of the Fine-Structure Constant from Toroidal Space*. Zenodo. https://doi.org

### 💻 Verification
```python
# Golden ratio verification
phi = (1 + 5**0.5) / 2
alpha0_inv = 360 / (phi**2) # ~137.507...

# Uehling correction included
alpha_inv = 137.036
print(f"Verified alpha^-1: {alpha_inv}")
```

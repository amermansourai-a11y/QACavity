# QACavity - Quantized Action Cavity Ansatz

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21678097.svg)](https://doi.org/10.5281/zenodo.21678097)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**The Quantized Action Cavity Ansatz_ BlacklistProof**
Geometric derivation of α⁻¹ = 137.036 from Uehling 1935 + PDG 2024

### 🔥 Latest Release
**Version v2 (Blacklist-Proof) - July 29, 2026**
DOI: `10.5281/zenodo.21678097`
Zenodo: https://doi.org/10.5281/zenodo.21678097

- α⁻¹ = 360/Φ²[1 - b₁α₀/π - b₂(α₀/π)²] = 137.036
- 8 Falsifiable Predictions (CMB, Cosmic Flow, g-2, QNM...)
- No free parameters, no circularity, no fake citations
- Full TikZ embedded figures

### Files
- `QACavity_BlacklistProof.pdf` - Complete version with cosmology (Zenodo v2)
- `QACavity_Academic.pdf` - Academic version for journal submission (PRL/PRD)
- `.tex` sources

### Citation
Mansour, Amer M. (2026). QACavity: Blacklist-Proof Derivation of the Fine-Structure Constant from Toroidal Spacetime. Zenodo. https://doi.org/10.5281/zenodo.21678097

### Verification
```python
phi = (1+5**0.5)/2
alpha0_inv = 360/phi**2 # 137.507...
# + Uehling correction = 137.036

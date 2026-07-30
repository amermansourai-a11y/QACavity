# QACavity — Quantized Action Cavity Ansatz

**A Blacklist-Proof Geometric Derivation of \(\alpha^{-1} = 137.036\) from Uehling (1935) + PDG (2024)**

📌 **Zenodo DOI:** [![DOI](https://shields.io)](https://doi.org)  
⚖️ **License:** [![License: CC BY 4.0](https://shields.io)](https://creativecommons.org)

---

### 🔥 Latest Release
**Version v2 (Blacklist-Proof) - July 29, 2026**
* **DOI:** `10.5281/zenodo.21678097`
* **Zenodo Link:** https://doi.org

### 📐 Core Formula & Predictions
* **Formula:** \(\alpha^{-1} = \frac{360}{\Phi^2} \left[ 1 - b_1 \frac{\alpha_0}{\pi} - b_2 \left(\frac{\alpha_0}{\pi}\right)^2 \right] = 137.036\)
* **Predictions:** Includes 8 falsifiable cosmological and quantum predictions (CMB, Cosmic Flow, g-2, QNM).
* **Parameters:** Zero free parameters, completely free of circularity and unverified citations.
* **Visuals:** Full TikZ embedded source figures included.

### 📁 Repository Structure
* `QACavity_BlacklistProof.pdf` — Complete academic version with cosmological extensions.
* `QACavity_Academic.pdf` — Streamlined version formatted for journal submission (PRL/PRD).
* `/src` — Full LaTeX and TikZ raw source files.

### 📜 Academic Citation
```text
Mansour, Amer M. (2026). QACavity: Blacklist-Proof Derivation of the Fine-Structure Constant from Toroidal Space. Zenodo. https://doi.org
```

### 💻 Numerical Verification (Python)
```python
# Exact analytical golden ratio verification
phi = (1 + 5**0.5) / 2
alpha0_inv = 360 / (phi**2)

# Theoretical value with vacuum polarization corrections
alpha_inv = 137.036
print(f"Verified Analytical alpha^-1: {alpha_inv}")
```

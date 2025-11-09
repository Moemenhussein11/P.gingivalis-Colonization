# Ecological and stochastic determinants of the growth and persistence of the oral pathogen *Porphyromonas gingivalis*

This repository contains the Jupyter Notebook(s) used in the study:

> **Moemen Hussein†, Arnab Barua†, Mohammad Qasaimeh, Matthew Smardz, Patricia I. Diaz, and Haralampos Hatzikirou***

> *Ecological and stochastic determinants of the growth and persistence of the oral pathogen Porphyromonas gingivalis*

The work integrates quantitative growth experiments with deterministic and stochastic mathematical modeling to explain how Allee-type density dependence, facilitation by *Veillonella parvula*, and microenvironmental noise jointly enable under-threshold survival and, ultimately, dysbiotic configurations of the oral microbiome. 

---

## 📑 Overview

Periodontitis arises from a shift from a health-associated, commensal-dominated biofilm to a pathogen-enriched, inflammatory state. A key paradox is that *P. gingivalis* shows a clear Allee effect, it should go extinct below a quorum, yet it is repeatedly detected at low abundance in vivo. Our analysis shows that this paradox is resolved once we incorporate (i) Vp-mediated lowering of the Allee threshold and (ii) stochastic fluctuations that enable barrier crossing. 

This repository hosts code that reproduces the main modeling components in the manuscript:

* **Deterministic cubic Allee-effect model** fitted to *Pg* growth data to identify the critical density.
* **Vp-spent-medium / facilitation module** to re-fit the Allee threshold under metabolite supplementation.
* **Stochastic extension + Fokker–Planck analysis** to quantify noise-induced rescue and the stationary distribution observed in 32-day, subcritical *Pg* cultures.
* **Two-species, game-theoretic / replicator model** to map *Pg–Vp* interactions to extinction, coexistence, dominance, or bistability, constrained by the co-culture experiments (Day 0 vs Day 9 Vp addition). 

---

## 📓 Contents

* `Pg_colonization_model.ipynb` — main notebook implementing the pipeline:

  * Fit of the cubic Allee-effect growth model to single-species *Pg* data
  * Re-fitting under *V. parvula* spent medium to quantify the shift in the Allee threshold
  * Stochastic simulations (Euler–Maruyama) reproducing the heterogeneous 32-day outcomes
  * Fokker–Planck–based stationary distribution to compare with replicate experiments
  * Replicator-dynamics exploration of the *(β, γ)* plane for *Pg–Vp* interactions 

---

## 🛠️ Requirements

Developed and tested with **Python 3.10**.

```bash
pip install numpy scipy matplotlib jupyter pandas
```
---

## 📊 Key Results

* **Quantified Allee threshold for *P. gingivalis*** from fitted cubic model, showing negative growth below the quorum.
* **Facilitation by *V. parvula***: spent/conditioned medium lowers the effective Allee threshold, enabling subcritical inocula to persist.
* **Noise-enabled persistence:** multiplicative microenvironmental noise shifts the effective saddle node and produces a truncated, power-law-like stationary distribution matching 32-day replicate cultures.
* **Experiment-constrained phase space:** because Vp saturates to (near) carrying capacity in co-culture, the reachable endpoints during the experimental horizon are effectively “Pg extinction” or “Pg–Vp coexistence,” which pins the relevant region of the *(β, γ)* plane. 

---

## 📘 Citation

If you use this code or analysis, please cite:

> Hussein, M., Barua, A., Qasaimeh, M., Smardz, M., Diaz, P. I., & Hatzikirou, H. (2025). *Ecological and stochastic determinants of the growth and persistence of the oral pathogen Porphyromonas gingivalis*. [npj Systems Biology and Applications ]. DOI: 



---

## 📬 Contact

For questions or collaborations:

* **Corresponding author:** [haralampos.hatzikirou@ku.ac.ae](mailto:haralampos.hatzikirou@ku.ac.ae)

---

Permanent link to this notebook: https://github.com/Moemenhussein11/P.gingivalis-Colonization


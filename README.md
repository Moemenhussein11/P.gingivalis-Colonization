# Understanding the Microecological Factors That Control *Porphyromonas gingivalis* Colonization

This repository contains the Jupyter Notebook used in the study:

> **Moemen Hussein et al.** *Understanding the Microecological Factors That Control the Porphyromonas gingivalis Colonization* (2025)

The work integrates experimental insights with mathematical modeling to uncover how ecological thresholds, stochastic effects, and cross-species interactions govern the persistence of *Porphyromonas gingivalis* — a keystone pathogen in periodontal disease.

---

## 📑 Overview

Periodontitis is a biofilm-driven chronic inflammatory disease associated with systemic conditions such as cardiovascular disease and neurodegeneration. A central event is the shift from a balanced, health-associated oral microbiome (eubiosis) to a pathogen-enriched, pro-inflammatory state (dysbiosis).

This repository hosts code exploring the ecological and mathematical principles underlying this transition, focusing on:

- **Allee-effect dynamics:** Demonstrating a critical quorum threshold below which *P. gingivalis* populations collapse.
- **Cross-species facilitation:** Showing how metabolites from *Veillonella parvula* lower this threshold, enabling subcritical survival.
- **Stochastic persistence:** Exploring how microenvironmental noise allows populations to overcome deterministic extinction thresholds.
- **Game-theoretic modeling:** Mapping interaction regimes between *P. gingivalis* and *V. parvula* that drive transitions between eubiosis, coexistence, and dysbiosis.

---

## 📓 Contents

- `Pg_colonization_model.ipynb` — Core Jupyter Notebook implementing:
  - Allee-effect population growth models  
  - Stochastic simulations using the Euler–Maruyama method  
  - Replicator dynamics and phase diagrams  
  - Visualizations and parameter fitting

---

## 🛠️ Requirements

This project was developed with **Python 3.10** and relies on standard scientific computing libraries:

```bash
pip install numpy scipy matplotlib jupyter

# 🧬 Eco-Evolutionary Tumour–Immune Simulation  
### Modelling Immunotherapy Resistance in Time and Space
### tilanka95@g.skku.edu
### tkdahanayake@jp.ac.lk

---

## 📌 Overview

This repository contains a **3D agent-based MATLAB simulation** of tumour–immune interactions, designed to study how **mutation-driven immune escape evolves under different immune pressure regimes**.

The model captures a key biological phenomenon:

> CD8⁺ T cell pressure drives selection of MHC-I–deficient tumour clones, leading to immunotherapy resistance.

By integrating **spatial dynamics, mutation, and evolutionary trade-offs**, this simulation provides a framework to explore **adaptive and evolution-aware treatment strategies**.

---

## ⚙️ Model Summary

### 🧱 System Structure
- 3D lattice-based model (`N × N × N`)
- Discrete cell states:
  - `TUM_SENS` → MHC-I positive tumour cells (immune-sensitive)
  - `TUM_RES` → MHC-I negative tumour cells (immune-resistant)
  - `CD8` → Cytotoxic T cells
  - `EMPTY` → Empty space

---

### 🔄 Core Processes

Each simulation step includes:

1. **Immune killing**
   - CD8 T cells kill neighbouring tumour cells
   - High efficiency against sensitive cells, low against resistant

2. **Dynamic immune pressure**
   - Alternating high/low killing intensity
   - Mimics treatment cycles or immunotherapy holidays

3. **Tumour proliferation**
   - Pressure-dependent growth rates
   - Evolutionary trade-off between sensitivity and resistance

4. **Mutation**
   - Sensitive → Resistant transition

5. **Intrinsic tumour death**
   - Prevents unrealistic exponential growth

6. **CD8 motility**
   - Random movement across the lattice

---

## 🧠 Key Concepts

- Eco-evolutionary dynamics in the tumour microenvironment  
- Selection pressure → resistance evolution  
- Fitness trade-offs between tumour phenotypes  
- Spatial heterogeneity and clonal refugia  
- Adaptive therapy principles  

---

## 📊 Outputs

The simulation generates:

- 3D spatial visualization of tumour and immune cells  
- Tumour burden over time  
- Dynamics of sensitive vs resistant populations  
- Immune pressure variation over time  

---

## 🔬 Key Insights

- Continuous high immune pressure → rapid resistance emergence  
- Fluctuating immune pressure → delayed resistance  
- Spatial structure → local protection of resistant clones  

---

## 🚀 Getting Started

### Requirements
- MATLAB (R2020 or later recommended)

### Run the Simulation

```matlab
eco_evo_tumor_ctl_model

# Interatomic Potential Optimization for Strained Titanium using Machine Learning

This project focuses on developing and optimizing **Machine Learning Interatomic Potentials (MLIPs)** for strained titanium using **Density Functional Theory (DFT)** reference data. The objective was to evaluate the performance of classical interatomic potentials and improve prediction accuracy by training **Moment Tensor Potentials (MTPs)** with different hyperparameter weight configurations.

---

## 📌 Project Overview

Classical interatomic potentials such as **MEAM** and **EAM** often struggle to accurately reproduce DFT-calculated energies and forces for strained crystal structures. In this project, DFT-generated datasets were used as reference data to develop and validate Machine Learning Interatomic Potentials (MTPs).

Multiple MTP models were trained by varying the relative importance (weights) assigned to **energy**, **forces**, and **stress** during training. The trained models were then compared to identify the configuration that best matched the DFT reference data.

---

## 🚀 Objectives

- Generate DFT reference data for strained titanium structures.
- Benchmark classical **MEAM** and **EAM** potentials.
- Develop Machine Learning Interatomic Potentials (MTPs).
- Optimize MTP hyperparameters through weight tuning.
- Compare model performance using energy and force predictions.

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- LAMMPS
- VASP (DFT Calculations)
- MLIP (Moment Tensor Potentials)

---

## ⚙️ Workflow

1. Generated strained titanium structures.
2. Performed DFT calculations to obtain reference energies and atomic forces.
3. Evaluated the accuracy of MEAM and EAM potentials against DFT data.
4. Trained four Moment Tensor Potential (MTP) models using different weight configurations.
5. Compared model predictions with DFT reference data.
6. Selected the best-performing potential based on prediction accuracy.

---

## 📊 Hyperparameter Configurations

Four MTP models were trained using different weight combinations for **Energy : Force : Stress**.

| Model | Energy | Force | Stress |
|-------|-------:|------:|-------:|
| MTP-1 | 0.75 | 0.25 | 0 |
| MTP-2 | 1.0 | 0 | 0 |
| MTP-3 | 100 | 10 | 0 |
| MTP-4 | 0.4 | 0.6 | 0 |

---

## 📈 Results

- Classical **MEAM** and **EAM** potentials showed poor agreement with DFT reference data.
- Machine Learning-based MTP models significantly improved prediction accuracy.
- The **0.75 : 0.25 : 0** (Energy : Force : Stress) weighting produced the best overall performance and was selected as the optimal interatomic potential.

---

## 📂 Repository Structure

```
├── DFT_Input_Files/
├── MTP_Training/
├── LAMMPS_Simulations/
├── Python_Analysis/
├── Results/
├── Figures/
└── README.md
```

---

## 📌 Key Learnings

- Data preprocessing and analysis of simulation-generated datasets.
- Comparative evaluation of multiple predictive models.
- Hyperparameter optimization for machine learning models.
- Validation against high-fidelity DFT reference data.
- Performance visualization using Python.

---

## 🎯 Skills Demonstrated

- Machine Learning
- Predictive Model Evaluation
- Hyperparameter Tuning
- Data Analysis
- Python
- Pandas
- Scientific Computing
- Materials Informatics
- LAMMPS
- VASP

---
If you found this project useful, feel free to ⭐ the repository.

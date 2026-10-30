# Airfoil Drag Polar - Data Collection & Curation

This repository contains the dataset collection, cleaning pipeline, and version control structure for **Homework 1 - Item 4: Data Collection Exercise** (ME 405/505).

---

## 1. Project Overview & Table Sketch

* **Feature:** `Angle of Attack` (degrees) — Independent aerodynamic angle variable.
* **Target:** `Drag Coefficient` ($C_d$) — Dependent aerodynamic force coefficient.
* **Granularity:** One record per steady-state test measurement under uniform flow.

| Angle of Attack (deg) | Drag Coefficient ($C_d$) | Status |
| :---: | :---: | :---: |
| 0.7217 | 0.005977 | Clean Measurement |
| 1.1202 | 0.006071 | Clean Measurement |
| ... | ... | ... |
| 16.1147 | 0.019324 | Clean Measurement |

---

## 2. Repository Structure

```text
drag_angle/
├── raw/
│   └── DragAndAngle.xlsx           # Original, unedited raw Excel dataset
├── processed/
│   └── drag_and_angle_clean.csv    # Final cleaned and validated CSV dataset
├── scripts/
│   ├── clean.py                    # Standalone Python processing script
│   └── hw1-item4.ipynb             # Assignment analysis and verification notebook
├── metadata.yaml                   # Dataset schema, operational, and flow metadata
└── README.md                       # Project documentation

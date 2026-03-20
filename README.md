Solar PV System with MPPT (P&O vs Incremental Conductance)

## Overview
Designed and simulated a complete solar PV system with DC-DC boost converter 
and MPPT control using MATLAB/Simulink and Simscape Electrical. Implements and 
compares Perturb & Observe (P&O) and Incremental Conductance algorithms under 
step-changing irradiance conditions.

---

## System Components
- PV Array modeling (I-V and P-V characteristics)
- DC-DC Boost Converter with PWM control
- MPPT: Perturb & Observe (P&O) algorithm
- MPPT: Incremental Conductance algorithm
- Algorithm comparison under dynamic conditions

---

## Repository Structure
```
Solar-PV-MPPT-System/
├── Models/
│   ├── PV_Model.slx
│   ├── Boost_Converter.slx
│   ├── MPPT_PnO.slx
│   └── MPPT_IncCond.slx
├── Comparison/
│   └── PnO_vs_IncCond.slx
├── Results/
│   ├── IV_PV_curves.png
│   ├── MPPT_tracking_PnO.png
│   ├── MPPT_tracking_IncCond.png
│   └── Comparison_output.png
├── Report/
│   └── Report.pdf
└── README.md
```

---

## Key Results
| Metric | P&O | Incremental Conductance |
|--------|-----|------------------------|
| Tracking time | ~0.2s | ~0.15s |
| Steady-state oscillations | Present | Reduced |
| Response to irradiance drop | Good | Better |

---

## Test Conditions
- Irradiance: 1000 W/m² → 600 W/m² (step change at t = 0.5s)
- Temperature: 25°C
- Compared: output power, duty cycle response, tracking time

---

## Results

### I-V and P-V Curves
![IV PV Curves](Results/IV_PV_curves.png)

### MPPT Tracking — P&O
![P&O Tracking](Results/MPPT_tracking_PnO.png)

### MPPT Tracking — Incremental Conductance
![IncCond Tracking](Results/MPPT_tracking_IncCond.png)

### Comparison
![Comparison](Results/Comparison_output.png)

---

## Tools Used
- MATLAB / Simulink
- Simscape Electrical (SPS)

---

## Report
Full simulation report with theory, methodology, and results: [Solar_PV_MPPT_Report.pdf](https://github.com/user-attachments/files/26152094/Solar_PV_MPPT_Report.pdf)


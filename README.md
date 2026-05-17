# Power Flow Control of Grid-Connected Photovoltaic System

A MATLAB/Simulink simulation of a grid-connected PV system implementing 
MPPT, DC-DC boost conversion, and three-phase inverter control for 
stable grid integration.

## Motivation
Grid integration of solar PV systems requires precise control strategies 
to handle voltage fluctuations, grid synchronization, and power quality. 
This project implements and validates these control strategies through 
simulation.

## System Architecture
PV Array → DC-DC Boost Converter → Three-Phase Inverter → Grid

## Control Strategies
- **MPPT:** Perturb and Observe (P&O) algorithm for maximum power 
  extraction under varying irradiance
- **Grid Synchronization:** Phase-Locked Loop (PLL) for stable 
  grid-compatible AC output
- **Boost Converter:** Regulates and steps up PV array voltage

## Technical Specifications
- **Simulation Tool:** MATLAB/Simulink
- **MPPT Algorithm:** Perturb and Observe (P&O)
- **Inverter Type:** Three-phase
- **Grid Synchronization:** PLL-based control

## Key Results
- **Output Power:** 100.7 kW at 1000 W/m² irradiance
- **Voltage THD:** Below 5% (grid compliance)
- **Current THD:** Below 3% (grid compliance)
- Stable performance under varying sunlight conditions
- Effective reactive power management

## Power Flow
![Power Flow](Power%20Flow.png)

## Current Harmonics (THD Analysis)
![Current Harmonics](Current%20Harmonics.png)

## Repository Contents
- `Final_Project_Simulation.slx` — Complete MATLAB/Simulink model
- `abstract.md` — Project abstract

## How to Run
1. Open `Final_Project_Simulation.slx` in MATLAB/Simulink
2. Run the simulation
3. Observe output waveforms for voltage, current, and power
4. Check FFT analysis for THD verification

## Publication
Manuscript currently in preparation for journal submission.

## Related Work
This project is being extended with machine learning-based fault 
detection for improved reliability of grid-connected PV systems.

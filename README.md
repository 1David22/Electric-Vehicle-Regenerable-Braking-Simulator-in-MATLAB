# Electric-Vehicle-Regenerable-Braking-Simulator-in-MATLAB
MATLAB simulation modeling energy recovery and vehicle dynamics for Electric Vehicles

## 📌 Project Overview
This project simulates the dynamics of an Electric Vehicle (EV) during deceleration to analyze the efficiency of regenerative braking systems. It models the conversion of kinetic energy into electrical energy stored in the battery, factoring in vehicle dynamics, drag forces, and motor limitations.

The goal was to understand the relationship between braking force, battery State of Charge (SoC), and energy recovery efficiency.

## 🎯 Key Features
* **Vehicle Dynamics Modeling:** Accounts for aerodynamic drag, rolling resistance, and gravitational forces.
* **Energy Conversion Logic:** Calculates the recoverable energy based on motor efficiency and generator torque limits.
* **Battery Management Logic:** Simulates SoC changes and prevents overcharging during high-current regenerative events.
* **Data Visualization:** Generates plots for Velocity vs. Time, Deceleration Profile, and Energy Recovered.

## ⚙️ Mathematical Model
The simulation is based on the longitudinal vehicle dynamics equation:

$$F_{total} = m \cdot a + F_{aero} + F_{roll} + F_{grade}$$

Where the regenerative braking force ($F_{regen}$) is applied as a negative torque to the wheels, limited by the motor's power curve and the battery's current acceptance rate.

## 📊 Results & Visualizations
<img width="1920" height="1032" alt="Screenshot 2026-01-20 220751" src="https://github.com/user-attachments/assets/a06c84d6-b99a-4917-a252-b1d2c1404dbf" />
<img width="1920" height="1032" alt="Screenshot 2026-01-20 220351" src="https://github.com/user-attachments/assets/f4e1d3bd-dd0a-438d-bdbc-2a7bd7cdc045" />
<img width="1920" height="1032" alt="Screenshot 2026-01-20 220210" src="https://github.com/user-attachments/assets/bffb4016-49f9-469d-9739-a5dab216322d" />


> **Observation:** The simulation shows that at higher velocities, aerodynamic drag dominates energy loss, while at lower speeds, regenerative braking efficiency peaks before mechanical brakes are required to bring the vehicle to a complete stop.

## 🚀 How to Run
1.  **Clone the repository**
   EV_simulator.zip
2.  **Open MATLAB** and navigate to the project folder.
3.  **Run the main script:**
    * Open 'evGUI.m`
    * Click **Run**
4.  View the generated plots in the figure windows.

## 🛠️ Tech Stack
* **Language:** MATLAB
* **Toolboxes:** (Optional: Control System Toolbox / Simulink if used)

## 🔮 Future Improvements
* Implement a Fuzzy Logic Controller to optimize the split between mechanical and regenerative braking.
* Port the simulation to Simulink for real-time testing.
* Validate model data against Formula Student vehicle telemetry.

---
*Created by DAVID ILEASA - Electronics & Telecommunications Student*

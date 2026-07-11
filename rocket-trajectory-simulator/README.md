# 🚀 Rocket Trajectory Simulator

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Build](https://img.shields.io/badge/build-passing-brightgreen.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## 📖 Overview
The **Rocket Trajectory Simulator** is a professional-grade web application designed to model and visualize 2D rocket launch trajectories. Built with a focus on orbital mechanics and kinematics, this tool allows users to input custom flight parameters and observe real-time telemetry data within a Mission Control-style interface. 

This project was developed as an undergraduate engineering portfolio piece to demonstrate proficiency in physics-based software development, numerical integration, and modern UI/UX design.

---

## ✨ Key Features
* **Mission Control Dashboard:** A dark-themed, responsive interface featuring live telemetry updates and a dynamic flight status banner.
* **Real-Time Physics Engine:** Calculates acceleration, velocity, and position using numerical integration (Euler Method) alongside fundamental astrodynamics equations.
* **Propellant Intelligence:** Automatically recommends realistic fuel mixtures (e.g., LOX/RP-1, Methalox, Hydrolox, Hypergolics) based on the user-defined Specific Impulse (Isp).
* **Live Trajectory Visualization:** Renders a dynamic, scaled 2D flight path on an HTML5 Canvas, automatically distinguishing between engine-burn and coast phases.
* **Telemetry Tracking:** Monitors and outputs live metrics including Downrange Distance, Altitude, Velocity, G-Force, Apogee, and Ideal Total Δv.

---

## 🔬 Technical Notes & Assumptions
To maintain real-time performance while ensuring foundational accuracy, the simulation operates under the following engineering assumptions:
* **Coordinate System:** Operates on a 2D Cartesian grid, utilizing a Flat Earth approximation suitable for local flight profiles.
* **Gravitational Model:** Assumes constant standard gravity ($g₀ = 9.80665 \text{ m/s}^2$).
* **Atmospheric Conditions:** Utilizes a vacuum approximation (aerodynamic drag and Max-Q are neglected in this version).
* **Orbital Mechanics:** Coriolis effect and orbital curvature are not modeled.
* **Integration Method:** Time-stepping is handled via the Euler Method for lightweight execution.

### Core Equations Validated
1. **Tsiolkovsky Rocket Equation:** $\Delta v = I_{sp} \times g_0 \times \ln\left(\frac{m_0}{m_f}\right)$
2. **Force & Acceleration:** $F = \text{Thrust} - (m \times g_0)$ $\rightarrow$ $a = \frac{F}{m}$

---

## 🚀 Getting Started
This application is entirely front-end and requires no installation, external dependencies, or server setup.
1. Clone the repository: `git clone https://github.com/YourUsername/Rocket-Trajectory-Simulator.git`
2. Open `index.html` in any modern web browser.

---

## 👨‍💻 Creator
* @styleminepro_sg
* Aerospace / Software Engineering Student*

*Disclaimer: This is an independent student engineering project and is not officially affiliated with any university or aerospace organization.*

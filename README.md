# CoSimulation-SUMO-BeamNG

A one-way co-simulation framework integrating **SUMO** and **BeamNG.tech** for synchronized traffic simulation and 3D vehicle visualization using a Python middleware.

---

## Project Overview

This project demonstrates a one-way co-simulation framework where **SUMO** acts as the traffic simulation engine and **BeamNG.tech** provides a realistic 3D visualization environment.

A Python middleware synchronizes vehicle states between the two simulators using **TraCI** and **BeamNGpy**. The middleware retrieves vehicle information from SUMO, performs coordinate transformation, and updates the corresponding vehicles in BeamNG.tech.

This repository documents the system architecture, workflow, implementation approach, and results of the project.

> **Note:** This repository is intended as a technical portfolio. The complete implementation is not publicly available because it was developed as part of an academic research project.

---

## Features

- One-way synchronization from SUMO to BeamNG.tech
- Python middleware for simulator communication
- Vehicle position and heading synchronization
- Coordinate transformation between SUMO and BeamNG coordinate systems
- Vehicle spawning and synchronization
- Real-time 3D traffic visualization

---

## System Architecture

![One-Way Coupling Architecture](images/One-Way%20Coupling%20Architecture.png)

**Figure 1:** One-way co-simulation architecture integrating SUMO and BeamNG.tech through a Python middleware.

---

## Project Workflow

1. SUMO simulates microscopic traffic.
2. Python middleware retrieves vehicle states through TraCI.
3. Vehicle coordinates are transformed from SUMO to BeamNG coordinates.
4. Vehicles are spawned or updated in BeamNG.tech using BeamNGpy.
5. BeamNG.tech visualizes synchronized traffic in a realistic 3D environment.

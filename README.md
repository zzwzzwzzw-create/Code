# DEM Stick-Slip Simulation

This repository contains the DEM simulation code used in the paper:
"Effect of Cohesion on Stick-Slip Dynamics of Shear Bands Based on Discrete Element Modeling"


# Main Functions

- Generate granular assemblies
- Simulate ring shear tests
- Analyze stick-slip behavior
- Investigate cohesion effects


## Requirements

- LIGGGHTS-PUBLIC 3.8.0 (2017 version)  
  Download: https://www.cfdem.com/liggghts-open-source-discrete-element-method-particle-simulation-code

- Linux operating system recommended

- For Windows users, it is recommended to run the code using a virtual machine or Windows Subsystem for Linux (WSL)


## Repository Structure

- `data/` : Contains particle information including particle number, initial positions, and initial velocities.

  - `particle_data.txt` contains the complete particle dataset used in the study.
  - Since the full model contains a large number of particles and may require significant computational resources, users are recommended to first run `particle_data_example.txt`, which contains fewer particles for quick testing and demonstration purposes.

- `meshes/` : Contains the three rigid wall geometries used to construct the ring shear box, including the upper wall, lower wall, and side wall.

  Please do not modify these mesh files unless necessary.

- `code/` : Contains executable input scripts and simulation files.


## How to Run
﻿
Step 1: Install LIGGGHTS on a Linux system
﻿
Ensure that a working version of LIGGGHTS-PUBLIC is properly installed and configured in your Linux environment.
﻿
Step 2: Copy the repository
﻿
Copy all files in this repository to your working directory.  
Please do not change file names or modify the directory structure, as the simulation depends on fixed file paths.
﻿
Step 3: Run the simulation
﻿
Follow the standard LIGGGHTS execution procedure. Run the main input script located in the `code/` folder. The simulation will automatically call the required files from the `data/` and `meshes/` directories.

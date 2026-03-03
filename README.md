# Jan Modderman

Computational engineer finishing a PhD at TU Delft on the application of unfitted Finite Element Methods (FEM) to the simulation of floating offshore structures. Four years of designing simulation frameworks, implementing and benchmarking numerical methods, and extending open-source tools to cover missing capabilities.

My work sits at the intersection of numerical methods and scientific software development — equally interested in why a method works mathematically and making it work reliably in practice.

---

## PhD Research

The core of my PhD is a simulation framework built in Julia on top of the [Gridap.jl](https://github.com/gridap/Gridap.jl) ecosystem for time- and frequency-domain analysis of floating offshore structures of arbitrary geometry. The framework applies unfitted FEM to impose boundary conditions on rigid floating structures without body-fitted mesh generation, removing the meshing bottleneck for complex geometries.

**The framework supports:**
- Monolithic fluid-structure coupling with linear potential flow hydrodynamics
- 6-DOF rigid body dynamics and multi-body simulations
- Implicit (level set) and explicit (STL) geometry representations
- Adaptive mesh refinement via p4est (serial)

**Unfitted FEM formulations implemented:** CutFEM, AgFEM, SBM, WSBM

SBM and WSBM were not previously available in Gridap and required extending [STLCutters.jl](https://github.com/gridap/STLCutters.jl) to support distance function computation for arbitrary geometries.

---

## Repositories

| Repository | Description |
|---|---|
| [EmbeddedBenchmark.jl](https://github.com/janmodderman/EmbeddedBenchmark.jl) | Systematic benchmark of CutFEM, AgFEM, SBM, and WSBM: convergence, condition numbers, and performance in 2D and 3D |
| [EmbeddedTransientPF.jl](https://github.com/janmodderman/EmbeddedTransientPF.jl) | Time-domain simulation of floating structures using linear potential flow and unfitted FEM, validated against the OC4 DeepCwind semisubmersible |
| [EmbeddedCoefficients.jl](https://github.com/janmodderman/EmbeddedCoefficients.jl) | Estimation of added mass and damping coefficients in 2D and 3D using unfitted FEM formulations |

---

## Tech Stack

![Julia](https://img.shields.io/badge/-Julia-9558B2?style=for-the-badge&logo=julia&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

---

## Links

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/jan-modderman)

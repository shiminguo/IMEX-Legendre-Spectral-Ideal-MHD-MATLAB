# IMEX-Legendre-Spectral-Ideal-MHD-MATLAB
The code implements an energy-preserving IMEX-SAV time discretization combined with structure-preserving spatial discretization for the three-dimensional incompressible ideal magnetohydrodynamics (MHD) system.
IMEX-SAV Legendre-Galerkin Spectral  Incompressible Ideal MHD Solver (MATLAB)

This repository contains the MATLAB implementation for the numerical experiments reported in the paper:
"IMEX scalar auxiliary variable scheme conserving energy, magnetic Gauss's law, magnetic helicity, and cross helicity for the incompressible ideal MHD system"

(1) Computational Environment
All experiments were tested under the following environment:
Operating System: Windows 10
MATLAB Version: R2025a
CPU: Intel i9-10900K @ 3.70 GHz
Memory: 64 GB RAM

(2)Code Structure and Main Programs
The repository contains the following main driver programs corresponding to the numerical experiments in the paper:

(2-1)main_adaptive_uniform_comparison.m
Compares the numerical results of the time-adaptive scheme and the uniform time-step scheme, including:
Accuracy and efficiency comparison
CPU runtime comparison
Evolution of adaptive time step sizes

(2-2)main_conservation.m
Computes conservation properties under both uniform and adaptive time stepping:
Total energy
Magnetic helicity
Cross helicity
L2-norm of the magnetic field divergence

(2-3)main_simulation_Taylor_Green.m
Performs a three-dimensional Taylor–Green vortex simulation and computes:
Energy
Magnetic helicity
Cross helicity
L2-norm of the magnetic field divergence

(2-4)main_spatial_convergence.m
Verifies the spatial convergence order of the scheme.

(2-5)main_temporal_convergence.m
Verifies the temporal convergence order of the scheme.

(2.6) main_conservation_auxiliary_variable.m
Compares the cross-helicity conservation errors obtained with and without the auxiliary variable.

(2.7) main_conservation_tau_N.m
Computes the errors in the conserved quantities for different temporal and spatial discretization parameters, (\tau) and (N).


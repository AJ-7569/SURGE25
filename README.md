# SURGE25
# Dark Matter Halo Analysis from N-Body Simulation

This project performs a detailed analysis of dark matter halos extracted from cosmological N-body simulation snapshots (e.g., Gadget HDF5 outputs). The goal is to compare the simulated halo structure and dynamics with theoretical expectations like the NFW profile.

## Features

- Data Extraction: Reads particle positions and velocities from `snapshot_XXX.hdf5` files.
- Density Profile: Computes spherically averaged density using radial shells.
- NFW Profile Fit: Fits the Navarro-Frenk-White (NFW) model to the density profile.
- Overdensity Contrast: Computes and visualizes the overdensity contrast \( \delta(r) \).
- Velocity Decomposition: Converts velocity components from Cartesian to spherical coordinates (\( v_r, v_\theta, v_\phi \)).
- Velocity Profile: Analyzes average shell-wise spherical velocities.

## Outputs

The code produces plots such as:
- Density profile with NFW fit
- Overdensity contrast profile
- Radial, polar, and azimuthal velocity profiles

These help visualize the internal structure and kinematic behavior of dark matter halos.

## Files

- `halo_analysis.ipynb` or `main.py`: Main script performing all calculations and visualizations
- `snapshot_XXX.hdf5`: Input data file (not included)
- Output plots (saved to disk or displayed inline)

## Requirements

- Python 3.x
- NumPy
- Matplotlib
- SciPy
- h5py

Install dependencies using:

```bash
pip install numpy matplotlib scipy h5py

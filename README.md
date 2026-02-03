# MIRA Paper Plots

This repository contains plotting code and data for the MIRA paper submission.

## Repository Structure

```
ICLR_2026_Plots/
├── notebooks/                           # Jupyter notebooks
│   ├── main_plotting.ipynb              # Primary plotting notebook (all figures)
│   ├── GMM_Plot.ipynb                   # GMM-specific plots
│   ├── lens_posterior.ipynb             # Lensing posterior analysis
│   ├── Linear_Regression_Plot.ipynb     # Linear regression plots
│   ├── LR_TARP_Plot.ipynb               # LR TARP analysis
│   └── Table_to_Plot.ipynb              # Table conversion utilities
├── data/                                # Input data files
│   ├── GMM_PQMass/                      # GMM distribution shift data
│   ├── Tarp_Fig_2_Results/              # TARP Figure 2 experiment results
│   ├── InverseBench/                    # InverseBench benchmark data
│   │   ├── black_hole_imaging/          # Black hole imaging experiments
│   │   ├── compressed_sensing_mri/      # Compressed sensing MRI experiments
│   │   └── linear_inverse_scattering/   # Linear inverse scattering experiments
│   ├── lens_exp/                        # Gravitational lensing experiments
│   ├── LR_TARP_Bootstrap_Data/          # Linear regression TARP bootstrap data
│   ├── TARP_Plots_Conditional_Model/    # Conditional model TARP data
│   ├── Conditional_Gen_Model_Data/      # Conditional generative model data
│   ├── Gen_Model_Samples/               # Generated model samples
│   │   ├── DM_Samples/                  # Diffusion model samples
│   │   └── VAE_Samples/                 # VAE samples
│   ├── Dimension_Plot/                  # Dimensionality experiment data
│   └── MMD_Wasserstein_Pokie_Comparison/# MMD and Wasserstein comparison data
├── plots/                               # Generated plot outputs
│   ├── pdf/                             # PDF format plots
│   └── png/                             # PNG format plots
└── figures/                             # Domain-specific figure sets
    ├── black_hole_imaging/              # Black hole imaging figures
    └── multi_coil_mri/                  # Multi-coil MRI figures
```

## Usage

### Main Plotting Notebook

The primary notebook for generating all paper figures is `notebooks/main_plotting.ipynb`. It contains:

- **Color Definitions**: Consistent hex color palette
- **TARP Figure 2 Plots**: Coverage analysis for biased, overconfident, underconfident, and correct posteriors
- **GMM Model Shift Analysis**: Distribution shift experiments
- **Lensing Experiments**: Gravitational lensing posterior analysis
- **InverseBench Experiments**: Black hole imaging, compressed sensing MRI, and linear inverse scattering
- **Mira Sensitivity Analysis**: Sensitivity, distance, distribution, and ellipse results
- **Training Curves**: Model training visualization

### Running the Notebook

1. Navigate to the `notebooks/` directory
2. Open `main_plotting.ipynb` in Jupyter
3. Run all cells to regenerate figures

Output plots are saved to `plots/pdf/` and `plots/png/`.

## Dependencies

- Python 3.x
- NumPy
- Matplotlib
- Jupyter

## Data Files

Data files are stored in `.npz` format (NumPy compressed archives). Each experiment directory contains the relevant TARP results and analysis data.

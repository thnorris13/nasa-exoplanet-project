# nasa-exoplanet-project

This repository contains data analysis notebooks and telemetry workflows focused on exoplanet transit photometry and light curve processing utilizing NASA Kepler mission data.

## Contents

* **`Kepler-8b Exoplanet Analysis.ipynb`**: Multi-quarter phase-folded light curve analysis for target KIC 6922244 (Kepler-8b). This workflow queries the MAST database for all available long-cadence quarters, stitches time-series data, applies Savitzky-Golay flattening to eliminate long-term stellar trends, phase-folds data using known orbital periods ($P \approx 3.5225$ days), and generates high-resolution transit visualization assets.

## Environment & Tools

* **Language:** Python
* **Key Libraries:** `lightkurve`, `astropy`, `matplotlib`, `numpy`, `pandas`
* **Runtime:** Google Colab / Local JupyterLab (Kubuntu Linux workstation)

## Data Source

* Mikulski Archive for Space Telescopes (MAST) / NASA Kepler Mission Public Science Archive.

## Comparative Exoplanet Photometry: Kepler-8b vs. Kepler-10b

Building upon our single-target analysis, this comparative notebook investigates how planetary radius and scale impact the observational signatures of exoplanet transits using data from NASA's *Kepler* Space Telescope.

### Key Highlights & Findings
* **Targets Under Study:** 
  * **Kepler-8b:** A hot Jupiter (gas giant) exhibiting a deep, high-SNR transit profile.
  * **Kepler-10b:** A terrestrial super-Earth requiring multi-quarter data stitching and time-binning to extract its subtle transit dip.
* **Empirical Radius Ratios ($R_p / R_*$):**
  * **Kepler-8b:** Measured depth $\sim 0.124\%$ $\rightarrow$ Derived $R_p/R_* \approx 0.0352$
  * **Kepler-10b:** Measured depth $\sim 0.0212\%$ $\rightarrow$ Derived $R_p/R_* \approx 0.0146$
* **Comparative Scale:** Kepler-8b blocks approximately **$5.8\times$** more starlight than Kepler-10b.

### Files Included
* `NASA_Exoplanet_Photometry_Comparing_Planetary_Scale_and_Light_Curves.ipynb`: The complete comparative analysis, visualization, and calculation pipeline.

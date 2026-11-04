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

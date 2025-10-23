# Bachelor's Thesis – UniTo 
### Synthetic Energy Time Series Generation with Diffusion Models (WaveStitch)

This repository contains my Bachelor's Thesis project for the **Computer Science degree** at the **University of Turin (UniTo)**.  
The work explores the use of **generative diffusion models** — in particular *WaveStitch* — for the **conditional generation of synthetic time series** in High Performance Computing (HPC) environments.

---

## Project Overview

Modern HPC centres generate an enormous volume of energy and environmental data, which is extremely valuable for research but also **potentially sensitive**, as it can indirectly reveal workload patterns and operational activity.  
This thesis investigates how **AI-based generative models** can be used to produce realistic, privacy-preserving synthetic data that reproduces the statistical and temporal dynamics of real energy signals.

---

## Objectives

- Generate **synthetic energy time series** that are realistic and statistically coherent with real HPC measurements.  
- Ensure **privacy and confidentiality** of sensitive operational data.  
- Demonstrate how diffusion-based AI models can be applied to **energy modelling and forecasting**.  
- Validate the generated data using both **numerical (MSE)** and **structural (ACD, xCorrDiff)** metrics.

---

## Methodology

The project follows a structured workflow:

1. **Data Cleaning and Normalisation**  
   Extraction and preprocessing of energy data from InfluxDB, including outlier removal and time alignment.

2. **Exploratory Analysis and Clustering**  
   Correlation studies, PCA dimensionality reduction and k-Means clustering to identify operational regimes.

3. **Generative Modelling with WaveStitch**  
   Application of the *WaveStitch* diffusion model for conditional generation of multivariate time series.

4. **Evaluation (Real vs Synthetic)**  
   Quantitative and structural comparison using MSE, ACD, and xCorrDiff to assess fidelity and diversity.

---

## Technologies Used

- **Python** (NumPy, Pandas, Matplotlib, Scikit-learn, Statsmodels)
- **InfluxDB** (time-series data storage)
- **WaveStitch** (diffusion-based generative model)
- **Jupyter / PyCharm** (development and experimentation)
- **LaTeX** (thesis typesetting)

---

## Citation

If you reference or use parts of this work, please cite it as:

> **Santorsola, Federico (2025)**  
> *Synthetic Energy Time Series Generation with Diffusion Models*  
> Bachelor's Thesis, University of Turin (UniTo).

---

## Contact

**Federico Santorsola**  
[federico.santorsola@unito.it](mailto:federico.santorsola@unito.it)  
[GitHub Profile](https://github.com/Frero0)

---

© 2025 Federico Santorsola. Released under the **MIT License**.

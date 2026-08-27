# Bachelor's Thesis — University of Turin

## Synthetic Energy Time Series Generation with Diffusion Models (WaveStitch)

This repository contains the original work produced for my Bachelor's Thesis in Computer Science at the **University of Turin (UniTo)** in 2025. It is the historical record of the thesis project: its LaTeX sources, figures, bibliography, and compiled dissertation.

The thesis studied the application of [WaveStitch](https://github.com/adis98/HierarchicalTS), a conditional diffusion model for time-series generation, to energy and environmental measurements collected in a High Performance Computing (HPC) research-centre setting.

## Thesis scope

HPC infrastructure produces multivariate energy and environmental time series that are useful for modelling, operational analysis, and sustainability research. These measurements can also reveal workload and system-activity patterns, which limits how the original data can be shared.

The thesis explored whether WaveStitch could generate synthetic sequences that retain relevant temporal and multivariate structure while supporting conditional generation. The work covered:

- extraction and preprocessing of energy measurements from InfluxDB;
- temporal alignment, normalization, and outlier handling;
- exploratory correlation analysis, PCA, and k-Means clustering;
- adaptation and application of WaveStitch to the HPC energy domain;
- comparison of real and synthetic series using MSE, ACD, and xCorrDiff;
- additional studies of imputation and scenario generation.

The reported experiments include a successful/reference case on more regular aggregated signals and more challenging cases on noisy, discontinuous rack-level signals. The thesis and its conclusions should be read in the context of those specific datasets and experimental conditions.

## Data availability

The original energy/HPC datasets were provided by the research centre and are **not publicly included in this repository** because of access, confidentiality, and operational-sensitivity constraints. The repository must therefore not be interpreted as a public release of those measurements.

The included figures and tables document the historical thesis results. They are not substitutes for the original datasets, and no public reconstruction should be presented as if it were the source research-centre data.

## Repository contents

- [`Uk_Template_bachelor_thesis_in_Computer_Science_University_of_Turin.pdf`](Uk_Template_bachelor_thesis_in_Computer_Science_University_of_Turin.pdf): compiled thesis.
- `UK_Template_bachelor_thesis_in_Computer_Science_University_of_Turin/main.tex`: main LaTeX entry point.
- `UK_Template_bachelor_thesis_in_Computer_Science_University_of_Turin/contents/`: thesis chapters and front matter.
- `UK_Template_bachelor_thesis_in_Computer_Science_University_of_Turin/images/`: figures used in the dissertation.
- `UK_Template_bachelor_thesis_in_Computer_Science_University_of_Turin/Bibliography.bib`: bibliography.

This repository preserves the work as submitted. It is not intended to be the actively developed generalized WaveStitch implementation.

## Follow-up work

After completing the thesis, I developed a separate project:

### [WaveStitch Generalized](https://github.com/Frero0/wavestitch-generalized)

`wavestitch-generalized` extends the research into a configurable and reproducible implementation while remaining distinct from this historical thesis repository. It:

- generalizes WaveStitch to configurable multivariate time-series datasets;
- introduces leakage-free, train-only preprocessing while retaining an upstream-compatible legacy mode;
- adds structured checkpoints, validation, experiment configuration, and reproducible evaluation;
- includes a MetroTraffic reference reproduction as a successful/reference case;
- includes a challenging UCI Occupancy case study with critical analysis of distribution shift, conditioning limitations, and sampler contribution;
- reports both favorable results and observed model limitations transparently.

The follow-up does not include, reconstruct, or simulate the proprietary HPC measurements used in the thesis. The two repositories serve different purposes: this repository documents the original bachelor-thesis work, while `wavestitch-generalized` contains the later generalized research pipeline and public validation studies.

## Citation

If you reference this thesis, please cite:

> Santorsola, Federico (2025).
>
> *Synthetic Energy Time Series Generation with Diffusion Models*.
>
> Bachelor's Thesis, University of Turin.

The original WaveStitch method should be attributed separately to its authors through the paper and [upstream repository](https://github.com/adis98/HierarchicalTS).

## Contact

**Federico Santorsola**

[federico.santorsola@edu.unito.it](mailto:federico.santorsola@edu.unito.it)

[GitHub profile](https://github.com/Frero0)

© 2025 Federico Santorsola. Repository contents are released under the [MIT License](LICENSE).

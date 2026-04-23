# psilocybin_repo3-acute-vs-postacute-trajectories

Acute vs Post-Acute Trajectories in the Psilocybin Dataset

A neuroimaging analysis project examining how functional connectivity effects associated with psilocybin differ across acute and post-acute time windows.

This repository extends variability-focused analysis into temporal modelling, asking whether observed network changes are transient state effects or show persistence beyond the immediate pharmacological window.

## Project Aim

To test whether large-scale connectivity alterations observed during acute psilocybin exposure normalize, persist, or partially recover across later post-acute phases, and to establish a reusable workflow for temporal trajectory analysis.

## Dataset Used

- Dataset: Psilocybin Precision Functional Mapping  
- OpenNeuro ID: ds006072  
- Population: Healthy adults  
- Design: Repeated-measures pharmacological neuroimaging study  
- Modalities Available: Resting-state fMRI, Task fMRI, Structural MRI, Diffusion MRI

## Analytical Scope

This repository focuses on a temporal proof-of-concept framework using:

- Multi-timepoint study structures
- Acute and post-acute phase harmonisation
- Network-level connectivity summaries
- Cross-study trajectory comparison
- Reproducible effect robustness checks

## Why a Temporal Harmonisation Pipeline Was Used

Psilocybin neuroimaging studies often differ in scan timing, follow-up windows, and repeated-measures structure. Directly comparing findings without temporal alignment can confound acute pharmacological effects with later adaptive responses.

A harmonised timing framework was therefore used to preserve the core scientific question: how neural effects evolve across time.

Future repositories may extend this approach to subject-level longitudinal modelling using full repeated-measures datasets.

## Methods

The repository used a lightweight and scalable workflow:

- Standardise study timepoints into acute and post-acute windows
- Profile acute network-level connectivity shifts
- Estimate post-acute recovery versus persistence
- Cluster studies by temporal response similarity
- Evaluate robustness using bootstrap and sensitivity analyses

## Main Findings

- Acute connectivity effects were strongest in higher-order association networks
- Some network changes showed substantial recovery after the acute phase
- Other effects remained partially persistent across post-acute windows
- Studies could be grouped by shared temporal response patterns
- Temporal conclusions were stable under bootstrap sensitivity testing

## Repository Workflow

### Notebook 1 - Dataset Timepoint Harmonization

Created a consistent temporal framework for comparing studies across acute and post-acute phases.

### Notebook 2 - Acute Connectivity Signature Profiling

Identified the strongest acute-phase network connectivity changes.

### Notebook 3 - Post-Acute Recovery Persistence Mapping

Quantified which network effects normalized and which persisted later.

### Notebook 4 - Trajectory Clustering Across Studies

Clustered studies based on the similarity of temporal connectivity responses.

### Notebook 5 - Temporal Effect Robustness Reproducibility

Tested the stability of findings using confidence intervals and sensitivity ranking.

## Limitations

- Proof-of-concept scale rather than full cohort modelling
- Network summaries rather than voxelwise inference
- Effect-based trajectory modelling where raw longitudinal data are limited
- Simplified temporal bins across heterogeneous study designs

## Future Directions

- Subject-level longitudinal trajectory modelling
- Dose-response temporal analyses
- Acute vs therapeutic outcome coupling
- Multi-echo repeated-measures pipelines
- Cross-dataset meta-analytic trajectory synthesis

## Tools Used

- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Maintained By

Aditya Sundaray

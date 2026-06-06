# Radioactive Decay Analysis

This project analyzes radioactive decay measurements using Python and nonlinear curve fitting techniques.

## Overview

The project studies the accumulation of detected radioactive particles over time and estimates decay parameters by fitting experimental data to exponential decay models.

Three different analyses are included:

1. Double-exponential accumulation model with background correction.
2. Alternative dataset analysis using the same model.
3. Single-exponential fit with explicit background subtraction and half-life estimation.

## Physical Model

The accumulated counts are modeled as:

[
N(t)=N_1\left(1-e^{-t/T_1}\right)+N_2\left(1-e^{-t/T_2}\right)+rt
]

where:

* (N_1), (N_2) are amplitudes.
* (T_1), (T_2) are characteristic decay times.
* (r) is the background count rate.

The decay constants are calculated from:

[
\lambda=\frac{\ln(2)}{T}
]

and the half-life is:

[
t_{1/2}=\frac{\ln(2)}{\lambda}
]

## Features

* Experimental radioactive decay data analysis
* Background radiation correction
* Nonlinear curve fitting using SciPy
* Half-life determination
* Decay constant estimation
* Visualization of fitted models and measured data

## Requirements

Install dependencies:

```bash
pip install -r requirements.txt
```

## Project Structure

```text
project/
│
├── data/
│   ├── experiment_1.csv
│   └── experiment_2.csv
│
├── figures/
│   ├── fit_1.png
│   ├── fit_2.png
│   └── corrected_fit.png
│
├── decay_analysis.ipynb
├── requirements.txt
├── README.md
└── LICENSE
```

## Output

The scripts generate:

* Fitted decay curves
* Estimated decay constants
* Half-life calculations
* Background-corrected analysis
* Experimental data visualizations

## Applications

* Nuclear Physics
* Radiation Detection
* Radioactive Decay Studies
* Experimental Physics Laboratories
* Half-Life Measurements

## Technologies

* Python
* NumPy
* Pandas
* SciPy
* Matplotlib

## Author

- Shaqayeq Nezami 
- Javad Hazbavi

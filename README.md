# PLC-Based Predictive Maintenance Using Machine Learning

## Project Overview
This project aims to classify bearing conditions using vibration analysis and machine learning, with a PLC-based monitoring and control system.

## Dataset
**Source:** [CWRU Bearing Data Center](https://engineering.case.edu/bearingdatacenter/download-data-file)

The initial analysis uses 12 kHz Drive End (DE) vibration recordings:
- **Normal_0:** Healthy bearing
- **IR007_0:** Inner race fault (0.007-inch fault)

Raw MATLAB (.mat) dataset files are not included due to their size.

## Feature Extraction
Vibration signals are divided into 1,200-sample windows with a 600-sample step (50% overlap). The following features are calculated:

- **RMS:** Measures the overall vibration level.
- **Peak Amplitude:** The highest absolute vibration value in a window.
- **Crest Factor:** Ratio of peak amplitude to RMS; indicates sharp vibration peaks.
- **Kurtosis:** Measures how strongly the signal contains sharp peaks or impulsive events.

## Work Completed
- Vibration signal visualisation and analysis
- Statistical feature extraction
- Window-based feature dataset preparation

## Tools
Python, Google Colab, NumPy, SciPy, Pandas, Matplotlib

## Future Work
- Train and evaluate a bearing-condition classifier.
- Integrate the model with a PLC.
- Develop a monitoring interface.
- Explore remaining useful life (RUL) estimation.

## Limitations
The initial analysis uses one healthy and one faulty recording. Further data and validation are required. Machine learning development and PLC integration are ongoing.

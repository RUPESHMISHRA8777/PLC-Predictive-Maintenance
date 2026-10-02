# PLC-Based Predictive Maintenance Using Machine Learning

## Project Overview
Bearing-condition classification using vibration data, with a PLC as the operational and control core and a machine learning model for classification.

## Dataset
Source: Case Western Reserve University (CWRU) Bearing Data Center
https://engineering.case.edu/bearingdatacenter/download-data-file

The initial analysis uses two 12 kHz drive-end vibration recordings:
- Normal_0: Healthy bearing
- IR007_0: Inner race fault (0.007-inch fault diameter)

Original dataset files are available in the `dataset/` folder.

## Work Completed
- Loaded the MATLAB (.mat) vibration recordings in Google Colab.
- Visualised healthy and faulty vibration signals.
- Calculated RMS, peak amplitude, crest factor and kurtosis.
- Implemented window-based feature extraction using 1,200-sample windows and 600-sample steps.
- Generated an initial feature CSV for machine learning.

## Repository Contents
- `dataset/`: Original vibration recordings.
- `Bearing_Vibration_Analysis.ipynb`: Python analysis notebook.
- `bearing_features.csv`: Extracted vibration features, if included.

## Limitations
The initial analysis uses one healthy and one faulty recording. The overlapping windows are not independent recordings. Further data, validation and testing are required before drawing general conclusions about model performance.

## Future Work
- Expand the dataset.
- Train and evaluate a bearing-condition classifier.
- Integrate the ML model with PLC control and monitoring.
- Validate the integrated system.

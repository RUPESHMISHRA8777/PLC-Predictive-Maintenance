# PLC-Predictive-Maintenance
PLC-Based Predictive Maintenance Using Machine Learning
# PLC-Based Predictive Maintenance Using Machine Learning

## Project
Bearing-condition classification using vibration data,
with a PLC as the operational/control core and an
ML model for condition classification.

## Dataset
Source: Case Western Reserve University Bearing Data Center

https://engineering.case.edu/bearingdatacenter/download-data-file

## Initial Data
- Normal_0: Healthy bearing
- IR007_0: Inner race fault, 0.007-inch fault diameter

Sampling frequency: 12 kHz
Measurement: Drive-end vibration

## Work Completed
- Loaded MATLAB (.mat) vibration data in Google Colab
- Plotted healthy and faulty vibration signals
- Calculated RMS, peak, crest factor and kurtosis
- Created an initial window-based feature extraction pipeline

## Files
- Bearing_Vibration_Analysis.ipynb
- bearing_features.csv

## Current Limitations
The initial analysis uses one healthy and one faulty
recording. Further recordings and validation are required.

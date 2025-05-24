# ecg_detection
ECG heart rate and QRS complex detection project, the goal is to demonstrate classical biomedical signal processing techniques using python.
Data = MIT-BIH Arrhythmia Database, one of the most widely used public ECG database

The intended structure of this project is as follows
```
  ecg-qrs-analysis/
  ├── data/                       # To host raw data in repo
  ├── notebooks/                  # Jupyter notebooks for processing
  │   └── 01_qrs_detection.ipynb  # Main analysis notebook
  ├── results/                    # Plots, output CSVs, etc.
  ├── README.md
  ├── requirements.txt
  └── LICENSE
```

## Features
- Bandpass filtering
- QRS complex detection (Pan-Tompkins algorithm)
- RR interval and heart rate analysis
- Visualize processing results

## Dataset
MIT-BIH Arrhythmia Database ([link](https://physionet.org/content/mitdb/1.0.0/)) via WFDB package.

## Tools
- Python
- Numpy, Scipy, matplotlib
- WFDB (Waveform DataBase) Package

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook notebooks/01_qrs_detection.ipynb
```

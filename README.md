# ecg_detection
ECG heart rate and QRS complex detection project, the goal is to demonstrate classical biomedical signal processing techniques using python.
Data = MIT-BIH Arrhythmia Database, one of the most widely used public ECG database

The intended structure of this project is as follows
```
  ecg-qrs-analysis/
  ├── data/                       # Host raw data in repo (no need to stream data from PhysioNet)
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
MIT-BIH Arrhythmia Database, a subset database in PhysioNet.
It can be streamed via WFDB package (pn_dir='mitdb'), or downloaded for local access.
[link](https://physionet.org/content/mitdb/1.0.0/)
Specs: 360 Hz, 2-lead ECG, 11-bit reso, 10mV range, 48x 30min excerpts
Common files: 100.dat, 100.hea, 100.atr(annotations)

## Tools
- Python
- Numpy, Scipy, matplotlib
- WFDB Package (Native Python Waveform DataBase [link] (https://github.com/MIT-LCP/wfdb-python))

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook notebooks/01_qrs_detection.ipynb
```

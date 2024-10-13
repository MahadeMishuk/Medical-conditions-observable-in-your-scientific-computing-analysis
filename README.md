# Medical-conditions-observation-in-scientific-computing-analysis
Electrocardiogram (ECG) is the process of producing a recording of the heart's electrical activity through repeated cardiac cycles. An ECG is visualized as a graph of voltage versus time. The voltage is the electrical activity of the heart measured by placing electrodes on the skin.¶
Python has a built-in ECG dataset
from scipy.misc import electrocardiogram
Sampling rate is 360 Hz ecg = electrocardiogram()
• Unfortunately, this patient has patterns of unusual heart beats.
• For reference, the time period 9 seconds to 10.2 seconds is a set of normal heart activity.
• From 46.5 seconds to 50 seconds the ECG shows what doctors call premature ventricular contractions.
• Time period 207 seconds to 215 seconds show significant abnormal activity.
We will find out FFT and spectrograms to be used to help diagnose heart conditions. Specifically, we will compute FFT and spectrograms for the three time periods above as well as the entire time period to observe conditions.

---

# ECG Signal Analysis for Detecting Abnormal Heart Activity

This project implements various signal processing techniques and machine learning methods to analyze Electrocardiogram (ECG) signals for detecting abnormal heart activity such as arrhythmias and premature ventricular contractions (PVCs). By applying Fast Fourier Transform (FFT), spectrogram analysis, and clustering algorithms, we explore patterns in heart activity and identify abnormal signals.

## Key Features

- **FFT Analysis**: Frequency-domain representation of normal and abnormal heartbeats, allowing detection of irregularities.
- **Spectrograms**: Time-frequency analysis for visualizing how the frequency content of the signal changes over time.
- **K-Means Clustering**: Groups ECG data into clusters of normal, PVC, and abnormal heartbeats without prior labels.

## Signal Processing Overview

1. **Dataset**: Utilizes a pre-loaded ECG dataset with a sampling frequency of 360 Hz.
2. **FFT**: Applied to the entire signal as well as specific time periods corresponding to normal heartbeats, PVCs, and abnormal heart activity. This provides insight into the dominant frequencies during different cardiac conditions.
3. **Spectrogram**: Visualizes the time-frequency content of the ECG signal for better identification of irregular patterns.

## Clustering Analysis

We extract frequency-domain features using FFT and apply K-Means clustering to categorize the ECG data into three groups:

- Normal Heart Activity
- Premature Ventricular Contractions (PVC)
- Significant Abnormal Activity

This clustering helps to automatically detect abnormal patterns in the ECG data without the need for labeled training data.

## Results

The project visualizes:

- FFT results of various ECG segments
- Spectrograms of the entire ECG signal and specific conditions
- Clusters formed from FFT features of normal, PVC, and abnormal signals

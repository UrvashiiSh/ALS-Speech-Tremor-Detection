### Methodology

This document summarizes the methodology used in the research paper **"Exploiting Speech Tremors: Machine Learning for Early Diagnosis of Amyotrophic Lateral Sclerosis."**

---

### Research Objective

The objective of this study was to investigate whether speech tremors extracted from sustained phonation recordings can serve as reliable acoustic biomarkers for the early diagnosis of Amyotrophic Lateral Sclerosis (ALS).

The study evaluates multiple machine learning algorithms to identify subtle speech abnormalities associated with early-stage ALS.


### Dataset

The study utilized sustained speech recordings collected from publicly available ALS speech datasets.

#### Dataset Summary

| Feature | Description |
|---------|-------------|
| Recording Type | Sustained Phonation |
| Disease | Amyotrophic Lateral Sclerosis |
| Data Type | Audio Recordings |
| Target | Early ALS Detection |


### Exploratory Voice Analysis & Preprocessing

The first stage of the study involved a comprehensive exploration of the audio dataset to understand its structure and quality before applying machine learning models.
Each recording was examined for characteristics such as duration, sample rate, signal consistency, and acoustic properties. This exploratory analysis played an important role in identifying potential data quality issues, including incomplete or corrupted recordings, while guiding subsequent preprocessing steps.

The preprocessing stage included:

- Audio quality inspection
- Signal visualization
- Data cleaning
- Audio normalization
- Preparation of recordings for feature extraction

This initial exploration ensured that the speech recordings were suitable for extracting reliable acoustic biomarkers associated with ALS-related speech tremors.

### Feature Extraction

Following preprocessing, acoustic features were extracted from the sustained speech recordings to characterize vocal tremors associated with Amyotrophic Lateral Sclerosis (ALS).

The extracted features captured multiple aspects of speech production, including:

- Intensity
- Fundamental Frequency (Pitch)
- Harmonics-to-Noise Ratio (HNR)
- Glottal-to-Noise Ratio (GNR)
- Jitter
- Shimmer
- Spectral Features
- Formant Frequencies
- Mel-Frequency Cepstral Coefficients (MFCCs)

These features provide quantitative representations of voice quality, vocal stability, articulation, and neuromuscular control.
Together, they serve as objective biomarkers capable of distinguishing ALS-related speech characteristics from healthy speech.

Due to the high dimensionality of the extracted feature set—primarily driven by MFCC features—Principal Component Analysis (PCA) was applied to reduce redundancy
while preserving the most informative components for machine learning.

### Exploratory Voice Analysis

Before model development, an extensive exploratory analysis was conducted to understand the acoustic characteristics of both healthy and ALS speech recordings.

The visualization stage focused on identifying patterns that distinguish ALS-related vocal tremors from normal speech. Several signal representations were generated and interpreted, including:

- Waveforms
- Power Spectrums
- Mel-Frequency Cepstral Coefficients (MFCCs)
- Zero-Crossing Rate (ZCR)
- Pitch Contours

These visualizations provided valuable insights into vocal stability, pitch variation, spectral energy distribution, and speech irregularities associated with ALS.

The exploratory analysis also supported data cleaning and preprocessing by revealing inconsistencies, missing information, and variations in recording quality
before machine learning models were developed.

### Machine Learning Model & Model Evaluation

Multiple machine learning algorithms were evaluated to determine the most effective approach for early ALS diagnosis.\

- Ensemble Models
- Linear and Hyperplane Models
- Instance-based Models

The models were evaluated using standard classification metrics including:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

These metrics enabled a comprehensive comparison of predictive performance.


### Results

The machine learning models successfully identified speech tremor characteristics associated with ALS.\
The findings demonstrate that speech-derived acoustic biomarkers have strong potential for supporting early diagnosis and clinical decision-making.

### Limitations

The study has several limitations:

- Limited dataset size
- Need for external validation
- Demographic variability
- Clinical validation required before deployment

### Future Work

Potential future directions include:

- Deep learning approaches
- Larger multi-center datasets
- Real-time speech monitoring
- Mobile healthcare applications
- Longitudinal patient monitoring


### Workflow Overview

```
Speech Recording
        │
        ▼
Audio Preprocessing
        │
        ▼
Feature Extraction
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Machine Learning Models
        │
        ▼
Model Evaluation
        │
        ▼
Early ALS Prediction
```
<br>

---

### Additional Resources
See the project `README` for an overview of the research.\
Publication details and citation information are available in `publication.md`.

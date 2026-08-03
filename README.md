<div align="center">
# Ali Naderi
**AI Research Engineer | Data Scientist | M.Sc. Mechatronics Engineering**
Physics-informed deep learning for industrial systems, medical imaging, and signal intelligence.
<a href="https://alinaderiii.github.io/"><img src="https://img.shields.io/badge/Portfolio-E85D4A?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
<a href="https://doi.org/10.1155/cplx/1644859"><img src="https://img.shields.io/badge/Published_Research-6C4AB6?style=for-the-badge&logo=doi&logoColor=white" alt="Publication"></a>
<a href="https://www.linkedin.com/in/alinaderi-data-scientist"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="https://www.kaggle.com/alinaderi1"><img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" alt="Kaggle"></a>
<a href="https://orcid.org/0009-0004-8166-5449"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" alt="ORCID"></a>
<a href="mailto:alinaderi119@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
<sub>Dublin, Ireland &nbsp;|&nbsp; Open to research collaboration and applied AI engineering</sub>
</div>
---
## What I do
I turn raw physical signals into decisions engineers can defend.
Most machine learning treats the sensor as a black box and the model as another one. My background in **Mechatronics Engineering** pushes the opposite way: I encode the physics of the system directly into the architecture, so the model's behaviour can be traced back to something mechanical and real. The result is systems that stay accurate under industrial noise, run on modest hardware, and survive review by people who know the machine better than the model.
That approach produced a peer-reviewed CAD system for brain tumour classification, and a fault-diagnosis network that holds **99.72% accuracy at -10 dB SNR** - where the noise is ten times stronger than the signal.
**Currently:** extending physics-informed architectures to rotating machinery and drilling telemetry.
---
## Research
<table>
<tr><td width="55%">
**Convolutional Neural Network and Channel Attention Mechanism for Multiclass Brain Tumor Classification**
*Complexity* (Wiley), Vol. 2025 | Open Access
Naderi A., Asgharzadeh-Bonab A., Ahmadi F., Kalbkhani H.
Fine-tuned EfficientNetB7 with a channel attention module that amplifies clinically relevant tumour features. Validated by 5-fold stratified cross-validation across three MRI benchmarks.
[![DOI](https://img.shields.io/badge/DOI-10.1155/cplx/1644859-006699?style=flat-square)](https://doi.org/10.1155/cplx/1644859)
[![Repo](https://img.shields.io/badge/Materials-181717?style=flat-square&logo=github)](https://github.com/AliNaderiii/brain-tumor-classification-paper)
</td><td width="45%">
| Benchmark | Accuracy |
|---|---|
| Brats-4C (4-class) | **98.16%** |
| Brats-2C large | **99.4%** |
| Brats-2C small | **99.2%** |
<sub>Outperforms Kang et al. 2021 (91.58%), Irmak 2021 (92.66%), Demir & Akbulut 2022 (96.60%), Shahin et al. 2023 (94.02%).</sub>
</td></tr>
</table>
**PhyQ-TransNet: Physics-Informed Deep Learning for Intelligent Fault Diagnosis**
*International Journal of Machine Tools and Manufacture* (Elsevier) | **manuscript submitted, under review**
A physics-informed feature extractor coupled to a Transformer encoder, mathematically aligned with classical signal demodulation rather than learned from scratch. Evaluated on five international bearing benchmarks: CWRU, SGST, IMS, Paderborn, NBS.
| Metric | Result |
|---|---|
| Accuracy across 5 benchmarks | 99.98% |
| Real-fault accuracy (ECE 0.0047) | 99.03% |
| Accuracy at -10 dB SNR | 99.72% |
| Inference / parameters | ~8.5 ms (~117 FPS) / 1.4M |
---
## Selected work
| Project | What it does | Result | Links |
|---|---|---|---|
| **Brain Tumor Classification** | EfficientNetB7 + channel attention on MRI | 98.16% four-class | [Repo](https://github.com/AliNaderiii/brain-tumor-classification-paper) | [Paper](https://doi.org/10.1155/cplx/1644859) |
| **Traffic Density Estimation** | YOLO11 Nano + OpenCV dual-lane ROI counting | 97.4% mAP50, ONNX 10.1 MB | [Repo](https://github.com/AliNaderiii/Real-Time-traffic-density-estimation) | [Live](https://alinaderiii.github.io/Real-Time-traffic-density-estimation/) |
| **Heart Disease Prediction** | Stacking ensemble CDSS on UCI Cleveland | Recall-optimised, zero leakage | [Repo](https://github.com/AliNaderiii/Heart-disease-prediction) | [Live](https://alinaderiii.github.io/Heart-disease-prediction/) |
| **Rice Production Forecasting** | Hybrid SARIMAX + RF residual coupling, 1950-2024 | R2 0.9254, MAPE 5.12% | [Repo](https://github.com/AliNaderiii/Rice-Production-Forecasting-SriLanka) | [Live](https://alinaderiii.github.io/Rice-Production-Forecasting-SriLanka/) |
| **WHO Health Intelligence** | Production ETL over WHO GHO OData, LIVE/DEMO/STALE data modes | Idempotent SQLite + quality reports | [Repo](https://github.com/AliNaderiii/who-health-intelligence) |
| **ROGII Wellbore Geology** | Leakage-free pipeline for lithology prediction from drilling telemetry | Well-group CV isolation | [Repo](https://github.com/AliNaderiii/ROGII_Wellbore_Geology_Prediction) |
| **Smart Farming Analytics** | Precision agriculture yield modelling | Statistical audit proving feature independence | [Repo](https://github.com/AliNaderiii/Precision-Agriculture-Yield-Forecasting-Smart-Farming) | [Live](https://alinaderiii.github.io/Precision-Agriculture-Yield-Forecasting-Smart-Farming/) |
<sub>The Smart Farming study concluded the dataset carries **no predictive signal** - mutual information near zero, negative out-of-sample R2. I published the negative result and the overfitting curves rather than reporting a tuned score. Reporting what the data actually supports is part of the job.</sub>
---
## Engineering practice
<table>
<tr><td width="33%" valign="top">
**Validation discipline**
Chronological and group-wise splits, never random shuffles on temporal or clustered data. `ColumnTransformer` pipelines so scaling never sees the test fold. VIF and multicollinearity audits before inference.
</td><td width="33%" valign="top">
**Deployment realism**
ONNX export for cross-platform C++/OpenCV serving. Models sized for accessible hardware - GTX 1650, Intel i5 - not cloud clusters. Edge-compatible inference budgets.
</td><td width="34%" valign="top">
**Honest reporting**
Negative results published alongside positive ones. Calibration error reported next to accuracy. Scope statements that say what a system is *not* validated for.
</td></tr>
</table>
---
## Stack
**Core**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
**Modelling**
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=flat-square)
![LightGBM](https://img.shields.io/badge/LightGBM-9ACD32?style=flat-square)
![statsmodels](https://img.shields.io/badge/statsmodels-4051B5?style=flat-square)
![YOLO11](https://img.shields.io/badge/YOLO11-00BFC4?style=flat-square)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=flat-square&logo=onnx&logoColor=white)
**Data and delivery**
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white)
<details>
<summary><b>Domain depth</b></summary>
<br>
| Area | Methods |
|---|---|
| **Signal processing** | FFT, Hilbert-Huang Transform, wavelet decomposition, time-frequency analysis, envelope demodulation, multi-sensor fusion |
| **Predictive maintenance** | Bearing fault diagnosis, condition monitoring, noise-robust classification, CWRU / IMS / Paderborn benchmarks |
| **Medical imaging** | Transfer learning, attention mechanisms, CAD system design, stratified cross-validation |
| **Time series** | SARIMAX, exogenous forecasting, residual hybrid coupling, stationarity testing, chronological validation |
| **Statistics** | Mann-Whitney U, Chi-square with Cramer's V, Spearman rank, Q-Q normality, mutual information, ADF |
</details>
---
<div align="center">
### Open to research collaboration, industrial AI, and hard diagnostic problems
**[alinaderi119@gmail.com](mailto:alinaderi119@gmail.com)** &nbsp;|&nbsp; [Portfolio](https://alinaderiii.github.io/) &nbsp;|&nbsp; [LinkedIn](https://www.linkedin.com/in/alinaderi-data-scientist) &nbsp;|&nbsp; [ResearchGate](https://www.researchgate.net/profile/Ali-Naderi-21)
</div>

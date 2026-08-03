![Ali Naderi](https://capsule-render.vercel.app/api?type=waving&color=0:1b2a4a,45:6c4ab6,80:e85d4a,100:d98e2b&height=190&section=header&text=Ali%20Naderi&fontSize=48&fontColor=ffffff&fontAlignY=36&desc=AI%20Research%20Engineer%20%7C%20Physics-Informed%20Deep%20Learning&descSize=17&descAlignY=57)
<p align="center">
  <a href="https://doi.org/10.1155/cplx/1644859"><img src="https://img.shields.io/badge/Published-Complexity%20(Wiley)%202025-6C4AB6?style=for-the-badge&logo=bookstack&logoColor=white" alt="Published"></a>
  <a href="https://alinaderiii.github.io/"><img src="https://img.shields.io/badge/Portfolio-E85D4A?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/alinaderi-data-scientist"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://orcid.org/0009-0004-8166-5449"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" alt="ORCID"></a>
  <a href="mailto:alinaderi119@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>
<p align="center">
  <img src="https://komarev.com/ghpvc/?username=AliNaderiii&label=Profile%20views&color=6c4ab6&style=flat-square" alt="views">
  <img src="https://img.shields.io/badge/Dublin-Ireland-1b2a4a?style=flat-square&logo=googlemaps&logoColor=white" alt="location">
  <img src="https://img.shields.io/badge/M.Sc.-Mechatronics%20Engineering-d98e2b?style=flat-square" alt="education">
  <img src="https://img.shields.io/badge/Open%20to-Research%20Collaboration-2ea44f?style=flat-square" alt="status">
</p>
***
## I turn raw physical signals into decisions engineers can defend
Most machine learning treats the sensor as a black box and the model as another one. My background in **Mechatronics Engineering** pushes the opposite way: I encode the physics of the system directly into the architecture, so the model's behaviour traces back to something mechanical and real.
The result is systems that stay accurate under industrial noise, run on modest hardware, and survive review by people who know the machine better than the model.
* Peer-reviewed CAD system for brain tumour classification, **98.16%** four-class accuracy
* Fault-diagnosis network holding **99.72%** accuracy where noise is 10x stronger than signal
* Currently extending physics-informed architectures to rotating machinery and drilling telemetry
***
## Research
**Convolutional Neural Network and Channel Attention Mechanism for Multiclass Brain Tumor Classification**
`Complexity (Wiley)` &nbsp; `Vol. 2025` &nbsp; `Open Access` &nbsp; `30 June 2025`
Naderi A., Asgharzadeh-Bonab A., Ahmadi F., Kalbkhani H.
Fine-tuned EfficientNetB7 with a channel attention module that amplifies clinically relevant tumour features. Validated by 5-fold stratified cross-validation across three MRI benchmarks.
| Method | Architecture | Accuracy |
| :--- | :--- | ---: |
| Kang et al. (2021) | DenseNet-169 + ShuffleNet + MnasNet | 91.58% |
| Irmak (2021) | Custom CNN | 92.66% |
| Shahin et al. (2023) | MPCANet (PCANet + CNN) | 94.02% |
| Demir and Akbulut (2022) | R-CNN + SVM | 96.60% |
| **This work** | **EfficientNetB7 + CAM + FC** | **98.16%** |
[![DOI](https://img.shields.io/badge/DOI-10.1155%2Fcplx%2F1644859-006699?style=flat-square)](https://doi.org/10.1155/cplx/1644859) [![Materials](https://img.shields.io/badge/Materials-181717?style=flat-square&logo=github)](https://github.com/AliNaderiii/brain-tumor-classification-paper)
**PhyQ-TransNet: Physics-Informed Deep Learning for Intelligent Fault Diagnosis**
`IJMTM (Elsevier)` &nbsp; `Manuscript submitted` &nbsp; `Under review`
A physics-informed feature extractor coupled to a Transformer encoder, mathematically aligned with classical signal demodulation rather than learned from scratch. Evaluated on five international bearing benchmarks: CWRU, SGST, IMS, Paderborn, NBS.
| Accuracy (5 benchmarks) | At -10 dB SNR | Calibration ECE | Inference | Parameters |
| :---: | :---: | :---: | :---: | :---: |
| **99.98%** | **99.72%** | **0.0047** | **8.5 ms** | **1.4M** |
***
## Selected work
| Project | Approach | Result | Links |
| :--- | :--- | :--- | :--- |
| **Brain Tumor Classification** | EfficientNetB7 + channel attention on MRI | `98.16%` four-class | [Repo](https://github.com/AliNaderiii/brain-tumor-classification-paper) / [Paper](https://doi.org/10.1155/cplx/1644859) |
| **Traffic Density Estimation** | YOLO11 Nano + OpenCV dual-lane ROI counting | `97.4%` mAP50, ONNX 10.1 MB | [Repo](https://github.com/AliNaderiii/Real-Time-traffic-density-estimation) / [Live](https://alinaderiii.github.io/Real-Time-traffic-density-estimation/) |
| **Heart Disease Prediction** | Stacking ensemble CDSS on UCI Cleveland | Recall-optimised, zero leakage | [Repo](https://github.com/AliNaderiii/Heart-disease-prediction) / [Live](https://alinaderiii.github.io/Heart-disease-prediction/) |
| **Rice Production Forecasting** | Hybrid SARIMAX + RF residual coupling | `R2 0.9254`, MAPE 5.12% | [Repo](https://github.com/AliNaderiii/Rice-Production-Forecasting-SriLanka) / [Live](https://alinaderiii.github.io/Rice-Production-Forecasting-SriLanka/) |
| **WHO Health Intelligence** | Production ETL, LIVE/DEMO/STALE data modes | Idempotent SQLite + audits | [Repo](https://github.com/AliNaderiii/who-health-intelligence) |
| **ROGII Wellbore Geology** | Lithology prediction from drilling telemetry | Well-group CV isolation | [Repo](https://github.com/AliNaderiii/ROGII_Wellbore_Geology_Prediction) |
| **Smart Farming Analytics** | Yield modelling + statistical signal audit | Proved feature independence | [Repo](https://github.com/AliNaderiii/Precision-Agriculture-Yield-Forecasting-Smart-Farming) / [Live](https://alinaderiii.github.io/Precision-Agriculture-Yield-Forecasting-Smart-Farming/) |
> **On the Smart Farming result:** the dataset carried no predictive signal. Mutual information near zero, negative out-of-sample R2. I published the negative result and the overfitting curves rather than reporting a tuned score. Reporting what the data actually supports is part of the job.
***
## How I work
**Validation discipline** &mdash; Chronological and group-wise splits, never random shuffles on temporal or clustered data. ColumnTransformer pipelines so scaling never sees the test fold. VIF and multicollinearity audits before inference.
**Deployment realism** &mdash; ONNX export for cross-platform C++ and OpenCV serving. Models sized for accessible hardware such as GTX 1650 and Intel i5, not cloud clusters. Edge-compatible inference budgets.
**Honest reporting** &mdash; Negative results published alongside positive ones. Calibration error reported next to accuracy. Scope statements that say what a system is not validated for.
***
## Stack
<p>
  <img src="https://skillicons.dev/icons?i=python,pytorch,tensorflow,sklearn,opencv,docker&theme=dark" alt="core">
</p>
<p>
  <img src="https://skillicons.dev/icons?i=matlab,postgres,git,github,linux,vscode&theme=dark" alt="tools">
</p>
`XGBoost` &nbsp; `LightGBM` &nbsp; `statsmodels` &nbsp; `YOLO11` &nbsp; `ONNX` &nbsp; `Pandas` &nbsp; `NumPy` &nbsp; `SciPy` &nbsp; `Streamlit` &nbsp; `Ultralytics`
<details>
<summary><b>Domain depth</b></summary>
<br>
| Area | Methods |
| :--- | :--- |
| **Signal processing** | FFT, Hilbert-Huang Transform, wavelet decomposition, time-frequency analysis, envelope demodulation, multi-sensor fusion |
| **Predictive maintenance** | Bearing fault diagnosis, condition monitoring, noise-robust classification, CWRU / IMS / Paderborn / SGST / NBS |
| **Medical imaging** | Transfer learning, channel attention, CAD system design, stratified cross-validation |
| **Time series** | SARIMAX, exogenous forecasting, residual hybrid coupling, stationarity testing, chronological validation |
| **Statistics** | Mann-Whitney U, Chi-square with Cramer's V, Spearman rank, Q-Q normality, mutual information, ADF |
</details>
***
## Activity
<p align="center">
  <img width="48%" src="https://github-readme-stats.vercel.app/api?username=AliNaderiii&show_icons=true&hide_border=true&title_color=e85d4a&icon_color=6c4ab6&text_color=8b949e&bg_color=0d1117&include_all_commits=true" alt="stats">
  <img width="42%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=AliNaderiii&layout=compact&hide_border=true&title_color=e85d4a&text_color=8b949e&bg_color=0d1117&langs_count=6" alt="languages">
</p>
***
<p align="center">
  <b>Open to research collaboration, industrial AI, and hard diagnostic problems.</b>
</p>
<p align="center">
  <a href="mailto:alinaderi119@gmail.com"><img src="https://img.shields.io/badge/alinaderi119@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="email"></a>
  <a href="https://alinaderiii.github.io/"><img src="https://img.shields.io/badge/Portfolio-E85D4A?style=flat-square&logo=googlechrome&logoColor=white" alt="portfolio"></a>
  <a href="https://www.linkedin.com/in/alinaderi-data-scientist"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="linkedin"></a>
  <a href="https://www.kaggle.com/alinaderi1"><img src="https://img.shields.io/badge/Kaggle-20BEFF?style=flat-square&logo=kaggle&logoColor=white" alt="kaggle"></a>
  <a href="https://www.researchgate.net/profile/Ali-Naderi-21"><img src="https://img.shields.io/badge/ResearchGate-00CCBB?style=flat-square&logo=researchgate&logoColor=white" alt="researchgate"></a>
</p>
![footer](https://capsule-render.vercel.app/api?type=waving&color=0:d98e2b,20:e85d4a,55:6c4ab6,100:1b2a4a&height=100&section=footer)

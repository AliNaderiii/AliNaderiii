# Ali Naderi
**AI Research Engineer | Data Scientist | M.Sc. Mechatronics Engineering**
Physics-informed deep learning for industrial systems, medical imaging, and signal intelligence. Based in Dublin, Ireland.
[![Published](https://img.shields.io/badge/Published-Complexity%20Wiley%202025-6C4AB6?style=for-the-badge&logo=bookstack&logoColor=white)](https://doi.org/10.1155/cplx/1644859)
[![Portfolio](https://img.shields.io/badge/Portfolio-E85D4A?style=for-the-badge&logo=googlechrome&logoColor=white)](https://alinaderiii.github.io/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/alinaderi-data-scientist)
[![ORCID](https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white)](https://orcid.org/0009-0004-8166-5449)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:alinaderi119@gmail.com)
## About
I turn raw physical signals into decisions engineers can defend.
Most machine learning treats the sensor as a black box and the model as another one. My background in Mechatronics Engineering pushes the opposite way: I encode the physics of the system directly into the architecture, so the model behaviour traces back to something mechanical and real. The result is systems that stay accurate under industrial noise, run on modest hardware, and survive review by people who know the machine better than the model.
* Peer-reviewed CAD system for brain tumour classification, 98.16 percent four-class accuracy
* Fault-diagnosis network holding 99.72 percent accuracy where noise is ten times stronger than the signal
* Currently extending physics-informed architectures to rotating machinery and drilling telemetry
## Publications
**Convolutional Neural Network and Channel Attention Mechanism for Multiclass Brain Tumor Classification**
Complexity (Wiley), Volume 2025. Open Access. Published 30 June 2025.
Naderi A., Asgharzadeh-Bonab A., Ahmadi F., Kalbkhani H.
Fine-tuned EfficientNetB7 with a channel attention module that amplifies clinically relevant tumour features, validated by 5-fold stratified cross-validation across three MRI benchmarks.
| Method | Architecture | Accuracy |
| :--- | :--- | ---: |
| Kang et al. 2021 | DenseNet-169 + ShuffleNet + MnasNet | 91.58% |
| Irmak 2021 | Custom CNN | 92.66% |
| Shahin et al. 2023 | MPCANet (PCANet + CNN) | 94.02% |
| Demir and Akbulut 2022 | R-CNN + SVM | 96.60% |
| **This work** | **EfficientNetB7 + CAM + FC** | **98.16%** |

[![DOI](https://img.shields.io/badge/DOI-10.1155%2Fcplx%2F1644859-006699?style=flat-square)](https://doi.org/10.1155/cplx/1644859)
[![Materials](https://img.shields.io/badge/Materials-181717?style=flat-square&logo=github)](https://github.com/AliNaderiii/brain-tumor-classification-paper)
**PhyQ-TransNet: Physics-Informed Deep Learning for Intelligent Fault Diagnosis**
International Journal of Machine Tools and Manufacture (Elsevier). Manuscript submitted, under review.
A physics-informed feature extractor coupled to a Transformer encoder, mathematically aligned with classical signal demodulation rather than learned from scratch. Evaluated on five international bearing benchmarks: CWRU, SGST, IMS, Paderborn, NBS.
| Metric | Result |
| :--- | ---: |
| Accuracy across five benchmarks | 99.98% |
| Real-fault accuracy, calibration ECE 0.0047 | 99.03% |
| Accuracy under extreme noise at -10 dB SNR | 99.72% |
| Inference latency | 8.5 ms, about 117 FPS |
| Model size | 1.4M parameters, 3.21 GFLOPs |
## Projects
| Project | Approach | Result | Links |
| :--- | :--- | :--- | :--- |
| **Brain Tumor Classification** | EfficientNetB7 with channel attention on MRI | 98.16% four-class | [Repo](https://github.com/AliNaderiii/brain-tumor-classification-paper) - [Paper](https://doi.org/10.1155/cplx/1644859) |
| **Traffic Density Estimation** | YOLO11 Nano with OpenCV dual-lane ROI counting | 97.4% mAP50, ONNX 10.1 MB | [Repo](https://github.com/AliNaderiii/Real-Time-traffic-density-estimation) - [Live](https://alinaderiii.github.io/Real-Time-traffic-density-estimation/) |
| **Heart Disease Prediction** | Stacking ensemble decision support on UCI Cleveland | Recall-optimised, zero leakage | [Repo](https://github.com/AliNaderiii/Heart-disease-prediction) - [Live](https://alinaderiii.github.io/Heart-disease-prediction/) |
| **Rice Production Forecasting** | Hybrid SARIMAX with Random Forest residual coupling | R2 0.9254, MAPE 5.12% | [Repo](https://github.com/AliNaderiii/Rice-Production-Forecasting-SriLanka) - [Live](https://alinaderiii.github.io/Rice-Production-Forecasting-SriLanka/) |
| **WHO Health Intelligence** | Production ETL over WHO GHO OData, live and demo data modes | Idempotent SQLite with quality audits | [Repo](https://github.com/AliNaderiii/who-health-intelligence) |
| **ROGII Wellbore Geology** | Lithology prediction from drilling telemetry | Well-group cross-validation isolation | [Repo](https://github.com/AliNaderiii/ROGII_Wellbore_Geology_Prediction) |
| **Smart Farming Analytics** | Yield modelling with statistical signal audit | Proved feature independence | [Repo](https://github.com/AliNaderiii/Precision-Agriculture-Yield-Forecasting-Smart-Farming) - [Live](https://alinaderiii.github.io/Precision-Agriculture-Yield-Forecasting-Smart-Farming/) |
| **Dream** | Local-first bilingual assistant with Persian-aware memory retrieval | NFKC normalisation, zero-dependency core | [Repo](https://github.com/AliNaderiii/Dream) |

On the Smart Farming result: the dataset carried no predictive signal. Mutual information near zero, negative out-of-sample R2. I published the negative result and the overfitting curves rather than reporting a tuned score. Reporting what the data actually supports is part of the job.
## How I work
**Validation discipline.** Chronological and group-wise splits, never random shuffles on temporal or clustered data. ColumnTransformer pipelines so scaling never sees the test fold. VIF and multicollinearity audits before inference.
**Deployment realism.** ONNX export for cross-platform C++ and OpenCV serving. Models sized for accessible hardware such as GTX 1650 and Intel i5, not cloud clusters. Edge-compatible inference budgets.
**Honest reporting.** Negative results published alongside positive ones. Calibration error reported next to accuracy. Scope statements that say what a system is not validated for.
## Stack
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=flat-square&logo=onnx&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=flat-square)
![LightGBM](https://img.shields.io/badge/LightGBM-9ACD32?style=flat-square)
![statsmodels](https://img.shields.io/badge/statsmodels-4051B5?style=flat-square)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
## Domain depth
| Area | Methods |
| :--- | :--- |
| **Signal processing** | FFT, Hilbert-Huang Transform, wavelet decomposition, time-frequency analysis, envelope demodulation, multi-sensor fusion |
| **Predictive maintenance** | Bearing fault diagnosis, condition monitoring, noise-robust classification, CWRU, IMS, Paderborn, SGST and NBS benchmarks |
| **Medical imaging** | Transfer learning, channel attention, computer-aided diagnosis design, stratified cross-validation |
| **Time series** | SARIMAX, exogenous forecasting, residual hybrid coupling, stationarity testing, chronological validation |
| **Statistics** | Mann-Whitney U, Chi-square with Cramer V, Spearman rank, Q-Q normality, mutual information, ADF |
## Contact
Open to research collaboration, industrial AI, and hard diagnostic problems.
[alinaderi119@gmail.com](mailto:alinaderi119@gmail.com) | [Portfolio](https://alinaderiii.github.io/) | [LinkedIn](https://www.linkedin.com/in/alinaderi-data-scientist) | [Kaggle](https://www.kaggle.com/alinaderi1) | [ResearchGate](https://www.researchgate.net/profile/Ali-Naderi-21)
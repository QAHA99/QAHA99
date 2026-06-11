<h1 align="center">Qusai Al Haj Ali</h1>
<h3 align="center">
  Medical Engineer | MSc Data-Driven Health Student at <a href="https://www.kth.se/en/studies/master/data-driven-health">KTH</a>
</h3>
<p align="center">
  <i>Bridging the gap between Clinical Needs, AI Research, and Data Architectures.</i>
</p>
<div align="center">
  <a href="https://www.linkedin.com/in/qusai-al-haj-ali-76b29a39a/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin" />
  </a>
  <a href="mailto:alhajali.qusai@outlook.com">
    <img src="https://img.shields.io/badge/Email-Contact_Me-D14836?style=for-the-badge&logo=gmail" />
  </a>
</div>

<hr />

## Research & Clinical AI Experience

My work focuses on deep learning applications in medical imaging, specifically overcoming data scarcity and topological complexity in anatomical segmentation.

### Automated Lung Segmentation at NKS (New Karolinska Solna)

- **Role:** Medical Image Analyst / AI Engineer
- **Task:** Automatic segmentation of lung airways and pulmonary vessels from CT scans.
- **Method:** Utilized **nnU-Net**, a self-configuring deep learning framework that automates U-Net architecture design (preprocessing, network depth, and loss functions) to achieve robust segmentation on complex clinical data.

### Ongoing Research: Optimized Neural Networks for Pulmonary Topology

- **Objective:** Developing a specialized neural network architecture from scratch designed for the segmentation of pulmonary bodies.
- **Key Challenge:** Standard models often require massive datasets. My research focuses on Data-Efficient Learning, creating a model that achieves high accuracy with a smaller training database while optimizing computational efficiency for clinical settings.
- **Status:** *In Development*

<hr />

## Deep Learning & Medical AI

Hands-on deep learning projects across medical imaging, clinical NLP, and biosignals — most implemented from scratch in PyTorch. *(Datasets and trained weights are excluded from all repos; credentialed PhysioNet data is never redistributed.)*

### [Brain Tumor Segmentation & Classification (Self-Supervised, Multi-Task)](https://github.com/QAHA99/brain-tumor-ssl-segmentation)

- **Focus:** Self-supervised pre-training + multi-task learning on brain MRI
- Masked-Autoencoder pre-training, then joint tumor segmentation + 4-class classification; a controlled **U-Net vs. ResNet18-UNet** encoder comparison with an SSL-vs-no-SSL ablation.
- **Stack:** PyTorch, Dice/IoU/Hausdorff, macro-F1. *(Group project)*

### [Generalizable ECG Classification — CNN-Transformer + Semi-Supervised Learning](https://github.com/QAHA99/ecg-cnn-transformer)

- **Focus:** 12-lead ECG diagnosis robust across recording environments
- CNN-Transformer trained on PTB-XL (5 diagnostic super-classes) with pseudo-labelling on LTDB; Focal Loss for class imbalance; attention/SHAP/Integrated-Gradients interpretability.
- **Stack:** PyTorch, SciPy (signal processing). *(Group project)*

### [Binary Liver Segmentation — U-Net from Scratch](https://github.com/QAHA99/liver-segmentation-unet)

- **Focus:** CT organ segmentation
- U-Net built from scratch on AbdomenAtlas CT slices; BCE+Dice loss; **Dice 0.90 / IoU 0.84** on liver-containing test slices.
- **Stack:** PyTorch.

### [Chest X-Ray Report Generation — Show, Attend and Tell](https://github.com/QAHA99/chest-xray-captioning)

- **Focus:** Image captioning of radiology impressions
- CNN encoder + attention LSTM decoder generating the IMPRESSION sentence from MIMIC-CXR; includes an honest analysis of beam-search mode collapse and the CE-vs-BLEU disconnect.
- **Stack:** PyTorch.

### [Medical NLP — Radiology Report Classification](https://github.com/QAHA99/medical-nlp-classification)

- **Focus:** Clinical text classification from scratch
- Naive Bayes baseline vs. BiLSTM and attention-BiLSTM (no pre-trained embeddings) on MIMIC-CXR reports labelled via CheXpert.
- **Stack:** PyTorch, scikit-learn.

### [Early Sepsis Prediction from Clinical Time Series](https://github.com/QAHA99/sepsis-time-series-prediction)

- **Focus:** Multi-horizon clinical forecasting
- Bidirectional LSTM predicting sepsis onset 2/4/6 h ahead from 8 h of physiological signals; sliding windows, class-weighted loss, Youden's-J thresholding.
- **Stack:** TensorFlow/Keras, scikit-learn.

### [ICU False Alarm Prediction](https://github.com/QAHA99/icu-false-alarm-prediction)

- **Focus:** Reducing ICU alarm fatigue from biosignals
- Time- and frequency-domain features from ECG/PPG/ABP waveforms (VTaC); Random Forest reaches **ROC-AUC ≈ 0.83** vs. a Logistic Regression baseline.
- **Stack:** scikit-learn, SciPy, WFDB.

### [Backpropagation from Scratch (micrograd)](https://github.com/QAHA99/backprop-from-scratch)

- **Focus:** First-principles autograd
- A scalar reverse-mode autodiff engine + MLP library with no deep learning framework, gradients validated against PyTorch.
- **Stack:** NumPy, Graphviz.

### [LLM-Based MIMIC-IV Column Annotation](https://github.com/QAHA99/mimic-llm-column-annotation)

- **Focus:** Applying LLMs to clinical database understanding
- Locally hosted LLM (Ollama) auto-annotates MIMIC-IV table columns with Pydantic-validated structured output and MLflow experiment tracking.
- **Stack:** Ollama, Pydantic, MLflow, Pandas. *(Group project)*

<hr />

## Health Informatics & Data Engineering

### [Clinical Relational Database System](https://github.com/QAHA99/secure-clinic-db-system)

- **Focus:** Relational Modeling, Data Integrity & Database Security
- Designed a normalized PostgreSQL database featuring advanced triggers for logic enforcement (anti-overlap), PL/pgSQL stored procedures, and Role-Based Access Control (RBAC).
- **Stack:** PostgreSQL, PL/pgSQL, Java (JDBC).

### [Hybrid Graph-Document Medical System](https://github.com/QAHA99/hybrid-medical-db)

- **Focus:** Complex Data Relationships
- A hybrid CLI system leveraging **Neo4j** to map complex doctor-patient graph relationships and **MongoDB** for high-throughput messaging.
- **Stack:** Neo4j (Graph), MongoDB (Document), Java.

### [Secure FHIR-Integrated Clinic Platform](https://github.com/QAHA99/Secure-Clinic-Platform-FHIR)

- **Focus:** Clinical Systems & Backend Security
- Built a role-based clinical management system using **HAPI FHIR R4** for standardized patient data exchange. Features secure auth and patient management.
- **Stack:** Java, HAPI FHIR, MongoDB (GridFS).

### [Healthcare Data Lake & Analytics Platform](https://github.com/QAHA99/healthcare-data-lake)

- **Focus:** Big Data, ETL, & FHIR Interoperability
- Designed an end-to-end pipeline for ingesting and standardizing heterogeneous medical data (JSON/FHIR) into a scalable data lake.
- **Stack:** NoSQL (MongoDB), JSON, Java.

<hr />

## General Software Engineering

- **Java Ecosystem:** [Sudoku (JavaFX)](https://github.com/QAHA99/sudoku-javafx-mvc), [Poker Solitaire (Logic)](https://github.com/QAHA99/poker-solitaire-logic), [Sliding Puzzle (Logic)](https://github.com/QAHA99/sliding-puzzle-logic)
- **Game Development:** [2D Physics Platformer (C# / Unity)](https://github.com/QAHA99/2d-physics-platformer)
- **Systems Programming:** [Board Game Rating System (C)](https://github.com/QAHA99/board-game-rating-system)

<br />

<p align="center">
  <img src="https://img.shields.io/badge/Code-Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/AI-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/Healthcare-FHIR-E32011?style=flat-square&logo=hl7&logoColor=white" />
  <img src="https://img.shields.io/badge/Imaging-DICOM-005A9C?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Database-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/Database-PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Database-Neo4j-008CC1?style=flat-square&logo=neo4j&logoColor=white" />
  <img src="https://img.shields.io/badge/Big_Data-Apache_Hudi-FF7F00?style=flat-square&logo=apache&logoColor=white" />
</p>

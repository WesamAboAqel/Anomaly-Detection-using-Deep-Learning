# Anomaly Detection using Deep Learning

## Overview
This project implements an anomaly detection system using two deep learning models:  
- **Detection Model**: Determines whether network traffic is an anomaly or normal traffic.  
- **Classification Model**: Categorizes detected anomalies into specific attack types (e.g., DDoS, PortScan, Bot).  
Both models are trained and evaluated on a dataset stored in the `Dataset/Model` directory, with their confusion matrices and metrics provided.


## Classes (Classification Model)**: 10 classes mapped as follows:
  - Benign
  - DDoS
  - PortScan
  - Bot
  - Infiltration
  - Web Brute Force
  - FTP-Patator
  - SSH-Patator
  - DoS slowloris
  - DoS Slowhttptest

## Project Structure
- `Testing.ipynb`: Jupyter notebook containing the evaluation of both models, including metrics (Precision, Accuracy, Recall) and confusion matrices for the Detection and Classification Models.
- `Dataset/Model/`: Directory containing the large datasets (stored using Git LFS).

## How to Run
1. **Prerequisites**:
   - Python 3.x
   - Install dependencies: `pip install numpy pandas matplotlib seaborn tensorflow scikit-learn`
   - Git LFS (to download large datasets): `git lfs install`

2. **Clone the Repository**:
  - git clone https://github.com/WesamAboAqel/Anomaly-Detection-using-Deep-Learning.git
  - cd Anomaly-Detection-using-Deep-Learning
  - git lfs pull

3. **Run the Evaluation**:
- Open `Testing.ipynb` in Jupyter Notebook.
- Ensure both models `Detection Model` and `ClassModel` are trained or loaded.
- Run the notebook to see the metrics and confusion matrices for both models.

## Results
The final metrics (Precision, Accuracy, Recall) and confusion matrices for both the Detection Model (anomaly vs. normal) and the Classification Model (10 attack categories) are available in `Testing.ipynb`.

## Notes
- Large datasets are stored using Git LFS due to their size.
- Ensure you have sufficient storage to download the datasets.


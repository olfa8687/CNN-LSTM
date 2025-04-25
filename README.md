# SecureAlert Intrusion Detection Model (using CICIDS2018)

This repository contains the source code for a CNN-LSTM neural network implemented in Python using Keras. The model is designed for network intrusion detection using the three datasets: (CIC-IDS2017, CSE-CIC-IDS2018, and CIC-DDoS2019), (in the .ipynb we include the code using  CSE-CIC-IDS2018 and the we show the results of the three datasets), and it replicates the experiments conducted in our research.

## 📄 Paper Title
**Securing IoV Environments with Blockchain-Integrated Detection Systems"**

## 📚 Abstract
This notebook presents the implementation of an SecureAlert-based deep learning model developed to detect various types of network intrusions from flow-based features. The model architecture, training process, and evaluation are included to support reproducibility.


## 🗂️ Repository Contents

- `LSTM2018_(new).ipynb`: Main Jupyter Notebook with model code, training, and evaluation.
- `README.md`: Documentation for usage and reproducibility.
- `requirements.txt`: Python dependencies required to run the notebook.

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/olfa8687/LSTM-IDS-CICIDS2018.git
cd LSTM-IDS-CICIDS2018


### 2. Set up the environment

Ensure Python (≥3.7) is installed, then install the required libraries using pip:

```bash
pip install -r requirements.txt
```

---

### 3. Download and prepare the dataset

This project uses the ** CSE-CIC-IDS2018** dataset, a comprehensive and realistic dataset for intrusion detection system (IDS) research provided by the Canadian Institute for Cybersecurity (CIC).

#### 🔹 Dataset Highlights:
- Captured over 5 days with a variety of normal and attack traffic.
- Includes attack types such as DDoS, Brute Force, Infiltration, Web Attacks, and Botnets.
- Each flow contains over 80 extracted features using CICFlowMeter.
- Properly labeled with attack types and benign labels.

#### 🔹 Instructions to use:
1. Download the dataset from the official CIC website:  
   👉 https://www.unb.ca/cic/datasets/ids-2018.html

2. Preprocess the CSV files:
   - Clean missing values.
   - Encode labels.
   - Normalize features as shown in the notebook.

3. Place the final processed dataset inside the project in a directory named:

```bash
./data/
```

---

### 4. Run the notebook

Use Jupyter Notebook to open and execute the LSTM model:

```bash
jupyter notebook LSTM2018_(new).ipynb
```

- Follow the notebook cell-by-cell.
- It will guide you through data loading, preprocessing, model creation, training, and evaluation.

---

### 5. View results

Once the notebook has been executed:

- You will see **training vs validation accuracy/loss** plots.
- It will display the **confusion matrix** and **classification report**.
- Precision, Recall, and F1-score will be printed for each class.
- The model's performance on detecting various types of intrusions will be highlighted.

You may also export the model and save the results for future use.

---

## 🧪 Requirements

Below is a list of the required Python packages:

```txt
numpy>=1.18.5
pandas>=1.1.0
matplotlib>=3.2.2
scikit-learn>=0.23.2
tensorflow>=2.4.0
keras>=2.4.3
jupyter>=1.0.0
seaborn>=0.10.1
```

Install them all using:

```bash
pip install -r requirements.txt
```

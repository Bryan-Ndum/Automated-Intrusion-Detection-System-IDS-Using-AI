🚨 Automated Intrusion Detection System (IDS) Using AI

📌 Overview

This project demonstrates a real-time Intrusion Detection System (IDS) powered by machine learning to identify and classify security threats in a Software-Defined Networking (SDN) environment. Using Mininet to simulate traffic, the IDS monitors packets and raises alerts when malicious activity is detected.

🎯 Objectives

Detect and classify network intrusions using AI models.

Provide real-time monitoring in a simulated SDN environment.

Evaluate detection accuracy against multiple attack types.

🛠️ Tech Stack

Languages & Tools: Python, Mininet, Wireshark/Tshark

Libraries: scikit-learn, pandas, NumPy, matplotlib, seaborn, pyshark

Models Used: Decision Tree, Random Forest, Logistic Regression

⚙️ Implementation

Data Collection – Captured normal and malicious traffic (DoS, port scans, spoofing) in Mininet.

Feature Extraction – Converted traffic into structured datasets (flow size, packet count, protocol).

Model Training – Trained and tuned ML classifiers for intrusion detection.

Real-Time Detection – Integrated the trained model with live packet streams to flag anomalies.

Evaluation – Compared models using accuracy, precision, recall, and F1-score.

📊 Results

Achieved 85% detection accuracy against simulated attacks in Mininet.

Random Forest provided the best balance of detection accuracy and low false positives.

IDS successfully flagged DoS, probing, and spoofing attacks in real-time.

🚀 Future Work

Extend detection to zero-day attacks using deep learning (LSTM, CNN).

Deploy in cloud/edge computing environments.

Add a Streamlit dashboard for visualization & alerts.

📂 Project Structure
IDS-AI/
│── README.md
│── requirements.txt
│── src/
│   ├── data_preprocessing.py
│   ├── feature_extraction.py
│   ├── train_model.py
│   ├── real_time_detection.py
│   └── utils.py
│── notebooks/
│   ├── EDA.ipynb
│   ├── Model_Training.ipynb
│   └── Results_Visualization.ipynb
│── data/
│── models/
│── results/
│── docs/

📦 Installation & Usage

Clone the repo:

git clone https://github.com/your-username/IDS-AI.git
cd IDS-AI


Install dependencies:

pip install -r requirements.txt


Run model training:

python src/train_model.py


Run real-time IDS:

sudo python src/real_time_detection.py

📖 Documentation

A detailed project report is available in the docs/
 folder.

🔗 Project Link

👉 [Live Repo / Portfolio Link Here]

👤 Author

Bryan Ndum

GitHub

LinkedIn

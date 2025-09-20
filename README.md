# 🚨 Automated Intrusion Detection System (IDS) Using AI  

## 📌 Overview  
This project demonstrates a real-time **Intrusion Detection System (IDS)** powered by **machine learning** to identify and classify security threats in a Software-Defined Networking (SDN) environment. Using **Mininet** to simulate traffic, the IDS monitors packets and raises alerts when malicious activity is detected.  

## 🎯 Objectives  
- Detect and classify network intrusions using AI models.  
- Provide real-time monitoring in a simulated SDN environment.  
- Evaluate detection accuracy against multiple attack types.  

## 🛠️ Tech Stack  
- **Languages & Tools:** Python, Mininet, Wireshark/Tshark  
- **Libraries:** scikit-learn, pandas, NumPy, matplotlib, seaborn, pyshark  
- **Models Used:** Decision Tree, Random Forest, Logistic Regression  

## ⚙️ Implementation  
1. **Data Collection** – Captured normal and malicious traffic (DoS, port scans, spoofing) in Mininet.  
2. **Feature Extraction** – Converted traffic into structured datasets (flow size, packet count, protocol).  
3. **Model Training** – Trained and tuned ML classifiers for intrusion detection.  
4. **Real-Time Detection** – Integrated the trained model with live packet streams to flag anomalies.  
5. **Evaluation** – Compared models using accuracy, precision, recall, and F1-score.  

## 📊 Results  
- Achieved **85% detection accuracy** against simulated attacks in Mininet.  
- **Random Forest** provided the best balance of detection accuracy and low false positives.  
- IDS successfully flagged DoS, probing, and spoofing attacks in real-time.  

## 🚀 Future Work  
- Extend detection to **zero-day attacks** using deep learning (LSTM, CNN).  
- Deploy in **cloud/edge computing** environments.  
- Add a **Streamlit dashboard** for visualization & alerts.  


## 📦 Installation & Usage  
# 1. Clone the Repository
git clone https://github.com/Bryan-Ndum/IDS-AI.git
cd IDS-AI

# 2. (Optional) Create a Virtual Environment
python -m venv venv
source venv/bin/activate    # On Linux/Mac
venv\Scripts\activate       # On Windows

# 3. Install Dependencies
pip install -r requirements.txt

# 4. Verify Installation
pip list

# 5. Install Mininet (Linux only)
sudo apt-get update
sudo apt-get install mininet -y

# 6. (Optional) Install Wireshark/Tshark for packet capture
sudo apt-get install wireshark tshark -y


# Usage

# 1. Train the Model (saves trained .pkl files in models/)
python src/train_model.py

# 2. Run Real-Time IDS on simulated traffic
sudo python src/real_time_detection.py

# 3. (Optional) Launch Jupyter Notebook for experiments
jupyter notebook
# Then open notebooks/EDA.ipynb or notebooks/Model_Training.ipynb





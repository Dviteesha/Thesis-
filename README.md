---

```markdown
# 🖐️ Adaptive Hand Gesture Recognition using ROAR (Reinforcement Learning-Based Online Active Learning)

This repository contains experiments for hand gesture recognition using physiological sensor data (EMG and IMU) and the ROAR algorithm (Reinforcement Learning-based Online Active Learning). The objective is to minimize manual labeling while maintaining high classification accuracy using an intelligent sample querying mechanism.

---

## 📁 Repository Contents

```
.
├── README.md            # This file
├── emg1.ipynb           # Notebook for EMG Dataset 1 (MYO armband)
├── classify.ipynb       # Notebook for EMG Dataset 2 (compressed sensor layout)
├── Taiwan.ipynb         # Notebook for IMU Dataset (multi-sensor)
```

---

## 📊 Datasets Used

Place the required dataset files in the same directory as the notebooks or modify the paths as needed.

- **EMG Dataset 1**: `EMG-data.csv`   
- **EMG Dataset 2**: `0.csv`, `1.csv`, `2.csv`, `3.csv`  
- **IMU Dataset**: `train.csv`, `test1.csv`, `test2.csv`  

---

## ⚙️ Setup Instructions

### 1. 📥 Clone this repository

```bash
git clone https://github.com/yourusername/roar-gesture-recognition.git
cd roar-gesture-recognition
```

### 2. 🐍 (Optional) Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate     # On Linux/Mac
venv\Scripts\activate        # On Windows
```

### 3. 📦 Install dependencies

```bash
pip install -r requirements.txt
```

> If `requirements.txt` is not present, use:
```bash
pip install numpy pandas scikit-learn matplotlib seaborn jupyter
```

### 4. 🚀 Run the Notebooks

Launch Jupyter and open any of the notebooks:

```bash
jupyter notebook
```

Then open:
- `emg1.ipynb` for EMG Dataset 1
- `classify.ipynb` for EMG Dataset 2
- `Taiwan.ipynb` for IMU Dataset

---

## 📌 Algorithms Implemented

| Strategy           | Description                                          |
|--------------------|------------------------------------------------------|
| **Baseline**        | Fully supervised model trained on entire dataset     |
| **Random Sampling** | Random sample selection under a limited query budget |
| **ROAR**            | RL-based strategy that queries only informative samples |

---

## 📈 Evaluation Metrics

- Accuracy  
- Macro F1 Score  
- Confusion Matrix  
- Query Budget (labels used)

---

## 🧠 Highlights

- Significant label efficiency using ROAR with minimal drop in accuracy  
- Statistical feature extraction from sliding windows  
- Rich experimental comparison across 3 distinct sensor datasets  

---

## 👩‍💻 Author

Dviteesha/Tanvi Salgaonkar 
MSc Artificial Intelligence  
Goa University  
2024–25

---

## 📚 Citation & Acknowledgements

- ROAR Algorithm: *Reinforcement Learning Based Online Active Learning for Human Activity Recognition — ISWC 2022*  

---
```

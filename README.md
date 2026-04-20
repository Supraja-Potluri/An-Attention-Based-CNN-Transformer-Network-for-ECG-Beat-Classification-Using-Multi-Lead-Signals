# An-Attention-Based-CNN-Transformer-Network-for-ECG-Beat-Classification-Using-Multi-Lead-Signals

## 📌 Overview
This project presents a deep learning-based approach for automated ECG beat classification using multi-lead signals. The model combines Convolutional Neural Networks (CNN), Transformer Encoder, and Attention mechanisms to capture both local waveform features and long-range temporal dependencies in ECG signals.

The system is designed to classify ECG beats into five categories:
- CD (Conduction Disturbance)
- HYP (Hypertrophy)
- MI (Myocardial Infarction)
- NORM (Normal)
- STTC (ST/T Changes)

---

## 🎯 Objectives
- Utilize multi-lead ECG signals for better diagnosis
- Perform R-peak detection and beat segmentation
- Extract meaningful features using CNN
- Capture temporal dependencies using Transformer
- Improve classification accuracy using Attention mechanism

---

## 🧠 Methodology

1. Load raw ECG signals from PTB-XL dataset  
2. Perform R-peak detection  
3. Segment ECG signals into individual beats  
4. Normalize each beat  
5. Split dataset into train, validation, and test sets  
6. Train CNN–Transformer–Attention model  
7. Evaluate performance using standard metrics  

---

## 🏗️ Model Architecture

The architecture consists of:

- **CNN Block**
  - Extracts local waveform features (QRS, peaks, morphology)

- **Transformer Encoder**
  - Captures long-range temporal dependencies

- **Attention Mechanism**
  - Focuses on important ECG signal regions

- **Fully Connected Layer + Softmax**
  - Performs final classification

---

## 📊 Dataset

We used the **PTB-XL dataset**, a large publicly available ECG dataset containing:
- 21,000+ ECG records
- 12-lead signals
- Multiple diagnostic labels

### Citation:
Wagner, P., Strodthoff, N., Bousseljot, R., Samek, W., & Schaeffter, T. (2020).
PTB-XL, a large publicly available electrocardiography dataset.
PhysioNet. https://doi.org/10.13026/x4td-x982

---

## ⚙️ Requirements

### Hardware
- Minimum 8 GB RAM
- GPU (recommended for faster training)

### Software
- Python 3.9
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## 🚀 Execution Steps

```bash
# Clone the repository
git clone https://github.com/Supraja-Potluri/An-Attention-Based-CNN-Transformer-Network-for-ECG-Beat-Classification-Using-Multi-Lead-Signals.git

# Navigate to project folder
cd An-Attention-Based-CNN-Transformer-Network-for-ECG-Beat-Classification-Using-Multi-Lead-Signals

# Install dependencies
pip install -r requirements.txt

# Run the model
python main.py

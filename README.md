# EEG Seizure Detection using CNN-LSTM

## 📌 Abstract

This project focuses on detecting neurological disorders—particularly epilepsy—by analyzing EEG signals using deep learning. A hybrid CNN-LSTM model is employed to extract spatial and temporal features from EEG data obtained from the CHB-MIT Scalp EEG Database. The proposed system is capable of accurately distinguishing between seizure and non-seizure activity, achieving over 80% accuracy. This paves the way for real-time diagnostic tools and wearable device integration for continuous patient monitoring.

---

## 👨‍💻 Team Members

- A. Yashwanth (VTU 21166)  
- M. Rajesh (VTU 21196)  
- A. Pavan Kumar (VTU 21181)  

**Supervisor:** Dr. Ashwini A  
**Department:** Electronics and Communication Engineering  
**Institute:** Vel Tech Rangarajan Dr. Sagunthala R&D Institute of Science and Technology  

---

## 📂 Dataset

- **Name**: EEG Seizure Analysis Dataset  
- **Source**: Subset of CHB-MIT Scalp EEG Database  
- **Samples**: ~54,000 segments labeled as seizure or non-seizure  
- **Sampling Rate**: 256 Hz  
- **Used For**: Binary classification of seizure activity
- https://www.kaggle.com/datasets/adibadea/chbmitseizuredataset

---

## 🧠 Methodology

1. **Data Collection** – EEG data sourced from CHB-MIT dataset (preprocessed subset used)  
2. **Preprocessing** – Bandpass filtering, segmentation, normalization  
3. **Feature Extraction** – Statistical and frequency features  
4. **Model Design** – CNN for spatial features + LSTM for temporal patterns  
5. **Classification** – Binary output: seizure vs non-seizure  

---

## 🛠️ Implementation Details

- **Model**: CNN-LSTM hybrid
- **Loss Function**: Binary Cross-Entropy
- **Optimizer**: Adam
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score, Confusion Matrix

---

## 📊 Results

- **True Positives (TP)**: 1293  
- **True Negatives (TN)**: 1535  
- **False Positives (FP)**: 238  
- **False Negatives (FN)**: 480  
- **Training Accuracy**: 92%  
- **Validation Accuracy**: 79%

> ✅ The model shows strong seizure classification performance and real-world deployment potential.

---

## ✅ Conclusion

- Designed a deep learning system for seizure detection using EEG signals.
- Implemented a hybrid CNN-LSTM model to learn spatial and temporal patterns.
- Achieved high classification accuracy, supporting clinical diagnosis.
- Suitable for integration into real-time and wearable monitoring systems.

---

## 📚 References

1. Thalakola Syamsundararao et al., *Hindawi, 2022*  
2. C. Pappalettera et al., *GeroScience, 2022*  
3. M. Shi et al., *Math Problems in Engg., 2021*  
4. S. Sheykhivand et al., *IEEE Access, 2020*

---

## 🖥️ How to Run

```bash
# Clone the repository
git clone https://github.com/yourusername/eeg-seizure-detection.git
cd eeg-seizure-detection

# Install dependencies
pip install -r requirements.txt

# Train the model
python model_training.py

# Predict on new input
python inference.py --input path_to_input.edf

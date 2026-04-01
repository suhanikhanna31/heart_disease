🫀 Automated Heart Sound Classification Using Deep Learning

📌 Overview

This project presents a deep learning-based system for automatic classification of heart sounds using phonocardiogram (PCG) recordings. The model leverages a hybrid CNN-LSTM architecture to capture both spatial and temporal features from Mel-spectrogram representations of heart sound signals.

The goal is to assist in early detection of cardiovascular abnormalities by distinguishing between normal and abnormal heart sounds.

⸻

🚀 Features
	•	End-to-end pipeline for heart sound classification
	•	Audio preprocessing using Librosa
	•	Feature extraction using Mel-spectrograms
	•	Hybrid CNN + LSTM model architecture
	•	Class imbalance handling using class weights
	•	Threshold optimization using ROC curve & Youden’s Index
	•	Evaluation using accuracy, precision, recall, and F1-score

⸻

🧠 Model Architecture

The model combines:
	•	CNN layers → extract spatial features from spectrograms
	•	LSTM layer → capture temporal dependencies in heart signals
	•	Dense layers → final classification

This hybrid approach improves performance compared to standalone CNN models.

⸻

📊 Dataset
	•	Dataset consists of heart sound recordings from:
	•	set_a
	•	set_b
	•	Labels include:
	•	Normal
	•	Abnormal (murmur, artifact, extrasystole, etc.)

📌 Total samples used: 761
📌 Class distribution handled using weighted training

⸻

⚙️ Methodology
	1.	Data Loading & Label Matching
	•	Fixed dataset mismatch issues using robust filename matching
	2.	Audio Preprocessing
	•	Resampling and noise handling
	3.	Feature Extraction
	•	Conversion to Mel-spectrograms
	4.	Model Training
	•	CNN-LSTM model trained with class weighting
	5.	Threshold Optimization
	•	ROC curve used to determine optimal classification threshold
	6.	Evaluation
	•	Metrics computed on validation set

⸻
Metric      Value(abnormal)


Accuracy    0.64

Precision   0.73

Recall      0.63

F1 Score    0.64




📉 Visualizations
	•	Heart sound processing pipeline
	•	Mel-spectrogram representation
	•	ROC curve with optimal threshold selection

⸻

🛠️ Tech Stack
	•	Python
	•	TensorFlow / Keras
	•	Librosa
	•	NumPy / Pandas
	•	Scikit-learn
	•	Matplotlib


⸻


  ▶️ How to Run
  # Install dependencies
pip install librosa soundfile scikit-learn matplotlib pandas tensorflow

# Run notebook
heart_sounds_project.ipynb

⸻


📂 Project Structure
heart-sound-classification/
│
├── heart_sounds_project.ipynb
├── README.md
├── dataset/
│   ├── set_a/
│   ├── set_b/
│   ├── set_a.csv
│   └── set_b.csv


⸻

⚠️ Challenges & Improvements
	•	Dataset imbalance handled using class weights
	•	Initial dataset mismatch issue resolved through improved file matching
	•	Threshold tuning improved recall for abnormal cases (important in medical diagnosis)

⸻

🔮 Future Work
	•	Integration with real-time stethoscope devices
	•	Use of transformer-based architectures
	•	Explainable AI (XAI) for clinical interpretability
	•	Deployment as a web/mobile application

⸻

👩‍💻 Author

Suhani Khanna

⸻

⭐ Acknowledgment

This project is inspired by research in biomedical signal processing and aims to contribute to accessible healthcare solutions using AI.

⸻







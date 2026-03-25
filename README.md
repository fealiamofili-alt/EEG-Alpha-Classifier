EEG Classification of Alpha-Band Oscillations
Result: 100.00% Classification Accuracy achieved via a Logistic Regression Pipeline.

Neurophysiological Context: The Alpha Blockade
This project focuses on the automated detection of the "Alpha Blockade" phenomenon (the Berger Effect). When a subject’s eyes are closed, the visual cortex within the Occipital Lobe generates synchronized, high-amplitude oscillations at approximately 10Hz, known as the Alpha rhythm. This model identifies that distinct neural signature to differentiate between cognitive states with high precision.

Analysis and Evidence
1. Frequency Domain Analysis (The Alpha "Skyscraper")
Power Spectral Density (PSD) analysis reveals a prominent power spike at the 10Hz frequency during the "Eyes-Closed" state. This stands in stark contrast to the attenuated baseline observed during the "Eyes-Open" state, providing a clear biological feature for the classifier.

2. Spatial Interpretability (AI Feature Importance)
To validate the model's physiological accuracy, the classifier's coefficients were projected back onto a 2D topographical scalp map. The concentrated importance over the Occipital Lobe confirms that the algorithm is correctly prioritizing biological signals from the visual cortex rather than environmental noise or ocular artifacts.

Technical Architecture and Implementation
Primary Library: MNE-Python (Electrophysiological Signal Processing)

Classifier: Scikit-Learn (StandardScaler + Logistic Regression)

Dataset: 64-channel high-density EEG recording

Execution Instructions
Install necessary dependencies: pip install -r requirements.txt

Execute the analysis within the EEG-Alpha-Classifier.ipynb notebook via Anaconda or Jupyter.

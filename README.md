# MarineMamalDet
This project focuses on detecting multiple marine species—including dolphins, seals, and whales—from audio recordings using deep learning. The system is designed to work on polyphonic marine audio, where multiple species may be vocalizing at the same time.

Using a Hybrid CNN + BiLSTM architecture, the model extracts both spatial and temporal features from spectrograms to accurately identify species and estimate their counts within each audio file. This approach combines the strengths of convolutional networks for pattern recognition with recurrent networks for sequence understanding.

**Key Features**
Multi-label species detection: Identifies multiple marine species in a single audio clip.

Species count estimation: Predicts how many distinct vocal events occur for each species.

Hybrid CNN + BiLSTM model:

CNN extracts frequency-time structures from spectrograms

BiLSTM learns temporal dependencies in marine calls

End-to-end pipeline: Includes preprocessing, dataset creation, model training, evaluation, and inference.

Watkins Marine Mammal Sound Database compatible.

**Model Architecture**

CNN Block:
Extracts spatial features from spectrogram images (frequency patterns, harmonics, call shapes)

BiLSTM Block:
Captures long-range temporal patterns like repeated calls, rhythm, or duration variations

Fully Connected Multi-Label Output:
Produces species presence probabilities + count predictions.

**Evaluation Metrics**

Multi-Label Accuracy

F1-Score (per species)

Mean Absolute Error for count prediction

Confusion matrix visualizations

ROC Curves for each species

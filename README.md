## Safety Harness Image Classification
### 📌 Project Overview

This project builds a Convolutional Neural Network (CNN) to classify images of workers as Safe (wearing a harness) or Not Safe (without a harness). The system automates safety compliance monitoring in industrial settings.

### 📂 Dataset Composition

Train/Validation/Test sets split from ~538 labeled images.

- Classes:

  - Safe — worker wearing a harness

  - Not_Safe — worker without a harness

### ⚙️ Workflow

- Data Preparation

Image validation (remove invalid files).

Normalization (pixel values scaled 0–1).

Split into 70% training, 20% validation, 10% testing.

- Model Architecture

CNN with Conv2D, MaxPooling2D, Flatten, and Dense layers.

Activation: ReLU (hidden), Sigmoid (output).

Optimizer: Adam, Loss: Binary Cross-Entropy.

- Training

Trained for 20 epochs with early stopping.

TensorBoard logging enabled for monitoring.

- Evaluation

Metrics on the test set:

Precision: 93.33%

Recall: 82.35%

Accuracy: 87.5%

- Prediction

Loads a new image, resizes it to (256,256), and predicts class label (Safe or Not Safe).

### 📊 Results

The model demonstrates strong precision and balanced recall, making it reliable for safety monitoring.

Example result: Predicted class is Safe.

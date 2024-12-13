# Scene Recognition Using Combined CoAtNet and ResNet Models

This repository contains the implementation of a scene recognition system leveraging the combined power of CoAtNet and ResNet architectures. By integrating fully connected layers on top of their respective heads, the system generates accurate predictions on the Places365-Small dataset.

## Overview

Scene recognition is a crucial task in computer vision, enabling systems to classify and understand various environments. This project combines the strengths of CoAtNet and ResNet models by:

1. Extracting features from both architectures.
2. Adding fully connected layers to merge these features.
3. Generating robust predictions for scene classification.

## Features

- **Model Fusion**: Integrates outputs of CoAtNet and ResNet for improved accuracy.
- **Dataset**: Utilizes the Places365-Small dataset, a standard benchmark for scene recognition.
- **Customizable**: Easy-to-adapt architecture for other datasets and tasks.

## Requirements

- Python 3.7+
- TensorFlow or PyTorch (depending on the implementation specifics)
- NumPy
- Matplotlib
- Places365 dataset

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/coatnet-resnet-places365.git
   ```

2. Navigate to the project directory:
   ```bash
   cd coatnet-resnet-places365
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Dataset Preparation

1. Download the Places365-Small dataset from [Places365](http://places2.csail.mit.edu/download.html).
2. Extract the dataset and organize it as follows:
   ```
   dataset/
   |-- train/
   |-- val/
   |-- test/
   ```
3. Update the dataset path in the code.

## Model Architecture

The model integrates CoAtNet and ResNet as follows:

1. **Feature Extraction**:
   - CoAtNet and ResNet extract high-level features from input images.
   - The outputs of both models are flattened.
2. **Feature Fusion**:
   - Fully connected layers combine these features.
3. **Classification**:
   - The final output layer predicts the scene class.

## Training

To train the model, execute the following command:

```bash
python train.py
```

### Training Parameters

- **Batch Size**: Default is 32.
- **Epochs**: Default is 20.
- **Learning Rate**: Configurable via the training script.

## Evaluation

Evaluate the trained model on the validation dataset:

```bash
python evaluate.py
```

The script provides metrics such as accuracy and confusion matrix.

## Results

The combined model achieves significant improvements over standalone CoAtNet or ResNet models. Results will be updated in this section with detailed metrics.

## Usage

To use the model for inference:

1. Place the input images in a directory.
2. Run the inference script:
   ```bash
   python inference.py --input_dir /path/to/images --output_dir /path/to/results
   ```

## Contributions

Contributions are welcome! If you have ideas for improvement or encounter issues, please open an issue or submit a pull request.


## Acknowledgments

- [Places365 Dataset](http://places2.csail.mit.edu/download.html)
- CoAtNet and ResNet authors for their groundbreaking architectures.



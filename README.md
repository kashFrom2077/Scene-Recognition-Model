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
- PyTorch (depending on the implementation specifics)
- fastai



## Clone the repository:
   ```bash
   git clone https://github.com/kashFrom2077/Scene-Recognition-Model.git
   ```


## Note that the .pkl file for pre trained the coatnet and .pth file for resnet is given. Coatnet is trained using fastai. 



## Model Architecture

The model integrates CoAtNet and ResNet as follows:

1. **Feature Extraction**:
   - CoAtNet and ResNet extract high-level features from input images.
   - The outputs of both models are flattened.
2. **Feature Fusion**:
   - Fully connected layers combine these features.
3. **Classification**:
   - The final output layer predicts the scene class.





## Contributions

Contributions are welcome! If you have ideas for improvement or encounter issues, please open an issue or submit a pull request.


## Acknowledgments

- [Places365 Dataset](http://places2.csail.mit.edu/download.html)
- CoAtNet and ResNet authors for their groundbreaking architectures.



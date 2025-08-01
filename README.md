# SAR Image Colorization

This project focuses on the colorization of grayscale Synthetic Aperture Radar (SAR) images using advanced deep learning models. By leveraging DCGAN (Deep Convolutional Generative Adversarial Network) and UNet architectures, the system converts single-channel SAR images into realistic color images.

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Model Architectures](#model-architectures)
- [Dataset](#dataset)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Overview

Synthetic Aperture Radar (SAR) imagery is widely used in remote sensing and earth observation. However, SAR images are typically grayscale, which can make interpretation challenging for human observers. The goal of this project is to automate the process of converting grayscale SAR images into colorized versions, enhancing visual interpretation while preserving important features.

This is accomplished by training two deep learning models:
- **UNet** for pixel-wise colorization, capturing fine image details.
- **DCGAN** for generating realistic textures and enhancing the realism of the colorized images.

## Key Features

- Automatic colorization of grayscale SAR images
- Combines the strengths of UNet and DCGAN models
- End-to-end training pipeline
- Easily customizable and extendable
- Code written in Python, using popular machine learning libraries

## Model Architectures

### UNet

UNet is a convolutional neural network designed for image-to-image translation tasks. It employs an encoder-decoder structure with skip connections, allowing it to capture both local and global features for precise colorization.

### DCGAN

DCGAN is a type of Generative Adversarial Network (GAN) that uses convolutional layers. It consists of a generator and a discriminator that are trained together, with the generator aiming to produce realistic colorized images and the discriminator trying to distinguish between real and generated images.

## Dataset

You will need a dataset of paired grayscale SAR images and their corresponding color images for training and validation. Publicly available SAR datasets or your own collected data can be used.

## Getting Started

### Prerequisites

- Python 3.7+
- PyTorch or TensorFlow (depending on implementation)
- numpy, matplotlib, pillow, and other required libraries (see `requirements.txt`)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sar-image-colorization.git
   cd sar-image-colorization
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Usage

1. Prepare your dataset and update the configuration paths as needed.
2. Train the model:
   ```bash
   python train.py
   ```
3. Colorize new SAR images:
   ```bash
   python colorize.py --input path/to/grayscale_sar.png --output path/to/colorized_result.png
   ```

## Results

Below is a comparison of the grayscale SAR input, the predicted color output, and the actual color reference:

![image1](image1)

| Grayscale SAR Image | Predicted Color | Actual Color |
|---------------------|-----------------|-------------|
|         Left        |     Center      |    Right    |

## Contributing

Contributions, bug reports, and feature requests are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For queries or collaborations, please contact [yourname](mailto:your.email@example.com) or visit the [GitHub repository](https://github.com/yourusername/sar-image-colorization).

---
_Bringing color to SAR imagery using deep learning!_

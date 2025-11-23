### Fake-Images-Using-Generative-Adversarial-Network
## Generating Fake Images Using DCGAN &amp; StyleGAN 


## Overview

Generate realistic human face images using DCGAN and StyleGAN models in Python with Keras and TensorFlow.

![Generated Faces][1]

## Features

- Train a DCGAN or StyleGAN on custom face datasets.
- Generate new face images with controllable styles and variations.
- Save and visualize results as images and GIFs.

## Dataset

- Download the CelebA dataset from Kaggle for training:
  - https://www.kaggle.com/datasets/jessicali9530/celeba-dataset/data[2]

## References

- DCGAN project tutorial:  
  - https://towardsdatascience.com/fake-face-generator-using-dcgan-model-ae9322ccfd65[2]
- StyleGAN implementation code:  
  - https://github.com/longluu/DL-styleGAN-faceForVisualExperiment[2]

## Requirements

- Python 3.x
- TensorFlow
- Keras
- numpy
- imageio
- matplotlib

Install required packages:
```bash
pip install tensorflow keras numpy imageio matplotlib
```

## Usage

1. Download the CelebA dataset and place images in a `data/` folder.
2. Run the code in `Style_GAN.ipynb` to train the GAN and generate faces.
   - Training and generation code is provided with step-by-step cells.
3. Generated sample faces and training GIFs will be saved automatically.

## Quick Example

```python
from keras.models import Model
from keras.layers import Input, Dense, Reshape, Conv2DTranspose, Flatten, Dropout, LeakyReLU
import numpy as np

# Build generator and discriminator (see notebook for full code)
# ...[code in Style_GAN.ipynb]

# Train and save generated faces
# ...[code in Style_GAN.ipynb]
```

## Outputs

- Example of generated faces:  
  ![Faces Output][1]
- Training progress and losses are auto-plotted.

# Autoencoders using Handwritten Digit

This project implements an **Autoencoder neural network** to compress and reconstruct handwritten digit images from the MNIST dataset.  
The model learns an efficient lower-dimensional representation of images and reconstructs them from compressed features.

## Project Overview

Autoencoders are unsupervised neural networks used for:

- Dimensionality reduction
- Feature learning
- Image compression
- Noise removal

In this project, an autoencoder is trained on the **MNIST handwritten digit dataset** to learn compressed representations of images and reconstruct them.

## Dataset

The project uses the **MNIST dataset**, which contains:

- 60,000 training images
- 10,000 testing images
- Image size: **28 × 28 pixels**
- Grayscale handwritten digits (0–9)

Dataset Source:
Keras built-in dataset loader.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- TensorFlow / Keras

## Model Architecture

The autoencoder consists of three main parts:

### Encoder
Compresses the input image into a lower dimensional representation.

### Decoder
Reconstructs the image from compressed features.

Input Layer (784 neurons)

↓

Dense Layer (256 neurons, ReLU)
↓

Bottleneck Layer (100 neurons, ReLU)
↓

Dense Layer (256 neurons, ReLU)
↓

Output Layer (784 neurons, Sigmoid)

## Data Preprocessing

Steps performed:

1. Load MNIST dataset
2. Normalize pixel values (0–255 → 0–1)
3. Reshape images from **28×28 → 784 vector**
4. Visualize sample training images

## Model Training

The model is trained using:

- Optimizer: **Adam**
- Loss Function: **Binary Crossentropy**
- Epochs: **10**

The model learns to reconstruct the input image from compressed features.

## Results

The project visualizes three outputs:

- Original handwritten digits
- Encoded representation (compressed features)
- Reconstructed images produced by the autoencoder

The reconstructed images closely resemble the original handwritten digits, demonstrating effective dimensionality reduction.

## Project Workflow

1. Import libraries
2. Load MNIST dataset
3. Normalize and reshape images
4. Build autoencoder architecture
5. Train the model
6. Generate encoded representations
7. Reconstruct images
8. Visualize results

## How to Run the Project

Clone the repository: git clone https://github.com/BhavanaTallapaka/Autoencoders-using-Handwritten-Digit.git

Install dependencies: pip install numpy pandas matplotlib seaborn tensorflow keras

Run the notebook: jupyter notebook

Open the notebook and execute the cells.

## Future Improvements

Possible improvements include:

- Using **Convolutional Autoencoders**
- Increasing training epochs
- Adding noise for **denoising autoencoders**
- Visualizing latent space representations
- Applying autoencoders for anomaly detection

## Author

Bhavana Tallapaka  
Computer Science Student  

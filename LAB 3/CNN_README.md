# Convolutional Neural Network for MNIST Digit Classification

## Program Title

**Handwritten Digit Classification using Convolutional Neural Network (CNN)**

## Aim

To develop and train a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify handwritten digits from 0 to 9.

## Dataset Used

The **MNIST handwritten digit dataset** is used. It contains grayscale images of handwritten digits.

* Image size: **28 × 28 pixels**
* Number of classes: **10 (digits 0–9)**
* Training images: **60,000**
* Testing images: **10,000**
* Pixel values are normalized to the range **0 to 1**.

## Model Used

The CNN consists of:

* Three `Conv2D` layers with ReLU activation
* Two `MaxPooling2D` layers
* One `Flatten` layer
* One Dense layer with 64 neurons
* Final Dense layer with 10 neurons and Softmax activation

The model is compiled using the **Adam optimizer** and **Sparse Categorical Cross-Entropy** loss.

## Results

The model is trained for **5 epochs**. The program evaluates the model on the MNIST test dataset and prints the **test accuracy**.

Training and validation **accuracy** and **loss** are also plotted using Matplotlib. The graphs help observe how the model learns during training.

The exact test accuracy is generated when the program is executed and may vary slightly depending on the environment.

# MNIST Digit Classification Using LSTM

## Program Title
Handwritten Digit Recognition using a Long Short-Term Memory (LSTM) Neural Network.

## Aim
To build and train an LSTM-based deep learning model that recognises handwritten digits (0–9) from the MNIST dataset.

## Dataset Used
- **MNIST** handwritten digit dataset.
- 60,000 training images and 10,000 test images.
- Each image is a 28 × 28 grayscale image.
- Pixel values are normalised to the range [0, 1].
- Labels are converted into one-hot encoded vectors for the 10 digit classes.

## Methodology
1. Import TensorFlow/Keras, MNIST, and Matplotlib.
2. Load the MNIST training and testing datasets.
3. Normalise image pixel values by dividing by 255.
4. Reshape each image into a sequence of 28 time steps, with 28 features per time step.
5. One-hot encode the digit labels.
6. Build a Sequential model containing:
   - An LSTM layer with 64 units and ReLU activation.
   - A Dense output layer with 10 neurons and softmax activation.
7. Compile the model using the Adam optimiser, categorical cross-entropy loss, and accuracy metric.
8. Train for 5 epochs with a batch size of 128.
9. Evaluate the model on the test dataset and plot training and validation accuracy.

## Results
The model achieved a **test accuracy of 97.14%** after 5 epochs. The recorded validation accuracy improved across training, reaching 97.14% in the fifth epoch. This indicates that the LSTM model learned to classify handwritten digits effectively on the MNIST test set.

## Requirements
- Python 3
- TensorFlow / Keras
- Matplotlib
- Jupyter Notebook

## How to Run
1. Open the notebook `1BM24CD027_Karan_Kumar_N_Program_5(1).ipynb` in Jupyter Notebook or Google Colab.
2. Run the cells from top to bottom.
3. If required, install the dependencies:
   ```bash
   pip install tensorflow matplotlib
   ```
4. The MNIST dataset is downloaded automatically by Keras when it is first loaded.


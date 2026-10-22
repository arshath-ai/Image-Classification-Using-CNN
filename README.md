<<<<<<< HEAD
# Image Classification Using CNN

A Deep Learning project that classifies images into two categories: **Thanos** and **Joker**, using a Convolutional Neural Network (CNN) built with Python and Keras.

## Project Overview

This project uses image classification to identify whether an input image belongs to the Thanos or Joker class. The CNN learns image features from a labeled dataset and predicts the class of unseen images.

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Convolutional Neural Network (CNN)
- ImageDataGenerator
- OpenCV-compatible image workflows

## Model Architecture

The CNN consists of the following layers:

1. **Convolutional Layer:** Extracts image features using 32 filters of size 3 × 3.
2. **Max Pooling Layer:** Reduces the spatial dimensions of feature maps.
3. **Flatten Layer:** Converts feature maps into a one-dimensional vector.
4. **Dense Layer:** Uses 128 neurons with ReLU activation.
5. **Output Layer:** Uses one neuron with sigmoid activation to classify images into two classes.

### Model Configuration

- Input image size: 64 × 64 pixels
- Input channels: 3 (RGB)
- Optimizer: Adam
- Loss function: Binary cross-entropy
- Evaluation metric: Accuracy
- Batch size: 8
- Training epochs: 50

## Project Structure

```text
Image-Classification/
├── Dataset/
│   ├── train/
│   │   ├── Joker/
│   │   └── Thanos/
│   ├── val/
│   │   ├── Joker/
│   │   └── Thanos/
│   └── test1/
├── train.py
├── predict.py
├── model.json
├── model.h5
├── requirements.txt
├── .gitignore
└── README.md
```

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Image-Classification.git
cd Image-Classification
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```powershell
.\venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

## Training the Model

Make sure the training and validation datasets are organized into class-specific folders.

Run:

```bash
python train.py
```

The training script trains the CNN and saves the model architecture in `model.json` and the model weights in `model.h5`.

## Predicting Images

Place test images in the test directory and update the directory path in `predict.py` if necessary.

Run:

```bash
python predict.py
```

The program prints the predicted class for each image.

## Data Preprocessing

The training pipeline resizes images to 64 × 64 pixels and rescales pixel values to the range 0–1. It also applies data augmentation, including shear transformations, zooming, and horizontal flipping.

Validation images are resized and rescaled without augmentation.

## Applications

- Image recognition
- Computer vision learning
- CNN and deep learning practice
- Binary image classification

## Future Improvements

- Improve model accuracy using a larger and more diverse dataset.
- Add additional convolutional and pooling layers.
- Display predictions with confidence scores.
- Build a web interface for uploading and classifying images.
- Evaluate the model using precision, recall, and a confusion matrix.

## Author

**Seyyadh Arshath**

GitHub: https://github.com/arshath-ai

## License

This project is intended for educational and learning purposes.
=======
# Image-Classification-Using-CNN
>>>>>>> 364689e1e4be3d0f3947c88f3ebf765be9e53536

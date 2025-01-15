# Detection Faces

## Description
This project implements a facial detection and recognition system using TensorFlow and OpenCV. The system detects faces from images, processes them, and classifies them into predefined categories using a trained neural network.

## Features
- Detects faces in images using OpenCV's Haar Cascade Classifier.
- Preprocesses detected faces for input into a TensorFlow-based neural network.
- Classifies faces into predefined categories.
- Visualizes detection and recognition results, saving output images with labeled faces.

## Requirements
To run this project, you need the following dependencies:

- Python
- TensorFlow
- OpenCV
- Matplotlib
- NumPy
- PIL
- Google Colab (optional, for running in the cloud)

Install the required libraries using:
```bash
pip install opencv-python opencv-python-headless opencv-contrib-python tensorflow matplotlib
```

## Setup
1. Extract the provided dataset (e.g., `data_1.zip`) and ensure the folder structure matches the following:
   ```
   data/
   ├── train/
   ├── train_faces/
   ├── valid/
   ├── test/
   ```
2. Train images should be placed under `train/` subfolders, where each subfolder corresponds to a class label.
3. The test images should be placed under `test/` for recognition.

## How to Run
### 1. Train the Model
The script preprocesses the dataset, trains a convolutional neural network (CNN) using TensorFlow, and evaluates it on a validation set.

### 2. Detect and Recognize Faces
Run the script to detect faces in the test images. Detected faces will be labeled with their respective class names and saved as an output image (`output_image.jpg`).

### 3. Save and Load the Model
The trained model is saved as `model_cast.h5` for future use.

## Results
- Accuracy and loss during training are visualized.
- Final outputs show labeled faces with predicted class names on the test images.

## Example Output
![Example Output](path/to/output_image.jpg)

## Additional Information
- The classification categories used in the script are:
  - Amy
  - Bernadete
  - Leonard
  - Penny
  - Raj
  - Sheldon

- Modify the `classificationImage` function and `classes` list to adapt to your dataset.

## Notes
- Ensure the dataset is properly labeled and organized for best results.
- The `face_cascade` settings (e.g., `scaleFactor`, `minNeighbors`) can be adjusted for better detection performance.

---
Feel free to customize this README based on your specific project requirements.

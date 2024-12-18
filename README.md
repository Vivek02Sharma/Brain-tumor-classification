# Brain Tumor Classification App

This **Streamlit** web application classifies brain tumor types based on MRI images. It uses a pre-trained Convolutional Neural Network (CNN) model to predict the presence and type of brain tumor, including Glioma, Meningioma, Pituitary tumors, or No tumor.

## 🛠 Features

- **User Input**: Upload an MRI image of the brain (grayscale).
- **Model Prediction**: Classifies the brain tumor into one of the four classes:
  - Glioma (Class 0)
  - Meningioma (Class 1)
  - No Tumor (Class 2)
  - Pituitary Tumor (Class 3)
- **Prediction Probability**: Displays the probability of each classification.
- **Image Preprocessing**: Automatically converts color images to grayscale and resizes them to match the model’s input dimensions.

## 🚀 Getting Started

### Prerequisites

To run this project locally, you'll need:

- **Python 3.7+**
- **pip** (Python package manager)
- **Streamlit** for the web interface
- **TensorFlow** for model prediction
- **Pillow** for image handling

### Installation

1. Create a virtual environment:
    ```bash
    python -m venv env
    ./env/Scripts/activate
    ```

2. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```

### Running the Application

To run the Streamlit app, use the following command:

```bash
streamlit run main.py
```

## 🔧 How It Works

1. **Image Upload**: The user uploads an MRI image of the brain.
2. **Preprocessing**: The app converts the uploaded image to grayscale (if necessary) and resizes it to the required dimensions (300x300).
3. **Model Prediction**: The app uses a pre-trained CNN model to classify the tumor type (Glioma, Meningioma, No Tumor, or Pituitary).
4. **Results Display**: The app shows the predicted tumor class and the probability of the classification.

## 📊 Model Used

The app uses a **Convolutional Neural Network (CNN)** to classify brain tumors into one of four categories:

- **Glioma (Class 0)**
- **Meningioma (Class 1)**
- **No Tumor (Class 2)**
- **Pituitary Tumor (Class 3)**

The CNN model consists of several layers:
- **Convolutional Layers**: Extract features from the input images.
- **Max Pooling Layers**: Reduce the spatial dimensions.
- **Fully Connected Layers**: Learn high-level representations of the features.
- **Softmax Output Layer**: Produces probabilities for each of the four classes.

The model is trained using a dataset of MRI images of brains with various tumor types and is designed to predict the tumor type based on new inputs.

## 📂 Directory Structure

```
Brain-Tumor-Classification-App/
├── brain-tumor-dataset/
├── model/
│   └── brain-tumor-model.h5
├── train.py
├── main.py
├── requirements.txt
└── README.md
```

## 🔧 Dependencies

All required dependencies are listed in the `requirements.txt` file. You can install them using:
```
pip install -r requirements.txt
```

### Key dependencies:

`streamlit`
`numpy`
`tensorflow`
`matplotlib`

## 📸 Screenshots

### App Interface:
![image1](https://github.com/user-attachments/assets/60d0fe93-f3e4-45f9-b639-b40b740bf6d6)

### Prediction Results:
![image2](https://github.com/user-attachments/assets/61f539b5-08c7-4383-af6a-d4d03ad770ff)

## 🧑‍💻 How to Train the Model (Optional)

- Run the `train.py` script:
  
```
python train.py
```

This will retrain the model and save the updated `brain-tumor-model.h5` file in the `model/` folder.

## 🔄 Example
### Input:
- MRI Image of a brain scan (upload your own image).
  
### Output:
```
Prediction: Meningioma
Prediction Probability: 99.59%
```

## 💬 Feedback & Contributions
Feel free to open an issue or pull request if you encounter any problems or have suggestions for improvements.

## 🎉 Acknowledgments
- **Streamlit**: A great framework for creating web applications.
- **Keras/TensorFlow**: Used for training and building the neural network model.

## 👨‍💻 Created By

[Vivek Sharma](https://github.com/Vivek02Sharma).

**Thank you** for checking out the project!
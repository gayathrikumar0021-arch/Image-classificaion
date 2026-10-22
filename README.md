🖼️ Image Classification Using Hugging Face Transformers

📌 Project Overview

This project demonstrates image classification using a pre-trained deep learning model from the Hugging Face Transformers library.

The model analyzes an input image and predicts the most likely object categories. It returns classification labels along with confidence scores, making it easy to understand the model's predictions.

The project is implemented in Python using Jupyter Notebook and demonstrates how pre-trained AI models can be used without training a model from scratch.

🎯 Objectives

Understand image classification using deep learning.

Explore pre-trained models available on Hugging Face.

Load and classify images using Python.

Display the top 3 predicted classes.

Interpret model predictions using confidence scores.

Learn how to use PyTorch and Transformers for computer vision tasks.

✨ Features

Uses a pre-trained image classification model.

Supports common image formats such as JPG and PNG.

Processes images using a Transformers image-classification pipeline.

Displays the top 3 predictions.

Shows confidence scores for each prediction.

Runs experiments in Jupyter Notebook.

Demonstrates transfer learning through pre-trained model inference.

🛠️ Technologies Used

Technology

Purpose

Python

Programming language

PyTorch

Deep learning framework

Hugging Face Transformers

Loading and running the model

Pillow (PIL)

Loading and processing images

Jupyter Notebook

Running the experiment

🧠 Model Information

This project uses a pre-trained image classification model available through the Hugging Face Hub.

Task: Image Classification

Model source: Hugging Face Hub

Framework: PyTorch

Output: Predicted labels and confidence scores

Model name: Check the model argument in your notebook's pipeline initialization to identify the exact model used in your experiment.

For example, google/vit-base-patch16-224 is a pre-trained Vision Transformer model that can be used for image classification. Use this identifier only if it matches your actual notebook configuration.

🔄 Project Workflow

Import the required Python libraries.

Initialize the image classification pipeline.

Load an image from a local file.

Pass the image to the pre-trained model.

Generate predictions.

Select the top 3 predictions.

Display the predicted labels and confidence scores.

⚙️ Installation and Setup

Prerequisites

Python

Jupyter Notebook or JupyterLab

Internet connection for downloading the model the first time, unless it is already cached locally

Step 1: Clone the Repository

git clone https://github.com/gayathrikumar0021-arch/Image-classificaion.git

Step 2: Open the Project Folder

cd Image-classificaion

Step 3: Install Dependencies

pip install torch transformers pillow jupyter

Step 4: Launch Jupyter Notebook

jupyter notebook

Open the project notebook and execute the cells in order.

💻 Example Code

The following example demonstrates image classification using a pre-trained Hugging Face model.

1. Import Libraries

from transformers import pipeline
from PIL import Image

2. Load the Classification Model

classifier = pipeline("image-classification")

3. Load an Image

image = Image.open("your_image.jpg").convert("RGB")

Replace your_image.jpg with the path to an actual image on your computer.

4. Generate Predictions

results = classifier(image, top_k=3)

for result in results:
    print(f"{result['label']}: {result['score']:.2%}")

Example Output

golden retriever: 92.45%
Labrador retriever: 4.21%
cocker spaniel: 1.83%

The output above is illustrative only. Actual labels and confidence scores depend on the input image and model.

📊 Understanding the Results

Label: The category predicted by the model.

Score: The model's confidence score for that category.

Top 3 predictions: The three highest-scoring categories returned by the model.

A higher score indicates that the model assigns more confidence to that label. It does not guarantee that the prediction is correct.

📁 Project Structure

Image-classificaion/
│
├── image_classification.ipynb
├── images/
│   └── sample.jpg
└── README.md

This is an example structure. Update the filenames and folders to match your actual repository.

🚀 Applications

Image classification can be applied to:

Object recognition

Plant and animal identification

Product categorization

Image organization

Educational computer vision projects

Visual data analysis

🔮 Future Enhancements

Build a simple web interface for uploading images.

Display prediction results with visual confidence charts.

Compare different pre-trained image classification models.

Add batch image classification.

Explore fine-tuning with a custom dataset.

Extend the project to image detection and other computer vision tasks.

⚠️ Limitations

Predictions depend on the model's training data and supported classes.

Unfamiliar images may produce incorrect predictions.

Confidence scores should not be interpreted as guaranteed accuracy.

The initial model download requires an internet connection if the model is not already cached.

Performance depends on the model, image quality, and available computing resources.

📚 References

Hugging Face Transformers Documentation

Hugging Face Image Classification Models

PyTorch Documentation

👩‍💻 Author

Gayathri Kumar

GitHub: gayathrikumar0021-arch

Project Repository: Image Classification

⭐ If you find this project useful, consider starring the repository!

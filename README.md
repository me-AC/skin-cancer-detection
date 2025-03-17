# Skin Cancer Detection Using MobileNet

This project utilizes the MobileNet architecture to detect and classify skin cancer from images. The goal is to provide an efficient and accurate method for early detection, aiding in timely medical interventions.

## Introduction

Skin cancer is one of the most common types of cancer worldwide. Early detection significantly increases the chances of successful treatment. This project leverages deep learning techniques, specifically the MobileNet architecture, to classify skin lesions as benign or malignant.

## Dataset

The model is trained on the HAM10000 dataset.

### From Author of HAM10000 
Training of neural networks for automated diagnosis of pigmented skin lesions is hampered by the small size and lack of diversity of available dataset of dermatoscopic images. We tackle this problem by releasing the HAM10000 ("Human Against Machine with 10000 training images") dataset. We collected dermatoscopic images from different populations, acquired and stored by different modalities. The final dataset consists of 10015 dermatoscopic images which can serve as a training set for academic machine learning purposes. Cases include a representative collection of all important diagnostic categories in the realm of pigmented lesions: Actinic keratoses and intraepithelial carcinoma / Bowen's disease (akiec), basal cell carcinoma (bcc), benign keratosis-like lesions (solar lentigines / seborrheic keratoses and lichen-planus like keratoses, bkl), dermatofibroma (df), melanoma (mel), melanocytic nevi (nv) and vascular lesions (angiomas, angiokeratomas, pyogenic granulomas and hemorrhage, vasc).

## Model Architecture

MobileNetV2, known for its efficiency on mobile and embedded vision applications, serves as the backbone of our model. Its depthwise separable convolutions reduce the number of parameters, making it suitable for real-time applications without compromising accuracy.

## Training

The dataset was split into training and testing sets. Data augmentation techniques such as random rotations, flips, and color jittering were applied to enhance model generalization. The model was trained using the Adam optimizer with a learning rate of 0.001 and a batch size of 32 for 10 epochs.

## Evaluation

The model achieved a testing accuracy of 96.94%, demonstrating its effectiveness in classifying different types of skin lesions. Detailed evaluation metrics, including precision, recall, and F1-score, are available in the evaluation section of this repository.


## Results

The model's performance metrics are as follows:

- **Accuracy:** 94.22%
- **Precision:** Detailed per class in the evaluation section
- **Recall:** Detailed per class in the evaluation section
- **F1-Score:** Detailed per class in the evaluation section


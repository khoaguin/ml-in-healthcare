# Week 1 - Disease Detection with Computer Vision
In this week, we will practice classifying diseases on chest x-rays images using a neural network.

## Labs
### [Lab 01: Data Exploration & Image Preprocessing](./labs/C1_W1_Lab_1_data_exploration_and_image_preprocessing.ipynb)
In this first lab, we'll get a chance to explore the [ChestX-ray8 dataset](https://arxiv.org/abs/1705.02315) and familiarize ourselves with some of the techniques we'll use in the first graded assignment.

<img src="./images/xray-image.png" alt="drawing" width="200"/>

### [Lab 02: Counting Labels & Weighted Loss Function](./labs/C1_W1_Lab_2_counting_labels_and_weighted_loss_function.ipynb)
In this second lab, we learn how to use the weighted loss technique to deal with the class imbalance problem which often occur in medical datasets. 

<img src="./images/counting_labels.png" alt="drawing" width="350"/>

### [Lab 03: DenseNet](./labs/C1_W1_Lab_3_densenet.ipynb)
In this lab, we briefly walk through [DenseNet](https://arxiv.org/pdf/1608.06993.pdf) - the convolutional network that we are going to use for X-ray image classification in the assignment.

<img src="./images/densenet.png" alt="drawing" width="350"/>

### [Lab 04: Patient Overlap & Data Leakage](./labs/C1_W1_Lab_4_patient_overlap_and_data_leakage.ipynb)
Patient overlap refers to the problem of having data examples of the same patient in different data splits, e.g. the training split and the test split. Deep learning models can memorize specific features of this patient's data and uses these information when doing predictions on the test split. This leads to the problem of over-optimistic results on the test split, and also data leakage. In this lab, we learn how to tackle this challenge.

<img src="./images/patients-overlap.jpg" alt="drawing" width="250"/>

## [Assignment: Chest X-Ray Medical Diagnosis with Deep Learning](./assignment)
![](./images/xray-header-image.png)

In this week's [assignment](./assignment/C1_W1_Assignment.ipynb), we will walk through some of the steps of building and evaluating a chest X-ray classifier using Keras. In particular, we will:
- Pre-process and prepare a real-world X-ray dataset.
- Use transfer learning to retrain a DenseNet model for X-ray image classification.
- Learn a technique to handle class imbalance
- Measure diagnostic performance by computing the AUC (Area Under the Curve) for the ROC (Receiver Operating Characteristic) curve.
- Visualize model activity using GradCAMs.
### Requirements
`keras==2.3.1`  
`tensorflow==1.15.0`
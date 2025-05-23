# Soil Image Classification Challenge – Annam.ai @ IIT Ropar

This repository contains the complete workflow for a soil image classification project using deep learning, submitted to the Soil Classification Challenge organized by Annam.ai at IIT Ropar.

## Objective

Classify soil images into one of the four categories:
- Alluvial soil
- Black soil
- Clay soil
- Red soil

The evaluation metric is the minimum F1-score across all classes, encouraging balanced accuracy.

## Model Overview

Model: ResNet18 (transfer learning)  
Framework: PyTorch  
Training Accuracy: 99.36 percent  
Validation Accuracy: 100.00 percent

Final F1-Scores (per class):  
Alluvial soil: 1.00  
Black soil: 1.00  
Clay soil: 1.00  
Red soil: 1.00  

Minimum F1 Score: 1.00

## Dataset

Images are classified into 4 soil types:  
Alluvial soil, Black soil, Clay soil, Red soil

Input format:  
A CSV file with columns: image_id, soil_type

## Preprocessing

- Resize images to 224x224
- Normalize using ImageNet mean and standard deviation
- Stratified train-validation split for balanced classes

## Training Details

- Loss Function: CrossEntropyLoss
- Optimizer: Adam
- Epochs: 5
- Early stopping on validation accuracy
- Best model saved automatically

## Submission Format

The final submission file, submission.csv, contains the following columns:

image_id,soil_type

Example:

image_id,soil_type
img_abc123.jpg,Alluvial soil
img_xyz456.jpg,Red soil


## Evaluation Script

Classification report generated using sklearn's classification_report method on the validation set.

## Results Summary

| Soil Type       | Precision | Recall | F1-Score | Support |
|-----------------|-----------|--------|----------|---------|
| Alluvial soil   | 1.00      | 1.00   | 1.00     | 53      |
| Black soil      | 1.00      | 1.00   | 1.00     | 23      |
| Clay soil       | 1.00      | 1.00   | 1.00     | 20      |
| Red soil        | 1.00      | 1.00   | 1.00     | 27      |
| Accuracy        |           |        | 1.00     | 123     |

## How to Run

1. Clone the repository
2. Install dependencies
3. Run the training script to train the model
4. Generate submission.csv for final predictions

## Acknowledgments

Competition hosted by Annam.ai  
Dataset and challenge organized at IIT Ropar  
Model built using PyTorch and Torchvision

**Credits**
Task	                                              Contributor

Problem Understanding & Metric Interpretation	      Santhosh Kandagatla
Data Loading & Preprocessing	                      Santhosh Kandagatla
Model Building (ResNet18, PyTorch)	                Santhosh Kandagatla
Training & Evaluation (Loss, Accuracy, F1-score)	  Santhosh Kandagatla
Prediction & CSV Generation	                        Santhosh Kandagatla
Final Submission Preparation	                      Santhosh Kandagatla
Report / README Documentation                      	Santhosh Kandagatla

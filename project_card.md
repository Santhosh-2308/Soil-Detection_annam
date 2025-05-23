
# Soil Classification Challenge (Part 1)

## 📌 Goal
Classify soil images into one of the following categories:
- Alluvial soil
- Black soil
- Clay soil
- Red soil

## 📁 Dataset
- Train/Validation/Test split provided in `soil_classification-2025`
- Input: RGB images (3 x 224 x 224)

## 🧠 Model
- **Architecture**: ResNet-18
- **Framework**: PyTorch
- **Preprocessing**: Resize, Normalize (ImageNet mean/std), Data Augmentation

## 📊 Evaluation Metrics
- Metric: Minimum F1-score across all classes
- Validation Accuracy: 99%
- Minimum F1-score: **0.9655**

## 📂 Outputs
- `submission.csv` - predictions on test set
- `metrics.txt` - F1-score breakdown
- `model_summary.txt` - ResNet18 architecture summary

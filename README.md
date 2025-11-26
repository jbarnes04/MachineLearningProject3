# Machine Learning Project 3 - CNNs

This repository contains a Convolutional Neural Network (CNN) to classify images into two categories: official University of Arkansas logo vs. not official logo. The workflow includes dataset creation, preprocessing, model training, hyperparameter tuning, evaluation, and final model export.

The project uses images that were manually collected from Google Images, Etsy, Pinterest, and the official school website. They were sorted into two folders, official and unofficial.  Official contains official Razorback logo variations and unofficial contains merchandise, alternate Arkansas graphics, and unrelated pig images.

---

## Features
- CNN for binary classification
- Automatic image conversion to .jpg
- Dataset preprocessing with resizing to 500x500
- Hyperparameter tuning across multiple candidate models
- Train/validation/test split
- Model saving in required '.ph' format
---

## Project Structure
```
.
├── Group_26_Project3_Code.ipynb   # Jupyter notebook with full code
├── Images/                        # Official and unofficial logo images
├── Group_26_CNN_FullModel.ph      # Saved final CNN model
└── README.md
```

---

## Installation

Clone the repository:  
```bash
git clone https://github.com/jbarnes/MachineLearningProject3.git
cd your-repo-name
```

Install dependencies:
```bash
pip install -r requirements.txt
```

**Requirements:**
- Python 3.9+
- PyTorch
- Torchvision
- NumPy
- Pillow (with AVIF plugin)
- Matplotlib
---

## Usage
1. Place your dataset into the Images/ folder
2. Run the provided notebook
3. The notebook will:
- Convert images to .jpg
- Resize to 500x500
- Load the dataset with ImageFolder
- Train multiple CNN models
- Select the best model based on validation accuracy
- Evaluate on the test dataset
- Save final model as models/Group_26_CNN_FullModel.ph
---

## Results
- Best model achieved validation accuracy: 0.5455
- Test accuracy depends on dataset size but typically 40-55%
- Limited by small dataset and high variation in unofficial images
- Recommended improvements:
- More data
- Background cleanup
- Stronger CNNs or pretrained models
- Data augmentation
---

## Authors
Group 26 - Jodi Barnes & Lauren Moffett

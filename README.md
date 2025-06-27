
# Solar Radio Burst Classification

Classification of solar radio bursts from spectrogram images using transfer learning models.

## Overview

This project classifies solar radio burst spectrograms into three categories:
- **Type II**: Slow-drifting bursts associated with CMEs
- **Type III**: Fast-drifting bursts from electron beams  
- **Empty**: Background spectrograms without bursts


## Setup

```bash
# Clone repository
git clone https://github.com/Hermanlrx/SRBClassificationCodeAndData.git
cd SRBClassificationCodeAndData

# Create conda environment
conda create -n solar-bursts python=3.9
conda activate solar-bursts

# Install dependencies
conda install tensorflow keras opencv matplotlib pandas numpy scikit-learn jupyter
pip install ultralytics  # For YOLO
```

## Usage

Navigate to any model folder and run the corresponding Jupyter notebook:

```bash
jupyter notebook "Code and results of each model/1.Comparison Transferlearning Densenet201/1. Model+code/TransferLearningTest.ipynb"
```



## Project Structure



Each model folder contains:
- `1. Model+code/`: Jupyter notebooks with implementation
- `2. Images/`: Training plots and visualizations
- `3. Results/`: CSV files and result analysis notebooks
- `confusion_matrix*.png`: Model performance visualization

  
```SRBClassificationCodeAndData/
├── .gitignore
├── Code and results of each model/
│   ├── 1.Comparison Transferlearning Densenet201/
│   │   ├── 1. Model+code/
│   │   │   └── TransferLearningTest.ipynb
│   │   ├── 2. Images/
│   │   │   ├── DenseNetAcc.png
│   │   │   └── DenseNetLoss.png
│   │   ├── 3. Results/
│   │   │   ├── densenet.csv
│   │   │   └── Results.ipynb
│   │   └── confusion_matrixDensenet.png
│   ├── 2.Comparison Transferlearning LOCAL YOLOV8/
│   │   ├── 1. Model+code/
│   │   │   └── PYTORCH.ipynb
│   │   ├── 2. Images (Pytorch run)/
│   │   │   └── run/
│   │   │       ├── args.yaml
│   │   │       ├── confusion_matrix_normalized.png
│   │   │       ├── confusion_matrix.png
│   │   │       ├── results.csv
│   │   │       ├── results.png
│   │   │       ├── train_batch0.jpg
│   │   │       ├── train_batch1.jpg
│   │   │       ├── train_batch2.jpg
│   │   │       ├── val_batch0_labels.jpg
│   │   │       ├── val_batch0_pred.jpg
│   │   │       ├── val_batch1_labels.jpg
│   │   │       ├── val_batch1_pred.jpg
│   │   │       ├── val_batch2_labels.jpg
│   │   │       └── val_batch2_pred.jpg
│   │   ├── 3. Results/
│   │   │   ├── results.csv
│   │   │   └── results.ipynb
│   │   └── confusion_matrixYOLO.png
│   ├── 3.Comparison Transferlearning MobileNet/
│   │   ├── 1. Model+code/
│   │   │   └── TransferLearningTest.ipynb
│   │   ├── 2. Images/
│   │   │   ├── 0.8218125700950623_loss.png
│   │   │   └── MobileNet.png
│   │   ├── 3. Results/
│   │   │   ├── mobilenet.csv
│   │   │   └── Results.ipynb
│   │   └── confusion_matrix_MobileNet.png
│   ├── 4.Comparison Transferlearning RESnet152/
│   │   ├── 1. Model+code/
│   │   │   └── TransferLearningTest.ipynb
│   │   ├── 2. Images/
│   │   │   ├── 0.8003072142601013_loss.png
│   │   │   └── ResNet.png
│   │   ├── 3. Results/
│   │   │   ├── resnet152.csv
│   │   │   └── Results.ipynb
│   │   └── confusion_matrixResnet.png
│   └── 5.Comparison Transferlearning VGG19/
│       ├── 1. Model+code/
│       │   └── TransferLearningTest.ipynb
│       ├── 2. Images/
│       │   ├── 0.8064516186714172_loss.png
│       │   └── VGG.png
│       ├── 3. Results/
│       │   ├── Results.ipynb
│       │   ├── ResultsVgg19.xlsx
│       │   └── vgg19.csv
│       └── confusion_matrix_VGNETT.png
├── DATA/...
|
├── LICENSE
└── README.md
```



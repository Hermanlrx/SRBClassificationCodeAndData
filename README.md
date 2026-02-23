
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

## Raw data files
[Zenodo](https://doi.org/10.5281/zenodo.18712661)




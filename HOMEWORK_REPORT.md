# PyTorch Classification with DVC & MLflow - Homework Report

## Student Progress Summary

This report documents the steps taken to complete the PyTorch classification homework assignment and the roadblock encountered.

## Steps Completed Successfully

### 1. Repository Setup
- Forked the original repository: `https://github.com/besmaguesmi/classification-pytorch`
- Cloned the forked repository to local machine
- Set up Python virtual environment (`.venv`)

### 2. Dependencies Installation
- Installed required packages:
  ```bash
  pip install dvc dvc-gdrive
  pip install torch torchvision scikit-learn mlflow pillow numpy matplotlib seaborn pandas
  ```

### 3. DVC Configuration Attempts
- Encountered existing `.dvc` directory from original repository
- Attempted `dvc init` (failed due to existing DVC setup)
- Successfully configured DVC remotes:
  - Found existing Google Drive remote: `gdrive://0ABF-h_iJuV04Uk9PVA`
- Attempted data pull: `dvc pull` succefull 

![alt text](image-2.png)

### 4. MLflow Setup
- Installed MLflow
- Resolved Windows MIME type issues by tinkering with regedit
- Successfully started MLflow UI
4.1 MLflow runs: training the models was successfuk through mlflow as shows in this attachment: 
![alt text](<Screenshot (1498).png>)

also testing the runs was also successful: 
![alt text](image-3.png) 
![alt text](<Screenshot (1499).png>)
### 5. Code Analysis
- Examined project structure and dependencies
- Understood expected data structure:
  ```
  data/
  ├── train/
  │   ├── sea/     (image files)
  │   └── forest/  (image files)
  └── test/
      ├── sea/
      └── forest/
  ```

## Screenshots

### Screenshot 1: Mlflow UI
![alt text](image-1.png)
### Screenshot 2: Training Command Error
![alt text](image.png)

### Screenshot 3: DVC Status and Remote Configuration
![alt text](<Screenshot (1437).png>)

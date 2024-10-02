# YOLOv8 Car Detection
## Project Overview
This project focuses on training and testing a YOLOv8 model for detecting different car models in a custom dataset of Iranian cars. The dataset contains images of several car models, including:<br />
1. IranKhodro Dena<br />
2. Kia Cerato<br />
3. Mazda 3<br />
4. Peugeot 206<br />
5. Saipa Saina<br />

The goal is to accurately detect and classify these car models in real-world images using YOLOv8.<br /><br />

## Repository Structure
**datasets/:** Not included (dataset is private).<br />
**runs/:** Results from training and testing.<br />
**config/:** The data.yaml file and other configuration files.<br />
**notebooks/:** Google Colab notebook used to train and evaluate the model.<br />
**README.md:** This file.<br /><br />

## Dataset
The dataset contains images of five different car models, and their corresponding labels in YOLO format. The dataset is private and not included in this repository.
To run this project with your own dataset, ensure it follows the same structure:

 ```
datasets/
    ├── images/
    │   ├── train/
    │   ├── val/
    │   └── test/
    └── labels/
        ├── train/
        ├── val/
        └── test/
```

## How to Run the Project
**1. Open the Google Colab Notebook:** Click on the link to access the notebook: <a href="https://colab.research.google.com/drive/1udoXWKEvE4UcVRZ2HL426XK5ZEUNBetW#scrollTo=S1_tdMLhbs8z" target="_blank">click here</a>

**2. Make a Copy:** In Colab, go to File > Save a copy in Drive to create your own copy of the notebook. This allows you to edit and run the code.

**3. Set Up Your Environment:** Ensure you have the required libraries installed by running the installation command in the first cell:
```
!pip install ultralytics
```

**4. Mount Google Drive:**
```
from google.colab import drive
drive.mount('/content/drive')
```

**5. Load Your Dataset:**
Make sure your dataset is organized and accessible in your Google Drive. Update the paths in the code as necessary.

**6. Train the Model:**
Run the training cell to train the YOLOv8 model using your dataset. Modify the parameters in the model.train() function as needed. You can also see your training logs after running this code cell.


**7. Test the Model:**
Execute the testing code to evaluate the model's performance on the test set and view results such as the confusion matrix.

**8. View Results:**
Check the runs directory in your Google Drive for results, including confusion matrix, normalized confusion matrix, F1_curve, P curve, PR_curve, and R_curve. <br /><br />

## Contact
If you have any questions, suggestions, or issues, feel free to reach out:<br />
Email: a.sadeghzadeh02@gmail.com



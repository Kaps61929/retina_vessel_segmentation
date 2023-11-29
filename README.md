# Retina_vessel_segmentation

## Overview

Retinal vessel analysis plays a pivotal role in both personal identification and early disease detection. 
This repository showcases a lightweight attention-based U-Net model that significantly enhances retinal image segmentation, enabling the identification of crucial markers for diseases like diabetes and hypertension using Pytorch.
## Model Architecture
The proposed U-Net leverages dual attention modules to improve retinal image segmentation. The use of lightweight components enhances model capability without compromising performance.


![image](https://github.com/Kaps61929/retina_vessel_segmentation/assets/115138974/f26de308-22fb-408c-b6c7-2d4f911e16f5)


![image](https://github.com/Kaps61929/retina_vessel_segmentation/assets/115138974/46fb96cb-4c15-47f0-8760-e1d6fa94a764)



# Results
![image](https://github.com/Kaps61929/retina_vessel_segmentation/assets/115138974/c6ff6456-1147-4329-8ac1-be002f9bdebd)

![image](https://github.com/Kaps61929/retina_vessel_segmentation/assets/115138974/dd1907f2-0ea7-4c26-b2d8-6823e60a2357)


  
## Training Methodology
Dataset: https://www.kaggle.com/datasets/abdallahwagih/retina-blood-vessel

Data Split: 80% of the images were used for training, while 20% were allocated for testing.

Optimization: Adam optimizer with BCE+DiceLoss was employed, resulting in remarkable metrics.

model :unet along with attention module
## Model Performance
The model demonstrated robust performance in retinal segmentation tasks, exhibiting the following metrics:

Jaccard Index: 0.6297
F1 Score: 0.7718
Recall: 0.7356
Precision: 0.8228
Accuracy: 96.25%
![image](https://github.com/Kaps61929/retina_vessel_segmentation/assets/115138974/0973cbd4-6a78-4314-bf6b-fc49003de376)

## Resources
Kaggle - [Retina Blood Vessel Dataset](https://www.kaggle.com/datasets/abdallahwagih/retina-blood-vessel)
Research paper-https://ieeexplore.ieee.org/document/9091247

## File Architecture
This repository contains the following files and directories:

### Notebooks
-data.ipynb: Extracts data from the 'Data1' folder.
-loss.ipynb: Implements the loss function using BCE+DiceLoss.
-model.ipynb: Contains the implementation of the U-Net model along with attention modules.
-train.ipynb: Includes the code for the training phase of the model.
-test.ipynb: Comprises the code for the testing phase of the model.
### Directories
results: Contains saved results obtained after testing.
Data1: Directory housing the dataset, which includes images and their corresponding segmentation masks.



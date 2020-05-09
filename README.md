# Lung Nodule Identification
Erica Chio (ebc308) and Nithu Mathew (njm363)


##  Contributions
Both of us worked closely to have input on data preparation, augmentation, building the models, tuning, and evaluating.

**Erica Chio (ebc308)** 
  * XML Preprocessing: reading each patient's xml file (xml_preprocessing.ipynb)
  * Faster R-CNN
    * Preprocessing data 
    * Implementing Model
    * Evaluating Model
  * Modifying Source Code to be compatible (source_code folder)
  * mobilenet_v2 Faster R-CNN Model (not included in final write up) 

**Nithu Mathew (njm363)**
  * CSV Files: creating one file to include every patient's data (csv_preprocessing.ipynb)
  * Mask R-CNN
    * Preprocessing data
    * Implementing Model
    * Evaluating Model
  * Creating Evaluation Figures (model_comparison.ipynb)
  * VGG16 Faster R-CNN Model (not included in final write up) 
  
--- 
  
## Content

### lung_nodule_identification_ebc308_njm363.pdf
Final Report Write Up

### Code Folder

| Notebook Name | Backbone      | Model         | Dataset       | Area         |
| ------------- | ------------- | ------------- | ------------- |------------- |
| fasterrcnn_resnet50_area>50.ipynb | Resnet 50 | Faster R-CNN | COCO | area >= 50 |
| fasterrcnn_resnet50.ipynb | Resnet 5  | Faster R-CNN  | COCO | area >= 100  |
| fasterrcnn_imagenet.ipynb | Resnet 50 | Faster R-CNN  | imageNET | area >= 100  |
| final_maskrcnn_resnet50_50area.ipynb | Resnet 50  | Mask R-CNN | COCO | area >= 50 |
| final_maskrcnn_resnet50_100area.ipynb | Resnet 50  | Mask R-CNN | COCO | area >= 100  |
| final_maskrcnn_resnet50_imagenet_100area.ipynb | Resnet 50 | Mask R-CNN | imageNET  | area >= 100 |

### large_nodules.csv
Complete CSV file of every nodule with an area >= 3mm.

CSV files to separate train / validate / test:
* large_nodules_train.csv 
* large_nodules_validate.csv 
* large_nodules_test.csv 

### all_nodules.csv 
Complete CSV file of every nodule (< 3mm and >= 3mm)

#### source_code 
* modified torch.vision Faster R-CNN/Mask R-CNN files to be compatible to image size, include train accuracy / validation loss

#### deprecated_notebooks
* old notebooks to document progress of our work

#### pickle
* saving each model's:
  * train loss
  * validation loss
  * train accuracy
  * validation accuracy
  
 ### Figures
 
 * Validation Accuracy Curve Plots for each model 
 * Correct / Incorrect Prediction Images for Faster R-CNN (COCO, area > 50) 
 * Correct / Incorrect Prediction Images for Mask R-CNN model (COCO, area > 100)
---


# Lung Nodule Identification
Erica Chio (ebc308) and Nithu Mathew (njm363)


##  Contributions
Both of us worked closely to have input on data preparation, augmentation, building the models, tuning, and evaluating.

**Erica Chio (ebc308)** 
  * XML Preprocessing: reading each patient's xml file (xml_preprocessing.ipynb)
  * FasterRCNN
    * Preprocessing data 
    * Implementing Model
    * Evaluating Model
  * Modifying Source Code to be compatible (source_code folder)
  * mobilenet_v2 FasterRCNN Model (not included in final write up) 

**Nithu Mathew (njm363)**
  * CSV Files: creating one file to include every patient's data (csv_preprocessing.ipynb)
  * MaskRCNN
    * Preprocessing data
    * Implementing Model
    * Evaluating Model
  * Creating Evaluation Figures (model_comparison.ipynb)
  * VGG16 FasterRCNN Model (not included in final write up) 
  
--- 
  
## Content

### Code Folder

| Notebook Name | Backbone      | Model         | Dataset       | Area         |
| ------------- | ------------- | ------------- | ------------- |------------- |
| fasterrcnn_resnet50_area>50.ipynb | Resnet 50 | Faster RCNN | COCO | area >= 50 |
| fasterrcnn_resnet50.ipynb | Resnet 5  | Faster RCNN  | COCO | area >= 100  |
| fasterrcnn_imagenet.ipynb | Resnet 50 | Faster RCNN  | imageNET | area >= 100  |
| final_maskrcnn_resnet50_50area.ipynb | Resnet 50  | MaskRCNN | COCO | area >= 50 |
| final_maskrcnn_resnet50_100area.ipynb | Resnet 50  | MaskRCNN | COCO | area >= 100  |
| final_maskrcnn_resnet50_imagenet_100area.ipynb | Resnet 50 | MaskRCNN | imageNET  | area >= 100 |

### large_nodules.csv
Complete CSV file of every nodule with an area >= 3mm.
large_nodules_train.csv / large_nodules_validate.csv / large_nodules_test.csv : CSV files to separate train / validate / test

### all_nodules.csv 
Complete CSV file of every nodule (< 3mm and >= 3mm)

#### source_code 
* modified torch.vision FasterRNN/MaskRCNN files to be compatible to image size, include train accuracy / validation loss

#### deprecated_notebooks
* old notebooks to document progress of our work

#### pickle
* saving each model's:
  * train loss
  * validation loss
  * train accuracy
  * validation accuracy
  
 ### Figures
 
---


# Lung Nodule Identification
Erica Chio (ebc308) and Nithu Mathew (njm363)

## Folders

### source_code 
* modified torch.vision FasterRNN/MaskRCNN files to be compatible to image size, include train accuracy / validation loss

### deprecated_notebooks
* old notebooks to document progress of our work

### pickle
* saving each model's:
  * train loss
  * validation loss
  * train accuracy
  * validation accuracy
  
---

##  Contributions
Both of us worked closely to have input on data preparation, augmentation, building the models, tuning, and evaluating.

**Erica Chio (ebc308)** 
  * XML Preprocessing: reading each patient's xml file
  * FasterRCNN
    * Preprocessing data 
    * Implementing Model
    * Evaluating Model
  * Modifying Source Code to be compatible
  * mobilenet_v2 FasterRCNN Model (not included in final write up) 

**Nithu Mathew (njm363)**
  * CSV Files: creating one file to include every patient's data
  * MaskRCNN
    * Preprocessing data
    * Implementing Model
    * Evaluating Model
  * Creating Evaluation Figures 
  * VGG16 FasterRCNN Model (not included in final write up) 

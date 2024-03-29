---
description: >-
  Before creating an annotation project, you should upload your dataset in the
  “Dataset” tab.
---

# 2.1 Dataset Format

DeepQ AI Platform support three types of annotation: image classification, object detection & object segmentation

![](../.gitbook/assets/con-2-1-1.png)

## Dataset Format

The accepted dataset format is described below, please check your dataset and image format before uploading.

### Dataset format: zip file

* **Image only:** Only a folder of images should be presented here. Please note that the folder name must be “**image**,” entirely in lowercase letters.
* **With annotation:** A folder named “**image**” \_\_in lowercase and a file specifying the label of each image, “**label.csv**” should be presented here. You can either zip “image” and “label.csv” or put them into another folder and zip that folder.
* **For annotation file (label.csv) format, please refer to** [**Annotation Data Formats**](annotation-data-formats.md) _\*\*_

![](../.gitbook/assets/con-2-1-2.png)

### Import multi-class data from separate folders

Images can also be stored in different folders under "Classes" then upload the compressed zip file. By doing so, the DeepQ AI Platform will automatically label the images according to the folder name, e.g. "Class A", and no additional annotation effort will be needed.&#x20;

![](../.gitbook/assets/con-2-1-3.png)

### Zip-tool Notice:

For Windows users, please compress your file by "Bandizip" tool and process as the following steps if the name of your images are non-English format.

1. Compression Setting: Select "Store Unicode file names in an extra header field if Zip files (UTF-8)".
2. Compress "xxx.zip".
3. **Naming the zip file:** The name of the dataset will be the same as that of the zip file you uploaded, which cannot be edited in the “Dataset” tab. You can rename the zip file before you upload it.

![](../.gitbook/assets/con-2-1-4.png)

![](../.gitbook/assets/con-2-1-5.PNG)

# Data Formats

DeepQ AI Platform supports differnt types of labeld data such as classification, detection & segmentation. If a user has labels created by other annotation tools, just convert them into the formats described below then upload to the DeepQ AI platform. Once the dataset is accepted by the platform, you can train your models right away.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-2-2-1.png)

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td></td><td>Dataset format explained</td><td></td></tr><tr><td></td><td>Label format explained<br>/</td><td></td></tr></tbody></table>

***

### Dataset Format <a href="#dataset-format" id="dataset-format"></a>

The accepted dataset format is described below, please check your dataset and image format before uploading.

### Dataset format: zip file <a href="#dataset-format-zip-file" id="dataset-format-zip-file"></a>

* **Image only:** Only a folder of images should be presented here. Please note that the folder name must be “**image**,” entirely in lowercase letters.
* **With annotation:** A folder named “**image**” \_\_in lowercase and a file specifying the label of each image, “**label.csv**” should be presented here. You can either zip “image” and “label.csv” or put them into another folder and zip that folder.
* **For annotation file (label.csv) format, please refer to** [**Annotation Data Formats**](https://console.deepq.ai/docs/console/dataset/annotation-data-formats.html) _\*\*_

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-2-1-2.png)

### Import multi-class data from separate folders <a href="#import-multi-class-data-from-separate-folders" id="import-multi-class-data-from-separate-folders"></a>

Images can also be stored in different folders under "Classes" then upload the compressed zip file. By doing so, the DeepQ AI Platform will automatically label the images according to the folder name, e.g. "Class A", and no additional annotation effort will be needed.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-2-1-3.png)

### Image Classification: <a href="#image-classification" id="image-classification"></a>

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-2-2-2.png)

* Each line specifies the name of an image file and its category label that are separated by a comma.
* The same image should be repeated N times, where N is the number of classes assigned.
* The pairs of an image name and a category label start from the first line. That is, there is no CSV header in the label file.
* Pure number (e.g. 001) as class names must be double quoted. (e.g. "001").
* <mark style="color:red;">**The minimum annotation requirement for each class is 3 images. If the dataset contains class(es) with less than 3 images, the dataset will be rejected**</mark>

### Object Detection: <a href="#object-detection" id="object-detection"></a>

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-2-2-3.png)

* Each line specifies a bounding box of an object.
* Each line must include 6 fields, separated by a comma: image name, object name, xLeft, yTop, width, height. _\*\*_
* (xLeft, yTop) is the top-left vertex of the bounding box, and width and height indicate the width and height of the bounding box.
* (x, y, w, h) can be either integer or floating-point numbers.
* If an image contain more than 1 bounding boxes, it can be shown in multiple lines.
* The bounding box lines must start from the first line. That is, there is no CSV header in the label file.
* Pure number (e.g. 001) as class names must be double quoted. (e.g. "001").
* <mark style="color:red;">**The minimum annotation requirement for each class is 3 images. If the dataset contains class(es) with less than 3 images, the dataset will be rejected**</mark>

### Object Segmentation: <a href="#object-segmentation" id="object-segmentation"></a>

DeepQ AI platform uses a proprietary format for object segmentation that offers better flexibility in label modification and storage efficiency. If you want to export your segmentation label as a specific format, please contact DeepQ for assistance.

# 3.1.1.1 Annotation Quality Control

Label quality is an important factor in Deep Learning. In order to ensure the best labeling quality in each annotation project, users can choose from three validation workflows to run your project.

**DeepCap Smart Validation** provides a consistent rate based on DeepQ original algorithm for an iterative annotation process. The system suggests annotations and provides accurate ground truths for model training.

***

![validation workflow by DeepCap Smart Validation (DSV)](../../../.gitbook/assets/con-3-1-5-2.3.jpg)

![validation workflow performed only by reviewers](../../../.gitbook/assets/con-3-1-6-2.3.jpg)

![a hybrid method that combines DSV & reviewe mechanism](../../../.gitbook/assets/con-3-1-7-2.3.jpg)

***

## Enable DeepCap Smart Validation (DSV)

Cases from the dataset are automatically distributed to the annotators. To deliver qualified data for training, the DeepCap Smart Validation (DSV) function can be enabled if the annotator number is greater than or equal to two in the project.

For example, if the project contains three annotators, two or three annotators can be selected to work on each study. The maximum number of annotators that can be assigned to work on each case is five. The DSV function provides a consistent rate based on the DeepQ original algorithm for an iterative annotation process, and it will suggest accurate ground truths for model training.

### **Notice:**

* The number of annotators to work on each case cannot be edited once the project is published.
* The DSV result is applied as the default value to export for training.
* You can return each case to the annotator or exclude it from artificial intelligence (AI) training if the DSV result is not acceptable to your requirements.

![](../../../.gitbook/assets/con-3-1-12.png)

## View DSV result from Annotation Details

As a project owner, you can view the suggested DSV result for each image and can also check annotation results from each annotator.

#### Image Classification:

* **DSV result:** The suggested label and the consistency rate are shown in this section. The DSV calculation for image classification is simple as the DSV result is determined by estimating the majority consensus. For example, if there were three annotators work on each image, two of them select the same label for one image, the consistency rate would be 67%. If The DSV result presented as “failed” means the consistency rate is equal or less than 50%. In this case, you can return (![](../../../.gitbook/assets/con-icon-21.png)) this study to the annotator or exclude (![](../../../.gitbook/assets/con-icon-9.png)) this case from AI training.

![](../../../.gitbook/assets/con-3-1-13.jpg)

#### Object Detection:

* **The DSV result for object detection is based on the following calculation steps:**
* Calculate IoU for each bounding box from different annotator.
* Grouping the bounding boxes.
* Calculate the average of the bounding box groups.

**\[Disable annotator result]**

* **DSV result:** The suggested bounding box and consistency rate **will** be presented in this area, you can hide the DSV bounding box \_\*\*\_label by clicking “![](../../../.gitbook/assets/con-icon-23.png)”.

![](../../../.gitbook/assets/con-3-1-14.jpg)

**\[Enable annotator result]**

* **Annotator result:** You can enable “annotator result” to view all bounding boxes annotated by each annotator on the image. The remaining bounding boxes will be presented on the image.

![](../../../.gitbook/assets/con-3-1-15.jpg)

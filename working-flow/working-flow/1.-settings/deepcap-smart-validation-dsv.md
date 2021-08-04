# Annotation Quality Control

**DeepCap Smart Validation** provides a consistent rate based on DeepQ original algorithm for an iterative annotation process. The system suggests annotations and provides accurate ground truths for model training.

## Enable DeepCap Smart Validation \(DSV\)

Cases from the dataset are automatically distributed to the annotators. To deliver qualified data for training, the DeepCap Smart Validation \(DSV\) function can be enabled if the annotator number is greater than or equal to two in the project.

For example, if the project contains three annotators, two or three annotators can be selected to work on each study. The maximum number of annotators that can be assigned to work on each case is five. The DSV function provides a consistent rate based on the DeepQ original algorithm for an iterative annotation process, and it will suggest accurate ground truths for model training.

### **Notice:**

* The number of annotators to work on each case cannot be edited once the project is published. 
* The DSV result is applied as the default value to export for training. 
* You can return each case to the annotator or exclude it from artificial intelligence \(AI\) training if the DSV result is not acceptable to your requirements.

![](../../../.gitbook/assets/3-1-1-1-000001.png)

## View DSV result from Annotation Details

As a project owner, you can view the suggested DSV result for each image and can also check annotation results from each annotator.

#### Image Classification:

* **DSV result:** The suggested label and the consistency rate are shown in this section. The DSV calculation for image classification is simple as the DSV result is determined by estimating the majority consensus. For example, if there were three annotators work on each image, two of them select the same label for one image, the consistency rate would be 67%.   If The DSV result presented as “failed” means the consistency rate is equal or less than 50%. In this case, you can return \(![](../../../.gitbook/assets/picture24.png)\) this study to the annotator or exclude \(![](../../../.gitbook/assets/image%20%2814%29.png)\) this case from AI training. 

![](../../../.gitbook/assets/3-1-1-1-000002.png)

#### Object Detection:

* **The DSV result for object detection is based on the following calculation steps:**
* Calculate IoU for each bounding box from different annotator.
* Grouping the bounding boxes. 
* Calculate the average of the bounding box groups.

**\[Disable annotator result\]**

* **DSV result:** The suggested bounding box and consistency rate **will** be presented in this area, you can hide the DSV bounding box _\*\*_label by clicking “![](../../../.gitbook/assets/picture26.png)”. 

![](../../../.gitbook/assets/3-1-1-1-000003.png)

**\[Enable annotator result\]**

* **Annotator result:** You can enable “annotator result” to view all bounding boxes annotated by each annotator on the image. The remaining bounding boxes will be presented on the image.

![](../../../.gitbook/assets/3-1-1-1-000004.png)


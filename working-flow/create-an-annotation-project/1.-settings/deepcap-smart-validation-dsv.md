# Annotation Quality Control \(Edzer\)

DeepCap Smart Validation provides a consistent rate based on DeepQ original algorithm for an iterative annotation process. The system suggests annotations and provides accurate ground truths for model training.

## Enable DeepCap Smart Validation \(DSV\) \(兩段可以合併\)

Cases from the dataset are automatically distributed to the annotators. To prepare qualified data for training, the DeepCap Smart Validation \(DSV\) function can be enabled if the number of annotators in this project is greater than or equal to two. ~~For example, two or three annotators can be selected to work on each case if the project has three annotators.~~  
_****_\(elly\)  
_****_For example, if the project contains three annotators, two or three annotators can be selected to work on each study.   
_****_ The DSV function provides a consistent rate based on the DeepQ original algorithm for an iterative annotation process. _DeepCap \(DSV???\) suggests accurate ground truths for model training._ **\(功能方面看不懂\)**  
 **Please note that the number of annotators to work on each case cannot be edited once the project is published.** 

![](../../../.gitbook/assets/picture6.png)

## 

## ~~Enable DSV During the Project Creation Process~~

~~You can enable DeepCap Smart Validation \(DSV\) function if the number of annotators in this project is greater than or equal to two. For example, you can select two or three annotators to work on each case if the project has three annotators.~~ \(重複\) The maximum number of annotators that can be assigned to work on each ~~case~~  \(study?\) ~~you can set~~ is five.

Notice: 

1. ~~The number of annotators to work on each case cannot be edited once the project is published.~~  \(重複\)
2. The DSV result is applied as the default value to export for training. 
3. You can return each ~~case~~ \(study?\) to the annotator or exclude it from artificial intelligence \(AI\) training if the DSV result is not acceptable to your requirements.

![](../../../.gitbook/assets/picture23.png)

## View DSV result from Annotation Details

As a project owner, you can view the DSV result ~~that the system suggests \(~~suggested\) ~~~~ for each image and can check ~~each~~ annotation results from each annotator.

#### Image Classification:

* **DSV result \(A\):** ~~The suggested label for the entire image and consistency rate can be presented in this area.~~ **\(The suggested label and the consistency rate are shown in this section.\)** _The DSV calculation for image classification is simple as the DSV result is determined by estimating the majority consensus. \(語意不清\)_  ~~__For example, suppose that three annotators work on each image. The consistency rate is 67% if two annotators select the same label for an image.~~ \(**For example, if there were three annotators work on each image, two of them select the same label for one image, the consistency rate would be 67%.\)** The DSV result is presented as “failed” if the consistency rate is less than or equal to 50%. In this case, you can return \(![](../../../.gitbook/assets/picture24.png)\) this case to the annotator or exclude \(![](../../../.gitbook/assets/image%20%2814%29.png)\) this case from AI training.   
* **Annotator result \(B\):** You can view the result labeled by each annotator in this section.

~~The DSV result is presented as “failed” if the consistency rate for the entire image is less than or equal to 50%. If a case has failed, you can return \(~~![](../../../.gitbook/assets/picture24.png)~~\) this case to the annotator or exclude \(~~![](../../../.gitbook/assets/image%20%2814%29.png)~~\) this case from AI training.~~  **重複**

![](../../../.gitbook/assets/picture25.png)

#### Object Detection:

* **DSV result \(A\):** The suggested bounding box and consistency rate might be presented in this area. You can ~~disable~~ **\(hide\)** ~~~~the DSV bounding box **label** ~~to show on the image~~ by clicking “![](../../../.gitbook/assets/picture26.png)”. The DSV result for object detection is based on the following calculation steps.

1. Calculate IoU for each ~~two~~ bounding box from different annotator.
2. Grouping the bounding boxes. 
3. Calculate the average of the bounding box groups.

* **Annotator result \(B\):** You can enable “annotator result” to view all bounding boxes annotated by each annotator on the image. ~~You can disable any annotator’s annotation result by clicking on “~~![](../../../.gitbook/assets/picture26.png)~~”.~~ 重複 The remaining bounding boxes will be presented on the image.

**\[Disable annotator result\]**   

![](../../../.gitbook/assets/picture27.png)

**\[Enable annotator result\]**

![](../../../.gitbook/assets/picture28.png)

**\[Disable DSV and any annotator’s annotation\]**

![](../../../.gitbook/assets/picture29.png)


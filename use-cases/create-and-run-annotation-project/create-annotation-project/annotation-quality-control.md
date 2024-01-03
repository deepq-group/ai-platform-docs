# Annotation Quality Control

Annotation quality is an important factor in Deep Learning. In order to ensure the best labeling quality in each annotation project, users can choose from three validation workflows to run your project.

**DeepCap Smart Validation** provides a consistent rate based on DeepQ original algorithm for an iterative annotation process. The system suggests annotations and provides accurate ground truths for model training.

***

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-5-2.3.jpg" alt="validation workflow by DeepCap Smart Validation (DSV)"><figcaption><p>validation workflow by DeepCap Smart Validation (DSV)</p></figcaption></figure>

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-6-2.3.jpg" alt="validation workflow performed only by reviewers"><figcaption><p>validation workflow performed only by reviewers</p></figcaption></figure>

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-7-2.3.jpg" alt="a hybrid method that combines DSV &#x26; reviewe mechanism"><figcaption><p>a hybrid method that combines DSV &#x26; reviewe mechanism</p></figcaption></figure>

***

### Enable DeepCap Smart Validation (DSV) <a href="#enable-deepcap-smart-validation-dsv" id="enable-deepcap-smart-validation-dsv"></a>

Cases from the dataset are automatically distributed to the annotators. To deliver qualified data for training, the DeepCap Smart Validation (DSV) function can be enabled if the annotator number is greater than or equal to two in the project.

For example, if the project contains three annotators, two or three annotators can be selected to work on each study. The maximum number of annotators that can be assigned to work on each case is five. The DSV function provides a consistent rate based on the DeepQ original algorithm for an iterative annotation process, and it will suggest accurate ground truths for model training.

#### **Notice:** <a href="#notice" id="notice"></a>

* The number of annotators to work on each case cannot be edited once the project is published.
* The DSV result is applied as the default value to export for training.
* You can return each case to the annotator or exclude it from artificial intelligence (AI) training if the DSV result is not acceptable to your requirements.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-12.png)

### View DSV result from Annotation Details <a href="#view-dsv-result-from-annotation-details" id="view-dsv-result-from-annotation-details"></a>

As a project owner, you can view the suggested DSV result for each image and can also check annotation results from each annotator.

**Image Classification:**

* **DSV result:** The suggested label and the consistency rate are shown in this section. The DSV calculation for image classification is simple as the DSV result is determined by estimating the majority consensus. For example, if there were three annotators work on each image, two of them select the same label for one image, the consistency rate would be 67%. If The DSV result presented as “failed” means the consistency rate is equal or less than 50%. In this case, you can return (![](https://console.deepq.ai/docs/console/.gitbook/assets/con-icon-21.png)) this study to the annotator or exclude (![](https://console.deepq.ai/docs/console/.gitbook/assets/con-icon-9.png)) this case from AI training.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-13.jpg)

**Object Detection:**

* **The DSV result for object detection is based on the following calculation steps:**
* Calculate IoU for each bounding box from different annotator.
* Grouping the bounding boxes.
* Calculate the average of the bounding box groups.

**\[Disable annotator result]**

* **DSV result:** The suggested bounding box and consistency rate **will** be presented in this area, you can hide the DSV bounding box \_\*\*\_label by clicking “![](https://console.deepq.ai/docs/console/.gitbook/assets/con-icon-23.png)”.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-14.jpg)

**\[Enable annotator result]**

* **Annotator result:** You can enable “annotator result” to view all bounding boxes annotated by each annotator on the image. The remaining bounding boxes will be presented on the image.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-15.jpg)

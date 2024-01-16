---
description: Test the performance of your trained model with Inference Jobs
---

# View/Test Models

### Create Inference Job <a href="#deploy-model--inference" id="deploy-model--inference"></a>

In the model detail view, you can create "Inference Jobs" to test the model

<figure><img src="../../../.gitbook/assets/AI_Training_Model_Detail_4.png" alt=""><figcaption></figcaption></figure>

* You have to deploy the model before creating any inference task.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-1.png)

* There are two modes of model inference: **batch & real-time.**

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-0.png)

### Real-time inference <a href="#real-time-inference" id="real-time-inference"></a>

Select and open one JPG/ PNG image from your local device, the inference result will be shown automatically with the AI image viewer.

The AI viewer contains the following information of each image:

<table><thead><tr><th width="148">Type</th><th>Image classification</th><th>Object detection</th><th>Object Segmentation</th></tr></thead><tbody><tr><td>prediction results</td><td>label name &#x26; confidence score</td><td>label name &#x26; bounding boxes in dotted lines</td><td>label name &#x26; objects with white stripes</td></tr><tr><td>Explainability</td><td>heat map of each label (can be toggled on of by <img src="../../../.gitbook/assets/icon_eye.png" alt="">)</td><td>NA</td><td>NA</td></tr><tr><td>Ground truth (if available)</td><td>ground truth labels</td><td>Bounding boxes in bold lines</td><td>Objects painted in solid colors</td></tr></tbody></table>

{% tabs %}
{% tab title="Image Classification" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Viewer_SLC_1.png" alt=""><figcaption><p>Image Classification: prediction &#x26; ground truth</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Viewer_SLC_2.png" alt=""><figcaption><p>Image classification: heat map on</p></figcaption></figure>
{% endtab %}

{% tab title="Object Detection" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Viewer_DET_1.png" alt=""><figcaption><p>Object detection:  prediction &#x26; ground truth</p></figcaption></figure>
{% endtab %}

{% tab title="Object Segmentation" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Viewer_SEG_1.png" alt=""><figcaption><p>Object Segmentation: prediction &#x26; ground truth</p></figcaption></figure>
{% endtab %}
{% endtabs %}

### Batch inference <a href="#batch-inference" id="batch-inference"></a>

* **Batch inference:** Select one of the dataset that you have uploaded from the drop list, enter the inference name and complete the creation process.
  * Prediction only: For datasets without annotation data, inference result will only provide prediction results without an inference report.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-5.png)

### View Inference Detail <a href="#view-inference" id="view-inference"></a>

#### Annotation Data (with ground truth/label) <a href="#annotation-data-with-ground-truthlabel" id="annotation-data-with-ground-truthlabel"></a>

* The inference detail, including training task, dataset, and annotation data will be shown here.
* Inference List: You can view the inference detail about the dataset, accuracy, and status.
* Inference Dataset shows all the cases that have been trained in this task.

#### Inference Detail for different types:

<table><thead><tr><th width="152">Type</th><th>Image Classification</th><th>Object Detection</th><th>Object Segmentation</th></tr></thead><tbody><tr><td>Performance metrics</td><td>>Accuracy<br>>ROC/PR Curve<br>>Confusion Matrix<br>>Evaluation Summary</td><td>>mAP<br>>FROC/PR Curve<br>>Evaluation Summary</td><td>>DICE scores<br>>Evaluation Summary</td></tr><tr><td>Dataset Statistics</td><td>>Label Distribution</td><td>>Box Label<br>>Box-per-Image<br>>Box Ratio<br>>Box Area<br>>Label Distribution (Image-wise)</td><td>>Label Distribution<br>>Mask-Coverage Distribution</td></tr></tbody></table>



{% tabs %}
{% tab title="Image Classification" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Detail_SLC_2.png" alt=""><figcaption><p>Inference Detail: Image Classification</p></figcaption></figure>
{% endtab %}

{% tab title="Object Detection" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Detail_DET_1.png" alt=""><figcaption><p>Inference Detail: Object Detection</p></figcaption></figure>
{% endtab %}

{% tab title="Object Segmentation" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Detail_SEG_1.png" alt=""><figcaption><p>Inference Detail: Object Segmentation</p></figcaption></figure>
{% endtab %}
{% endtabs %}



#### Prediction only <a href="#prediction-only" id="prediction-only"></a>

* if the batch inference dataset does not contain ground truth (annotation file not selected), there will be no performance metrics & Dataset statistics
* Each image of the selected dataset will be shown in the last column, you can check the result by clicking on the image.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-8.png)

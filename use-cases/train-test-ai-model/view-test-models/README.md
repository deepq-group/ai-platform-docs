# View/Test Models

### Create Inference Job <a href="#deploy-model--inference" id="deploy-model--inference"></a>

<figure><img src="../../../.gitbook/assets/AI_Training_Model_Detail_4.png" alt=""><figcaption></figcaption></figure>

* You have to deploy the model before creating any inference task.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-1.png)

* There are two modes of model inference: batch & real-time.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-0.png)

### Real-time inference <a href="#real-time-inference" id="real-time-inference"></a>

* **Real-time inference:** Select and open one JPG/ PNG image from your local device, the inference result will be shown automatically .
* ![](../../../.gitbook/assets/icon\_eye.png)

#### AI Image Viewer



{% tabs %}
{% tab title="Image Classification" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Viewer_SLC_1.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Viewer_SLC_2.png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Object Detection" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Viewer_DET_1.png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Object Segmentation" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Viewer_SEG_1.png" alt=""><figcaption></figcaption></figure>
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

{% tabs %}
{% tab title="Image Classification" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Detail_SLC_2.png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Object Detection" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Detail_DET_1.png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Object Segmentation" %}
<figure><img src="../../../.gitbook/assets/AI_Training_Inference_Detail_SEG_1.png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}



#### Prediction only <a href="#prediction-only" id="prediction-only"></a>

* Each image of the selected dataset will be shown in the last column, you can check the result by clicking on the image.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-8.png)

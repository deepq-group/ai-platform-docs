# View/Test Models

### Create Inference Job <a href="#deploy-model--inference" id="deploy-model--inference"></a>

<figure><img src="../../../.gitbook/assets/AI_Training_Model_Detail_4.png" alt=""><figcaption></figcaption></figure>

* You have to deploy the model before creating any inference task.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-1.png)

* There are two modes of model inference: batch & real-time.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-0.png)

#### Real-time inference <a href="#real-time-inference" id="real-time-inference"></a>

* **Real-time inference:** Select and open one JPG/ PNG image from your local device, the inference result will be shown automatically .

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-4.png)

#### Batch inference <a href="#batch-inference" id="batch-inference"></a>

* **Batch inference:** Select one of the dataset that you have uploaded from the drop list, enter the inference name and complete the creation process.
  * Prediction only: For datasets without annotation data, inference result will only provide prediction results without an inference report.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-5.png)

### View Inference <a href="#view-inference" id="view-inference"></a>

#### Annotation Data (with ground truth/label) <a href="#annotation-data-with-ground-truthlabel" id="annotation-data-with-ground-truthlabel"></a>

* The inference detail, including training task, dataset, and annotation data will be shown here.
* Inference List: You can view the inference detail about the dataset, accuracy, and status.
* Inference Dataset shows all the cases that have been trained in this task.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-6.png)



<mark style="background-color:red;">batch inference job detail missing</mark>





<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-7-2.png" alt=""><figcaption></figcaption></figure>

#### Prediction only <a href="#prediction-only" id="prediction-only"></a>

* Each image of the selected dataset will be shown in the last column, you can check the result by clicking on the image.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-8.png)

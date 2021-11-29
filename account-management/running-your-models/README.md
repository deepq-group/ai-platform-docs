# Running Your Models

## Deploy Model & Inference

* You have to deploy the model before creating any inference task.

![](../../.gitbook/assets/deploy.png)

* There are two modes of model inference: batch & real-time.

![](../../.gitbook/assets/batch-and-realtime.png)

### Real-time inference

* **Real-time inference:** Select and open one JPG/ PNG image from your local device, the inference result will be shown automatically .&#x20;

![](../../.gitbook/assets/inference-test.png)

### Batch inference

* **Batch inference:** Select one of the dataset that you have uploaded from the drop list, enter the inference name and complete the creation process.&#x20;
  * Prediction only: For datasets without annotation data, inference result will only provide prediction results without an inference report.

![](../../.gitbook/assets/batch-inference-.png)

## View Inference

### Annotation Data (with ground truth/label)

* The inference detail, including  training task, dataset, and annotation data will be shown here.&#x20;

![](<../../.gitbook/assets/inference-setting- (1).png>)

* The performance of each inference job is presented by the metrics of each type of application. for more information, please see [Deep Learning metrics explained](../deep-learning-metrics-explained/).&#x20;

![](<../../.gitbook/assets/inference-report (1) (1) (1).png>)

### Prediction only

* Each image of the selected dataset will be shown in the last column, you can check the result by clicking on the image.&#x20;

![](../../.gitbook/assets/batch-inference-dataset.png)

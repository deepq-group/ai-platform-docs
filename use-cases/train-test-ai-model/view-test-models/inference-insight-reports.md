# Inference Insight Reports

The inference insight report is a guide that helps you evaluate your trained model on a given test dataset. The provided metrics and figures depend on the task being performed. We also provide some case studies that showcase the model’s raw predictions. By analyzing the mistakes the model makes, we can identify possible weaknesses of the model and adjust future training accordingly.

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-2-2-0.png" alt=""><figcaption></figcaption></figure>

_Note: It is not necessary for the test dataset to originate from the same data source as the training dataset. Ideally, the test dataset should be rigorous (e.g. contain both simple and hard samples) so that the model’s true performance can be tested._

The definitions of the deep learning metrics are given in [https://console.deepq.ai/docs/console/account-management/deep-learning-metrics-explained](https://console.deepq.ai/docs/console/account-management/deep-learning-metrics-explained "mention").

#### Model Performance <a href="#model-performance" id="model-performance"></a>

**Multi-Class Classification**

In multi-class classification, we provide the ROC curves (left), the Precision-Recall (PR, center) curves, and the Confusion Matrix (right).

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-8-2-1.png" alt=""><figcaption></figcaption></figure>

**Multi-Label Classification**

In multi-class classification, we provide the ROC curves and the Precision-Recall (PR) curves (see multi-class classification for example plots).

**Object Detection**

In object detection, we show the PR curves (below left) and the FROC curves (below right).

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-8-2-2.png" alt=""><figcaption></figcaption></figure>

**Semantic Segmentation**

In Semantic Segmentation, there are no relevant curves to display.

#### Model Performance - Overview <a href="#model-performance---overview" id="model-performance---overview"></a>

The model performance table provides quantifiable values that evaluate the model’s performance. Below we show several example performance tables:

\\

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-8-2-3.png" alt=""><figcaption></figcaption></figure>

Aside from object detection, we organize the model performance according to class. We also provide the average performance across classes on the last row. By comparing the per-class performance with the average performance, you can identify classes where the model might be under-performing. In each row, we provide different metrics. Users will need to focus on the metrics that matter most according to their need.

#### Data and Prediction Statistics <a href="#data-and-prediction-statistics" id="data-and-prediction-statistics"></a>

The Data and Prediction Statistics figures and tables section provides a comparison between the ground truth label distribution and the model’s predicted label distribution. This is useful when we want to identify whether the model has potentially overfit/underfit to a certain class during training. We show an examples below:

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-8-2-4.png" alt=""><figcaption><p>Possible Data and Prediction Statistic plots generated. There is noticeable discrepancy between the ground truth test set and the model’s prediction on the test set.</p></figcaption></figure>

Explanation: We can see that the test dataset is roughly evenly distributed. But the majority of our model’s predictions are focused on cats and dogs. It’s possible this is caused by our training dataset having a large number of cat and dog images. We can see that our model rarely predicts fish. It’s possible that the fish images in our test set look largely different from the training set fish images. Or it could be that there are not that many fish images in our training set.

<mark style="color:yellow;">Note: We cannot use this comparison to conclude that a model is well trained (even in the case where the predicted and ground truth label distributions are equivalent). This comparison can only be used to identify potential overfitting or underfitting.</mark>

The explanation for each of these plots are given in the Training Insight Report tutorial. We can perform the same comparison across for the different tasks in a similar manner as shown above.

#### Case Studies <a href="#case-studies" id="case-studies"></a>

The case studies section of our inference report samples some of the model’s predictions and sorts them as either True Positive, False Positive, or False Negative by each class.

The definition for True Positive, False Positive, and False Negative are different between each task. We use the following figure to explain:

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-8-2-5.png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-8-2-6.png" alt=""><figcaption></figcaption></figure>

We provide 18 samples of True Positive, False Positive, False Negative cases from each class. By analyzing each of these predictions and their ground truths, we can identify the issues (False Positive and False Negatives) and identify possible areas of improvement for our model.

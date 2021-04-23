# Object Detection

![Inference report: Object detection](../../.gitbook/assets/image%20%28101%29.png)

**Average Precision \(AP\):**

          In computer vision, mAP is a popular evaluation metric used for object detection \(i.e. localisation and classification\). Localization determines the location of an instance \(e.g. bounding box coordinates\) and classification tells you what it is \(e.g. a dog or cat\).

![Image classification and localization](../../.gitbook/assets/image%20%28191%29.png)

Many object detection algorithms use mAP to evaluate their models. mAP stands for Mean Average Precision, where **Precision** measures how accurate your predictions are. i.e. the percentage of your predictions are correct. It measures how many of the predictions that your model made were actually correct.

Unlike classification, object detection systems make predictions in terms of a bounding box and a class label.

![](../../.gitbook/assets/image%20%28182%29.png)

For each bounding box, we measure an overlap between the predicted bounding box and the ground truth bounding box. This is measured by IoU \(intersection over union\), illustrated below.

![Intersection over Union \(IoU\)](../../.gitbook/assets/image%20%28166%29.png)

![](../../.gitbook/assets/image%20%28186%29.png)

For example the object detection task shown above, we calculate Precision and Recall using IoU value for a given IoU threshold. For example, if IoU threshold is 0.5, and the IoU value for a prediction is 0.7, then we classify the prediction as True Positive \(TF\). On the other hand, if IoU is 0.3, we classify it as False Positive \(FP\).

That also means that for a prediction, we may get different binary TRUE or FALSE positives, by changing the IoU threshold.

![](../../.gitbook/assets/image%20%281%29.png)

Another important term to understand is Recall.

**Recall** measures how well you find all the positives. For example, we can find 80% of the possible positive cases in our top K predictions.

![recall](file:///C:/Users/edzer_wu/AppData/Local/Temp/msohtmlclip1/01/clip_image012.jpg)

TP = True Positives \(Predicted as positive as was correct\)

FN = False Negatives \(Failed to predict an object that was there\)

**The general definition for the Average Precision \(AP\) is finding the area under the precision-recall curve above.**

**mAP \(mean average precision\)** is the average of AP. In some contexts, AP is calculated for each class and averaged to get the mAP. But in others, they mean the same thing.

![](../../.gitbook/assets/image%20%28173%29.png)

So for the above Advanced driver-assistance systems \(ADAS\) image, let’s calculate the mAP using the actual formula:

Here we assume that the confidence score threshold is 0.7 \(the default value of DeepQ AI platform for object detection\) and the IoU threshold is also 0.5. So we calculate the AP at IoU threshold 0.5.

For simplicity, we will calculate an average for the 11-point interpolated AP. In the latest research, more advanced techniques have been introduced to calculate the AP.

True Positives \(TP\) = 1 \(prediction & ground truth IOU&gt;0.5\)

Fasle Positives \(FP\) = 0 \(predicted bounding box only\)

False Negatives \(FN\) = 1 \(ground truth bounding box only\)

![precision](file:///C:/Users/edzer_wu/AppData/Local/Temp/msohtmlclip1/01/clip_image016.jpg)

![recall](file:///C:/Users/edzer_wu/AppData/Local/Temp/msohtmlclip1/01/clip_image018.jpg)

We plot the 11 points interpolated Precision-Recall curve.

![11 point interpolation precision recall curve](file:///C:/Users/edzer_wu/AppData/Local/Temp/msohtmlclip1/01/clip_image020.jpg)

We now calculate AP by taking the area under the PR curve. This is done by segmenting the recalls evenly to 11 parts: {0,0.1,0.2,…,0.9,1}.

![average precision AP](file:///C:/Users/edzer_wu/AppData/Local/Temp/msohtmlclip1/01/clip_image022.jpg)

So **mAP@0.5 for the image is 0.545**

![](file:///C:/Users/edzer_wu/AppData/Local/Temp/msohtmlclip1/01/clip_image024.png)

Different APs in the inference report, calculated with different IOUs and object areas

·       **Average recall \(AR\)**

Average recall describes the area doubled under the Recall x IoU curve. The Recall x IoU curve plots recall results for each IoU threshold where IoU ∈ \[0.5,1.0\], with IoU thresholds on the x-axis and recall on the y-axis. Similarly to mAP, mAR is the average of AR over the number of classes within the dataset


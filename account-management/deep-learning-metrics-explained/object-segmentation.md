# Object Segmentation

#### Inference report: Object segmentation

![](<../../.gitbook/assets/image (161).png>)

In object segmentation, **F\_1, Precision, Recall, Specificity & Accuracy** calculation is based on threshold 0.5. (Please see object detection section for details)

### **Intersection-Over-Union (IoU, Jaccard Index)**

The Intersection-Over-Union (IoU), also known as the Jaccard Index, is one of the most commonly used metrics in semantic segmentation… and for good reason. The IoU is a very straightforward metric that’s extremely effective.

![IoU calculation visualized. Source: Wikipedia](<../../.gitbook/assets/image (187).png>)

The IoU is the area of overlap between the predicted segmentation and the ground truth divided by the area of union between the predicted segmentation and the ground truth. This metric ranges from 0–1 with 0 signifying no overlap and 1 signifying perfectly overlapping segmentation. For binary (two classes) or multi-class segmentation, the mean IoU of the image is calculated by taking the IoU of each class and averaging them.

### **Dice Coefficient (F1 Score)**

The Dice Coefficient is 2 \* the Area of Overlap divided by the total number of pixels in both images.

![Illustration of Dice Coefficient. 2xOverlap/Total number of pixels](<../../.gitbook/assets/image (160).png>)

The Dice coefficient is very similar to the IoU. They are positively correlated, meaning if one says model A is better than model B at segmenting an image, then the other will say the same. Like the IoU, they both range from 0 to 1, with 1 signifying the greatest similarity between predicted and truth.\


_References:_

1. __[https://towardsdatascience.com/understanding-confusion-matrix-a9ad42dcfd62](https://towardsdatascience.com/understanding-confusion-matrix-a9ad42dcfd62)
2. [https://towardsdatascience.com/metrics-to-evaluate-your-semantic-segmentation-model-6bcb99639aa2](https://towardsdatascience.com/metrics-to-evaluate-your-semantic-segmentation-model-6bcb99639aa2)
3. [https://towardsdatascience.com/understanding-auc-roc-curve-68b2303cc9c5](https://towardsdatascience.com/understanding-auc-roc-curve-68b2303cc9c5)
4. [https://towardsdatascience.com/breaking-down-mean-average-precision-map-ae462f623a52](https://towardsdatascience.com/breaking-down-mean-average-precision-map-ae462f623a52)

__

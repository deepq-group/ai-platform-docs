# Advanced Tips

### Combine labels <a href="#combine-labels" id="combine-labels"></a>

In image classification tasks, although the idea of training a single algorithm to identify numerous classes is appealing, splitting training data among these classes might result in less data per class and eventually causing the neural network unable to learn from the data successfully, thus poor performance.

![](../../.gitbook/assets/DeepCap_Adv_1.png)

Splitting data among more classes causes less data per class, reducing the effective data size for the neural network to learn from.

![](../../.gitbook/assets/DeepCap_Adv_2.png)

During annotation project export, user can choose to export directly from the labels or to combine labels into new ones.

![](../../.gitbook/assets/DeepCap_Adv_3.png)

Click “add a combination” after toggling on the combine label function. User may choose how to combine the classes and assign new class names.

![](../../.gitbook/assets/DeepCap_Adv_4.png)

After combining labels, remember to toggle off the existing labels to prevent the new label to become a multi-label annotation (A single image belongs more than one class, “A1” & “Group A” in this case).

![](../../.gitbook/assets/DeepCap_Adv_5.png)

The combined labels will appear in the new annotation data.

### **Convert labels** <a href="#convert-labels" id="convert-labels"></a>

It happens when a user wants to train a classification AI with object detection annotation data. In order to do so, the labels have to be converted into classification for the algorithms to learn from. DeepQ AI platform provides an easy way for users to convert their label type and try out different applications with the same annotation data.

![](../../.gitbook/assets/DeepCap_Adv_6.png)

During export annotation, choose the annotation type (target) you want, DeepQ AI platform will automatically find out & show the available labels (source) to convert from. The target-source conversion table is listed below.

![](../../.gitbook/assets/DeepCap_Adv_7.png)

![](../../.gitbook/assets/DeepCap_Adv_8.png)

Both detection (object 1) & segmentation (object 2) labels can be converted into classification labels. The new classification label will be names as “object 1” & “object 2”

![](../../.gitbook/assets/DeepCap_Adv_9.png)

Only segmentation labels (object 2) can be converted into detection labels, the label name and number of objects will remain the same after conversion.

---
description: >-
  Datasets are shared between DeepCap and DeepQ AI Training, and can be used for
  annotation, model training and testing.
---

# 🖼 Dataset(s)

### Dataset List <a href="#dataset-list" id="dataset-list"></a>

![](../../.gitbook/assets/DeepCap\_Dataset\_Overview\_Example\_2.png)

* ![](https://console.deepq.ai/docs/console/.gitbook/assets/con-icon-4.png) **Upload Dataset:** Click on this button and upload your dataset in DICOM/ JPG, PNG form.
* ![](https://console.deepq.ai/docs/console/.gitbook/assets/con-icon-6.png) **Search:** Search for your uploaded dataset by its name.
* **Combine**: Combine two or more datasets to form a new dataset. The new dataset can be image-only or contains annotation from the source datasets.&#x20;
* The Dataset list shows all the datasets uploaded by the user and # of studies contained in each dataset
* The number of annotation data attached is shown, each dataset can have multiple annotation data of different types of labeling and number of studies (subsets).
* Users can hide the datasets without annotation by the toggle button "HIDE DATASET WITHOUT ANNOTATION DATA"
* If there is no annotation data, the user has to create an annotation data via annotation project, or else it cannot be used to train an AI model.
* Each dataset can contain multiple annotation data with different types or different number of studies. (the number of studies in an annotation can be a subset of the whole dataset)

### Dataset Detail View & Management <a href="#dataset-detail-view" id="dataset-detail-view"></a>

* Selecting a dataset brings out the detail view, showing the raw data (images) and annotation data attached under this image dataset.
* Owners can delete their datasets by clicking on the option icon "<img src="../../.gitbook/assets/icon_option.png" alt="" data-size="line"> ", a dialogue will pop up to double confirm deletion of the dataset and its derivative results in annotation projects, jobs, training tasks and inference jobs.
* Manually key-in "DELETE" to complete the deletion process.

{% hint style="warning" %}
Deleting a dataset will remove all annotations attached to it and any derivatives on the platform, proceed with caution.
{% endhint %}

![](../../.gitbook/assets/DeepCap\_Dataset\_Detail\_scrolldown.png)

* Clicking on the thumbnail of raw data(image) opens up the image viewer with essential browsing functions such as pan, zoom in/out & brightness/contrast adjustment.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-2-0-4.png)

### Annotation Details

* Selecting any annotation file will open the annotation detail view, showing the information of the annotation file: source, annotation type and its usage across the platform.
* The label distribution statistics is also provided as bar graph or table. &#x20;

![](../../.gitbook/assets/DeepCap\_Dataset\_Detail\_Annotation\_1.png)

* Clicking on each thumbnail opens the image viewer and showing the label information for a more detailed inspection.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-2-0-6.png)

Other than the browsing tools, user can toggle on/off the detection/segmentation labels by clicking on the ![](https://console.deepq.ai/docs/console/.gitbook/assets/con-icon-23.png)

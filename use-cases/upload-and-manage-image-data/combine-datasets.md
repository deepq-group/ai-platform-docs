# Combine Datasets

* Users can create new datasets by combining existing datasets.
* Click on the "**COMBINE**" tab at the upper right corner of the Dataset list

<figure><img src="../../.gitbook/assets/DeepCap_Dataset_Overview_Example_2.png" alt="Select &#x22;Combine&#x22; at the upper right corner to start combining datasets"><figcaption><p>Select "Combine" at the upper right corner to start combining datasets</p></figcaption></figure>

#### Rules of Dataset combination <a href="#rules-of-dataset-combination" id="rules-of-dataset-combination"></a>

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-2-6-0-1.png)

* If all source datasets are images, the combined result will consist only images.
* A new label will be created in the combined result if **at least one label** is selected from source datasets.
* Only **the same type** (classification, detection, segmentation) of labels can be combined.
* Dicom images will be converted to png format if the combination involves mixed image formats.

## Select Datasets <a href="#261-select-datasets" id="261-select-datasets"></a>

First step requires the user to choose source datasets.

<figure><img src="../../.gitbook/assets/Dataset_Combine_1.png" alt="Step #1 of combine dataset shows the list of all uploaded datasets, with or without annotation"><figcaption><p>Step #1 of combine dataset shows the list of all uploaded datasets, with or without annotation</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/Dataset_Combine_2.png" alt="Select more than one datasets to combine"><figcaption><p>Select more than one datasets to combine</p></figcaption></figure>

## Select Annotation Types <a href="#262-select-annotation-types" id="262-select-annotation-types"></a>

<figure><img src="../../.gitbook/assets/Dataset_Combine_4.png" alt="The system will list all the labels of the selected type from each source dataset for the user to select."><figcaption><p>The system will list all the labels of the selected type from each source dataset for the user to select.</p></figcaption></figure>

## Review & Combine <a href="#263-review--combine" id="263-review--combine"></a>

<figure><img src="../../.gitbook/assets/Dataset_Combine_5.png" alt="The last step requires the user to review the combination setting and name the combined dataset."><figcaption><p>The last step requires the user to review the combination setting and name the combined dataset.</p></figcaption></figure>

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-2-6-7.png" alt="Once the combination is successfully processed, the result can be viewed and managed in the dataset list"><figcaption><p>Once the combination is successfully processed, the result can be viewed and managed in the dataset list</p></figcaption></figure>

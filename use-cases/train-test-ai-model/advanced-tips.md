# Advanced Tips



## Dicom Specialized Training (SSDL) <a href="#id-414-dicom-specialized-training-ssdl" id="id-414-dicom-specialized-training-ssdl"></a>

#### Smart Scan Deep Learning (SSDL) <a href="#smart-scan-deep-learning-ssdl" id="smart-scan-deep-learning-ssdl"></a>

Smart Scan Deep Learning (SSDL) is a advanced technique that can optimize the training results of Dicom images. SSDL will automatically activate when Dicom format in the dataset are detected.

#### Prevent Data Leakage <a href="#prevent-data-leakage" id="prevent-data-leakage"></a>

Data Leakage during training happens when the train/validate split is not handled carefully, causing some of the validation data contains information from the training data. As a result the validation score might overperform and be misleading.

In medical scans with image series, information might be shared between slices in a single scan. Therefore, splitting data by study prevents data leakage, as shown in the figure below.

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-7-4-2.3.jpg" alt="SSDL prevents data leakage in sequential images through &#x22;split by study&#x22;"><figcaption><p>SSDL prevents data leakage in sequential images through "split by study"</p></figcaption></figure>

#### Activating SSDL <a href="#activating-ssdl" id="activating-ssdl"></a>

When the user selects a dataset in training tasks, the system will detect whether the dataset contains sequential information.

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-7-1.png" alt="DeepQ AI Platform detects sequential image in a dataset and activates SSDL."><figcaption><p>DeepQ AI Platform detects sequential image in a dataset and activates SSDL.</p></figcaption></figure>

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-7-2.png" alt="DeepQ AI Platform detects sequential image in a dataset and activates SSDL."><figcaption><p>DeepQ AI Platform detects sequential image in a dataset and activates SSDL.</p></figcaption></figure>

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-7-3.png" alt="SSDL showing up in training task detail"><figcaption><p>SSDL showing up in training task detail</p></figcaption></figure>

## AI Assisted Annotation <a href="#id-431-ai-assisted-annotation" id="id-431-ai-assisted-annotation"></a>

An algorithm trained to classify Chest X-ray images cannot help in segmenting tumors in brain MRI since each Deep learning algorithm is task-oriented. AI assisted annotation must start with an neural network trained specifically for the same purpose.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-9.png)

#### AI Training <a href="#ai-training" id="ai-training"></a>

* Create an prediction only batch inference.
* Select the dataset from the inference list, and click on the "EXPORT TO ANNOTATE" tab to start the AI assisted annotation task.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-10.png)

* Name the annotation data that you want to export.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-11.png)

* The column below shows the dataset details, where you can make sure if you have select the right one.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-12.png)

#### DeepCap <a href="#deepcap" id="deepcap"></a>

* Back to DeepCap, and create an annotation project.
* Select the dataset from the drop list, enable the option "Include annotation data", and choose the one that have been annotated by AI.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-3-133.png)

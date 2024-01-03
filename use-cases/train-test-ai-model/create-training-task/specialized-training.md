# Specialized Training

### Specialized Training <a href="#specialized-training" id="specialized-training"></a>

With specialized training, you may choose from the tasks that has been prepared by DeepQ. Users should provide datasets (image format & annotation) according to the table below.

***

### Select Application

<figure><img src="https://console.deepq.ai/docs/console/.gitbook/assets/con-4-1-2-2.3.png" alt=""><figcaption></figcaption></figure>

| Topics                      | Task type                       | Image format              | Classes                                                                                                                                      |
| --------------------------- | ------------------------------- | ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **Intracranial Hemmorhage** | Multi-Label Classification (5)  | Head CT , non-contrast    | <p>>Subarachnoid hemorrhage >Subdural hemorrhage<br>>Epidural hemorrhage<br>>Intraparenchymal hemorrhage<br>>Intraventricular hemorrhage</p> |
| **Pneumothorax**            | Single Label Classification (2) | Chest X-ray               | <p>>PTX<br>>normal</p>                                                                                                                       |
| **Pulmonary Embolism**      | Single Label Classification (2) | Chest CT with contrast IV | <p>>PE<br>>normal</p>                                                                                                                        |



***

## Select Dataset <a href="#411-select-dataset" id="411-select-dataset"></a>

* All training tasks requires the user to select one of the datasets from the drop list.
* Only datasets with annotation corresponding to your selected type will be shown in the list.
* Case preview will be shown below to help you ensure that you select the correct dataset.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-4-1-1-1.png)

***

### Model Tuning

#### Auto Tuning (Default)

<figure><img src="../../../.gitbook/assets/AITraining_Specialized_Tuning_Auto.png" alt=""><figcaption></figcaption></figure>

#### Manual Tuning

<figure><img src="../../../.gitbook/assets/AITraining_Specialized_Tuning_Manual.png" alt=""><figcaption></figcaption></figure>

#### Confirm & start task

<figure><img src="../../../.gitbook/assets/AITraining_Specialized_Tuning_confirm.png" alt=""><figcaption></figcaption></figure>

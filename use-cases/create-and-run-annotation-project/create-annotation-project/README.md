# Create Annotation Project

DeepCap is an annotation tool with a project-based workflow and a simple interface. You can create a new annotation project by completing the following steps: configure project settings, select dataset & define labels and add project members.

\


## 1. Settings <a href="#1-settings" id="1-settings"></a>

### Settings <a href="#settings" id="settings"></a>

Input project information, instruction files, set validation method & project schedule (optional)

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-0.png)

**Input project name and related instruction.**

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-2.png)

* Other than written instructions, project owner can attach additional reference files (jpg, png & pdf)

**Select validation method：**

Choose one of the validation method from the below options. For the detailed explanation of DSV & reviewer, please refer to [Annotation Quality Control](https://console.deepq.ai/docs/console/working-flow/create-an-annotation-project/1.-settings/deepcap-smart-validation-dsv.html).

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-3.png)

**Schedule the project progress (optional).**

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-4.png)

## 2. Dataset & Labels <a href="#2-dataset--labels" id="2-dataset--labels"></a>

### Select Dataset <a href="#select-dataset" id="select-dataset"></a>

* Select one of the datasets that have been uploaded from the drop list.
* Case preview will be shown below to help you ensure that you select the correct dataset.
* You can choose to include the annotation data.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-2-1.png)

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-2-2.png)

### Label Setting <a href="#label-setting" id="label-setting"></a>

* Chose one or more label types that you want to add on the dataset.
* Define the label names for each label type.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-2-1-3-2.png)

### Task definition <a href="#task-definition" id="task-definition"></a>

* **Single-Label Image Classification:** Only one label can be marked on a case.
* **Multi-Label Image Classification:** multiple labels can be marked on a case.
* **Object Detection:** Use bounding box to detect and identify target objects.
* **Object Segmentation:** To segment and define the ROI (region of interest).

## 3. Members <a href="#3-members" id="3-members"></a>

### Assign Annotators/Reviewers <a href="#assign-annotatorsreviewers" id="assign-annotatorsreviewers"></a>

Only users who have already registered on this platform can be invited as annotator/reviewer. Each annotator can be removed after selection.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-3-1.png)

## 4. Publishing <a href="#4-publishing" id="4-publishing"></a>

### Publish Project <a href="#publish-project" id="publish-project"></a>

The final step before publishing an annotation project is to review the settings.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-4-1.jpg)

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-1-4-4.png)

The annotation project can be published once the settings are correct. All the participated annotators would receive an invitation mail, and the annotation process is initiated.

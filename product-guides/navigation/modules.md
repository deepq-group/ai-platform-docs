# 🧱 Modules

The moment you log into DeepQ AI Platform, you can choose from the three modules to start from. Please contact the system admin for your module authorization.

The complete DeepQ AI Platform consists of three main modules：

* <img src="../../.gitbook/assets/AIP_DeepCap_icon.png" alt="" data-size="line">[**DeepCap**](modules.md#deepcap-overview)**：**Dataset management & image annotation
* <img src="../../.gitbook/assets/AIP_ AI Training_icon.png" alt="" data-size="line">[**AI Training**](modules.md#ai-training-overview)**：**Model selection/tuning & evaluation
* <img src="../../.gitbook/assets/AIP_Deeploy_icon.png" alt="" data-size="line">[**Deeploy**](modules.md#deeploy-overview)**：**Real-time model deployment, worklist & AI viewer

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-1-2-1.png)



<figure><img src="../../.gitbook/assets/AIP_whole.png" alt="The complete DeeQ AI Platform"><figcaption><p>The complete DeeQ AI Platform</p></figcaption></figure>

### DeepCap <a href="#deepcap-overview" id="deepcap-overview"></a>

The quality & quantity of datasets is the key to high performing AI models, but traditionally, preparing datasets is a tedious and lengthy process. DeepCap is designed with a highly intuitive interface, and includes critical features such as project management, AI-assisted annotation, and smart validation, to help you better prepare high-quality reliable data for training.

![](../../.gitbook/assets/DeepCap.png)

**Project**: Person who create a project will be the project owner. The project owner can check and manage all the projects in this tab.

**Dataset**: You can upload datasets in this tab.The system has imposes some limitations on your dataset, please refer to the [“Dataset Format”](https://app.gitbook.com/s/-LRpbrznmSNshCiwmSTG-3251841457/dataset/upload-dataset) and[ "Annotation Data Format"](https://app.gitbook.com/s/-LRpbrznmSNshCiwmSTG-3251841457/dataset/annotation-data-formats) tab for detailed information.

**My Job**: Annotators/Reviewers can view and work on the jobs assigned to them by a project owner.

***

### AI Training <a href="#ai-training-overview" id="ai-training-overview"></a>

Our no-code AI training module eliminates the entry barrier of AI. Without any computer science background necessary, all you need is a good idea and data, our AutoML engine kicks in to train a high performing model in the least amount of time.

\


![](<../../.gitbook/assets/AI Training.png>)

​

‌**Task**: All information regarding model training can be found here Person who create a task will be the project owner. The project owner can check and manage all the tasks in this tab.‌

#### **Model:**&#x20;

**Dataset**: You can upload datasets in this tab.The system has imposes some limitations on your dataset, please refer to the [“Dataset Format”](https://app.gitbook.com/s/-LRpbrznmSNshCiwmSTG-3251841457/dataset/upload-dataset) and ["Annotation Data Format"](https://app.gitbook.com/s/-LRpbrznmSNshCiwmSTG-3251841457/dataset/annotation-data-formats) tab for detailed information.

Models:&#x20;

### Deeploy  <a href="#deeploy-overview" id="deeploy-overview"></a>

Model Deployment is the last piece of an MLOPs cycle and it is where the power of AI brought to light. Improve performance and efficiency in your clinical workflow with Deeploy.

![](../../.gitbook/assets/Deeploy.png)

**Worklist**: A complete list of the image studies processed by model deployments that are authorized to you, shown from newest to oldest. Users can filter the worklist by selecting models by clicking on "**MODEL**".

**Authorized Models**: You can view the details of model deployments that are authorized to you. please contact system admin for model deployment authorization.

{% hint style="warning" %}
"Deeploy" Module is designed mainly for on-premise operations and will not be explained in this user guide
{% endhint %}

### Module permission <a href="#module-permission" id="module-permission"></a>

DeepQ AI Platform module & function permission is listed in the table below. Users can click on the upper right corner to switch modules, or contact the system administrator to check which modules do you have permission to access.

<table><thead><tr><th width="300">Functions</th><th width="126">DeepCap</th><th width="116">AI Training</th><th>Deeploy</th></tr></thead><tbody><tr><td>Upload/manage dataset</td><td>V</td><td>V</td><td></td></tr><tr><td>Create/manage annotation project</td><td>V</td><td></td><td></td></tr><tr><td>Annotate/review image(s)</td><td>V</td><td></td><td></td></tr><tr><td>Create/manage training tasks</td><td></td><td>V</td><td></td></tr><tr><td>Evaluate training tasks</td><td></td><td>V</td><td></td></tr><tr><td>View model deployments (worklist &#x26; viewer)</td><td></td><td></td><td>V</td></tr></tbody></table>


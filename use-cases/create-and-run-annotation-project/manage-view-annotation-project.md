# Manage/View Annotation Project

## Manage Annotation Projects <a href="#33-manage-annotation-projects" id="33-manage-annotation-projects"></a>

Once an annotation project has been published and running, the project owner can view and manage the project anytime.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-3-1.png)

### View Details <a href="#view-details" id="view-details"></a>

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-3-2.png)

* **Project schedule:** The summary of project schedule is shown here to help the project owner review the progress.
* **Annotation progress:** If the iteration you set is three, then the quantity of "Annotated" is equal to the annotation quantity that is completed by three annotators.
* **Review progress:** This column shows the review progress that has completed by the reviewer.
* **Export to training:** You can directly export the annotated data to DeepQ AI Training service by clicking on the bottom.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-3-3.png)

* You can add new annotators before the project is stopped and completed. The cases will be re-allocated once you add new annotators.
* An annotator/ reviewer can be suspended or removed from the project.
  * **Suspend:** An annotator’s job will be released when they are suspended from the project. The suspended status can be resumed.
  * **Remove:** An annotator’s job will be released when they are removed from the project. A removed annotator cannot be added again once removed by a project owner.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-3-4.png)

* **Filter | Sort by:** Study name, Last finished, Lowest DSV: classification, Lowest DSV: segmentation, Lowest DSV: detection, depends on the project type.
* **Export:** You can also export the annotated data to DeepQ AI Training service directly.

### Export Annotated Dataset for Training <a href="#export-annotated-dataset-for-training" id="export-annotated-dataset-for-training"></a>

Dataset that cannot be exported for training.

* Without annotation result: There is no any saved annotations for this dataset.
* User exclude: A project Owner excludes (![](https://console.deepq.ai/docs/console/.gitbook/assets/con-icon-9.png)) that case.
* System exclude: The DSV result excludes that case because of an unacceptably lower consistency rate.
* Problematic image: Annotated as “Problematic image” by an annotator.


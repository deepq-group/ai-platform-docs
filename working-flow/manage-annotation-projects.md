# 3.3 Manage Annotation Projects

Once an annotation project has been published and running, the project owner can view and manage the project anytime.

![](<../.gitbook/assets/manage annotation project .png>)

## View Details

![](<../.gitbook/assets/view detail.png>)

* **Project schedule:** The summary of project schedule is shown here to help the project owner review the progress.
* **Annotation progress:** If the iteration you set is three, then the quantity of "Annotated" is equal to the annotation quantity that is completed by three annotators.
* **Review progress:** This column shows the review progress that has completed by the reviewer.
* **Export to training:** You can directly export the annotated data to DeepQ AI Training service by clicking on the bottom.

![](<../.gitbook/assets/add member (1).png>)

* You can add new annotators before the project is stopped and completed. The cases will be re-allocated once you add new annotators.
* An annotator/ reviewer can be suspended or removed from the project.
  * **Suspend:** An annotator’s job will be released when they are suspended from the project. The suspended status can be resumed.
  * **Remove:** An annotator’s job will be released when they are removed from the project. A removed annotator cannot be added again once removed by a project owner.

![](<../.gitbook/assets/annotation dataset.png>)

* **Filter | Sort by:** Study name, Last finished, Lowest DSV: classification, Lowest DSV: segmentation, Lowest DSV: detection, depends on the project type.
* **Export:** You can also export the annotated data to DeepQ AI Training service directly.

## Export Annotated Dataset for Training

Dataset that cannot be exported for training.

* Without annotation result: There is no any saved annotations for this dataset.
* User exclude: A project Owner excludes (![](<../.gitbook/assets/image (10).png>)) that case.
* System exclude: The DSV result excludes that case because of an unacceptably lower consistency rate.
* Problematic image: Annotated as “Problematic image” by an annotator.
*   <mark style="color:red;">**The minimum annotation requirement for each class is 3 images. If the annotation contains class(es) with less than 3 images, it cannot be exported.**</mark>

    #### \*\*\*\*

## Annotation Conditions for Training

To deliver the best possible training performance, please ensure that your annotation meets our system requirements.

* **Image Classification**:

The annotated dataset should contain at least two categories and each category should be used as an annotation on at least two cases. For example: Class“A” was used on case 001 and case 002, and Class“B” was used on case 003 and case 004.

| Dataset  | Annotation |
| -------- | ---------- |
| Case 001 | A          |
| Case 002 | A          |
| Case 003 | B          |
| Case 004 | B          |

* **Object Detection**

The annotated dataset must contain at least three cases, and each case should be annotated with at least one bounding box.\
For example, Cases 001, 002, and 003 should be annotated with at least One bounding box.

| Dataset  | Annotation                |
| -------- | ------------------------- |
| Case 001 | Bounding Box with Tag “A” |
| Case 002 | Bounding Box with Tag “A” |
| Case 003 | Bounding Box with Tag “B” |

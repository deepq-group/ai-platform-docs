# Basic Annotation

## Start Annotation <a href="#32-start-annotation" id="32-start-annotation"></a>

Image annotation is the process of labeling or adding metadata to images to describe and identify objects, features, or attributes within those images. It involves marking or outlining specific areas or elements of an image to provide contextual information or categorization for machine learning algorithms.

In essence, image annotation is a fundamental process in computer vision, enabling machines to understand and interpret visual data by providing contextual information and labels crucial for training AI models.\


### My Job--Job List <a href="#my-job--job-list" id="my-job--job-list"></a>

Click on the "**My Job**" tab, you can view the job list that was assigned by the project owner. The total cases that have been assigned to you and the cases that have not been annotated is shown in each job. Click on "**ANNOTATE**" or "**REVIEW**"and begin the annotation process.

![](../../.gitbook/assets/DeepCap\_Jobs\_Overview\_Ongoing.png)

### Annotation Job--Detail Page <a href="#annotation-job--detail-page" id="annotation-job--detail-page"></a>

All information an annotator needs to know is shown in the annotation job detail page, from annotation progress in terms of # of jobs left & completion percentage, method & labels and the project owners instructions.

![](../../.gitbook/assets/DeepCap\_Jobs\_Detail\_1.png)

Scroll down to check the image studies assinged to you. Studies that have been annotated and subitted will have a green check mark on its thumbnail. You may select any study to start annotating, or simply click on "**ANNOTATE**" to start from the first unsubmitted study.

![](../../.gitbook/assets/DeepCap\_Jobs\_Detail\_2.png)

| Column Name       | Description                                                                      |
| ----------------- | -------------------------------------------------------------------------------- |
| My annotation job | Cases that have not been annotated.                                              |
| Progress          | The completion percentage of this project.                                       |
| Annotation Method | Annotation Method setting information.                                           |
| Study             | All the cases will be shown here, you can choose whichever you want to annotate. |

You can filter the studies by annotation status: Remaining, Finished, Returned.

### Image Annotation <a href="#image-annotation" id="image-annotation"></a>

#### Annotation view instructions: <a href="#annotation-view-instructions" id="annotation-view-instructions"></a>

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-2-4.png)

* Choose the annotation labels from the right column to add on the image.
* You can select one of the labels for the entire case. If there are no labels can be annotated, please select “Nothing to Label”.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-2-5.png)

* You can view the WW/WL of that image by the top left button, select it to adjust the WW/WL of the image.
* Click on ![](https://console.deepq.ai/docs/console/.gitbook/assets/con-icon-6.png) and slide to zoom in and zoom out the images.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-2-6.png)

* The annotator may also leave image-level or object-level comments in the annotation viewer. the comments will be passed down to the reviewer/project owner and will be recorded in the annotation project detail.

**After labeling the case:**

Click on “**SUBMIT**” after annotating each case. You can also click on “**<<**” to go back to the last case or click on “**>>**” to go to the next page without submission.

**Notice:**

* Once the case is submitted, the label cannot be changed unless returned by reviewer
* For larger images (>1000 both side), it may take some time to process complex annotation (e.g. segmentation), therefore it takes a while to reflect the changes after submit.

### Review job -- Detail Page <a href="#review-job----detail-page" id="review-job----detail-page"></a>

Once you click on the review job assigned to you, the ncessary review job information can be found in this overview page: review progress in terms of # of jobs left & completion percentage, method & labels and the project owners instructions and all review jobs and their respective status listed below.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-2-7.png)

All assigned studies that have been annotated/submitted by annoatators and waiting to be reviewed will appear on the list at the bottom.

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-2-8.png)

### Annotation Review <a href="#annotation-review" id="annotation-review"></a>

![](https://console.deepq.ai/docs/console/.gitbook/assets/con-3-2-9.png)

* **Pass**：The annotation result meets the standard of the project and can be sent to training
* **Fail**：The annotation or image does not qualify and therefore should be excluded and cannot be used to train models.

Make sure to click on "**SUBMIT**" button to send out your review results

{% hint style="warning" %}
Annotation cannot be modified once it is submitted, so make sure the annotation is correct before pressing the "SUBMIT" button!!
{% endhint %}



* **Return**：The annotation is sent back to the annotator with comments attached.

Comments can also be left as it is done in the annotation process.

# Start Annotation

Click on the "My Job" tab, you can view the job list that was assigned by the project owner. The total cases that have been assigned to you and the cases that have not been annotated is shown in each job. Click on "ANNOTATE" and begin the annotation process.

![](../.gitbook/assets/my-job.png)

## Detail Page

![](../.gitbook/assets/detail-page-.png)

![](../.gitbook/assets/detail-page-2.png)

| Column Name | Description |
| :--- | :--- |
| My annotation job | Cases that have not been annotated. |
| Progress | The completion percentage of this project. |
| Annotation Method | Annotation Method setting information. |
| Study | All the cases will be shown here, you can choose whichever you want to annotate. |

You can filter the studies by annotation status: Remaining, Finished, Returned.

## Image Annotation

### Annotation view instructions:

![](../.gitbook/assets/annotation-labels.png)

* Choose the annotation labels from the right column to add on the image.
* You can select one of the labels for the entire case. If there are no labels can be annotated, please select “Nothing to Label”. 

![](../.gitbook/assets/ww-wl.png)

* You can view the WW/WL of that image by the top left button, select it to adjust the WW/WL of the image. 
* Click on ![](../.gitbook/assets/filled-copy-2-1-.svg) _\*\*_ and slide to zoom in and zoom out the images. 

#### After labeling the case:

Click on “SUBMIT” after annotating each case. You can also click on “&lt;&lt;” to go back to the last case or click on “&gt;&gt;” to go to the next page without submission.

#### Notice:

Once the case is submitted, the label cannot be changed.

#### 

### Special features

###  **Propagate labels**

When annotating serial images such as CT or MRI, the user might want to duplicate labels for continuous slices such as the example shown below. Instead of clicking through each slice, “propagate label” function allows users to label multiple slices with ease.

![](../.gitbook/assets/image%20%28123%29.png)

“propagate label” will significantly reduce the effort needed to label continuous slices with the same label



![](../.gitbook/assets/image%20%28184%29.png)

In the annotation viewer, “propagate label” will automatically show up if the job is annotating continuous slices.





![](../.gitbook/assets/image%20%28208%29.png)

By clicking on “propagate labels”, the user is able to choose which slices will be tagged with the same label, and the type of label that will be assigned to these slices. For detection and segmentation, the user can simply assign “nothing to label” where the object does not exist. User can also exclude continuous slices in the same way by toggling “Exclude image”

![](../.gitbook/assets/image%20%28207%29.png)

After assigning specific slices with the same label, the slice indicator below will show that the slices have been labeled \(colored segments, representing labeled slices\).

### Combine labels

In image classification tasks, although the idea of training a single algorithm to identify numerous classes is appealing, splitting training data among these classes might result in less data per class and eventually causing the neural network unable to learn from the data successfully, thus poor performance.

![](../.gitbook/assets/image%20%28190%29.png)

Splitting data among more classes causes less data per class, reducing the effective data size for the neural network to learn from.


# 2.3 Import LabelMe annotation

**DeepQ AI platform label format support: LabelMe**

Other than DeepQ AI platform’s annotation format, we also support other annotation produced by other popular image labeling tools such as LabelMe. LabelMe is a project created by the MIT Computer Science and Artificial Intelligence Laboratory (CSAIL) and is widely used in computer vision research. DeepQ AI platform supports 3 types of annotation created by LabelMe: Classification, Detection & Segmentation.

![Annotation type nomenclatures](<../.gitbook/assets/image (125).png>)

![](<../.gitbook/assets/image (168).png>)

![](<../.gitbook/assets/image (167).png>)

* LabelMe annotation file consists of the following coding segments: Label Data, Image path & Image data
* A single LabelMe .json contains all types of annotation data of a single image, therefore the number of .json files should match the number of images.
* In the label data section, label type, class name & coordinates (rectangular & segmentation) is described.
* The image path points to the corresponding image which the annotation is created.
* The encoded image string stores a lossless copy of the image within the .json, therefore an individual image file is not required.
* DeepQ AI platform currently supports classification, detection & segmentation annotation data & models. Other labeling types such as points, circles, lines & linestrips can be uploaded & processed but might encounter errors during training task setup.

![](<../.gitbook/assets/image (128).png>)

If “Save with Image Data” is checked with LabelMe settings, image data will be embedded as text string in .json files and separate image file will not be required. However, if image file is provided along with a correct image path, it will be used as 1st priority over the embedded image.

![](<../.gitbook/assets/image (165).png>)

Once the LabelMe zip is successfully uploaded, the system will automatically create annotation data from the .json files. Note that each .json zip will produce at least one classification annotation, on top of other types of label data. \\(Detection & segmentation\\)

![](<../.gitbook/assets/image (166).png>)

* <mark style="color:red;">**The minimum annotation requirement for each class is 3 images. If the LabelMe dataset contains class(es) with less than 3 images, the dataset will be rejected**</mark>

## \*\*\*\*

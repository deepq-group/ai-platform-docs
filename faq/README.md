# FAQ

### General issues

**Q. What browsers are compatible with DeepQ AI Platform?**\
****A. Although our service works with all major browsers, we suggest users to run DeepQ AI platform on Google Chrome for your best experience.&#x20;

**Q. I forgot my password, what should I do?**\
****A. Please contact DeepQ customer service to reset your password and you should receive an email shortly afterwards.

**Q. The screen becomes unresponsive/freezes, what should I do?**\
****A. When uploading large datasets, it takes longer for the system to unzip/process the images/labels. You may try to refresh or even restart the browser if necessary. &#x20;



### Dataset Related

**Q. What is the max/min resolution for each image?**\
****A. The resolution of all uploaded image should be between 16px and 4096px in both width and height.

**Q. What is the max. size of each image?**\
****A. No, there is no restriction for single image size.

**Q. What is the max. size of each dataset .zip file?**\
****A. No, there is no restriction for dataset .zip file size. Technically however, zip files have a size limit of about 4 GB, and there are tools that can create .zip files greater than 4GB.

**Q. My uploaded dataset failed to process, what might be wrong?**\
1\. Check the .zip file structure.\
2\. Check the image formats: .jpg, .png & DICOM (.dcm) formats.\
3\. Check for duplicate image names in different folders , rename images with the same filename\
4\. make sure image filenames do not contain invalid characters, and replace spaces with underlines\
5\. For .dcm files, make sure that there are no duplicates, or files that share the same DICOM information.

**Q. My uploaded labeling information did not successfully process**\
****A. Please make sure that the uploaded label file follow the rules of DeepQ AI Platform instructed in [Annotation Data Formats](../dataset/annotation-data-formats.md). other than format, a valid label file consists of a minimum 3 images per class. the label file cannot be processed if it does not meet this criteria.

### Annotation related

**Q. Other than classification & detection, can I upload my segmentation labels?**\
****A. Other than LableMe, we currently do not support other segmentation formats.&#x20;

**Q. Does DeepCap support touchscreen and stylus?**\
****A. Yes, DeepCap supports mouse input, touchscreen and stylus (Apple pencil). other than iPad & Apple pencil, some tablet devices can configure stylus working in "mouse mode", and can be used to annotate.

**Q. What can I expect from AI assisted annotation?**\
****A. Since Deep Learning models were trained to perform specific tasks. One cannot expect models trained for other tasks to assist the labeling of your specific purpose. for instance, a liver segmentation model train on abdominal CT will fail to segment tumor in brain MRI. \
&#x20;    The best way is to leverage AI in annotation is to train a model with available data and run it on images that have yet been labeled. DeepCap supports export partially annotated data to training for the first part, and the AI labeled images can be sent to an annotation project for human inspection/review.

**Q. I cannot export my annotation project, what might go wrong?**\
****A. A valid label file consists of a minimum 3 images per class. the annotation job cannot be exported if it does not meet this criteria.

### Model Training Related

**Q. Can I estimate how long will a training job take?**\
****A. The total training job consists of numerous variables, from training data size, model types, model capacity, tuning strategy, early stop mechanism...etc. and cannot be easily predicted.&#x20;


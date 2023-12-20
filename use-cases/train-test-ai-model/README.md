# 👨🔬 Train/Test AI Model

### Deep Learning Pipeline <a href="#41-create-training-tasks" id="41-create-training-tasks"></a>

In the realm of deep learning, the process unfolds in distinct phases: training, testing, and production. During the training phase, the model learns from labeled data, adjusting its parameters to make accurate predictions. Subsequently, the model is subjected to the testing phase, where its performance is evaluated on unseen data to ensure generalization. Finally, in the production phase, the trained and tested model is deployed for real-world applications, making predictions on new, unseen data. Each phase plays a crucial role in developing robust and effective deep learning models for a variety of practical use cases.

<figure><img src="../../.gitbook/assets/DL_pipeline_full.png" alt=""><figcaption></figcaption></figure>

The 3 phases explained with a dog/cat image classifier:

### Training Phase

* **Training:** During this phase, the computer is shown lots of labeled pictures of dogs and cats. It learns to recognize patterns—like shapes, fur textures, and colors—associated with each animal.
* **Adjusting Parameters:** The model adjusts its internal settings (parameters) based on these examples to get better at telling dogs apart from cats. It learns the differences between the two animals.



### Testing Phase

Model training represents only half of the equation; the real challenge lies in testing it with real-world data. Deploy your models and generate inference results by running them on data with ground truth, yielding objective outcomes for further analysis.

<mark style="color:red;">In the testing phase of deep learning, it's like checking how well your friend learned to recognize fruits. You show them new pictures of fruits they haven't seen before and ask what each one is. If your friend can correctly name most of the fruits they haven't seen, they've learned well. Similarly, in deep learning, the computer uses new pictures it hasn't learned from before to see how good it is at recognizing things. If it can accurately figure out these new pictures, it shows that it's learned properly.</mark>

* **Testing:** Once the model has learned from the training data, it's tested with new, unseen pictures of dogs and cats that it hasn't studied before.
* **Assessing Accuracy:** The model tries to classify these new images as either dogs or cats. The accuracy is measured by how many it gets right. For example, if it correctly identifies 9 out of 10 new images, it's 90% accurate.

### Production Phase

In the production phase of deep learning, it's like your friend helping others recognize fruits. Your friend has learned a lot about fruits and can now tell what they are. Similarly, the computer, after learning from many examples, is ready to help with real tasks. It uses its knowledge to identify things in new pictures or situations, just like your friend helps others recognize fruits by sharing what they've learned.

* **Real-world Application:** In the production phase, the trained model is deployed for practical use. It's like using the trained model in a pet adoption center to identify animals in incoming pictures.
* **Practical Use:** When a new picture of an animal arrives, the model uses what it's learned from training to decide if it's a dog or a cat. It's essentially using its knowledge to perform the task it was trained for.

\
\


\

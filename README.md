# dog-vision-classification

* Problem statement:
This is a dog breeds identification machine learning problem, which has used the Kaggle.com competion datasets. The task is to build a deep learning model (uses transfer learning model mobileNetV2 model) to train, validate (experiment) and then use the full data to train the model and make predictions on the test dataset. The deep learning model has to learn image feature of each class across the 120 classes and match the respective labels to identify which label each image falls on.

* Nature of Data:
The data used for this project is from Kaggle's dog breed identification competition where there are 120 different classes (dog breeds) with more than 10,000 images in total. The training set has both images and labels while the test dataset has images only (no labels (dog unique breeds).
https://www.kaggle.com/c/dog-breed-identification/data

* Evaluation:
According to the kaggle.com competiton, evaluation is a file with prediction probabilities for each dog breed of each test image, which is a DataFrame indexed by the images ID's falling under each of the 120 class. Hence, the shape of the DataFrame is structure such that (image_ids (rows), dog classes (columns)).
https://kaggle.com/c/dog-breed-identification/evaluation

* Dataset Features: 
Some information about the data:
  * Images (unstructured data) so it's probably best done using deep learning/transfer learning.
  * There are 120 dog breeds (meaning there are 120 different classes).
  * There are around 10,000+ images in the training set (images have labels).
  * There are around 10000+ images in the test set (these images have no labels, because the classifier should be able to handle indicating the respective breed name/class).
 
* Model used:
The model selection adopted a transfer learning approach whereby an already trained model selected (MobileNetV2) for image classification and customized accordingly to suit the purposes for this project problem statement.
 
* Experimentation:
Experimentation of successful working of the model was done on 1,500 images split into training set (1,200) and validation set (300). Training the model, was able to perfectly learn on training set with accuracy of 100% and about 72% on validation set (kind overfitting because of small dataset used). The good thing at this stage is that the learning of the model on the dataset was successfully.

* Scalling up:
Experimented model was full trained on the entire training set from which the predictions on the test set were done.

* Deployment/usability:
The full trained model - tested on the entire test set was then applied to make predictions on 9 custom dog images, which has 100% correctly identified which breed each image belongs.

![image](https://github.com/user-attachments/assets/acab307a-4278-4fc7-a31f-550c7bccafee)




****Emotion Detection CNN Model****

**Introduction**

This project aims to classify the emotion on a person's face into one of seven categories, using deep convolutional neural networks. The model is trained on the FER-2013 dataset which was published on International Conference on Machine Learning (ICML). This dataset consists of 35887 grayscale, 48x48 sized face images with seven emotions - angry, disgusted, fearful, happy, neutral, sad and surprised.

**Dependencies**

Python 3, OpenCV, Tensorflow, sklearn, numpy, pandas and matplotlib

**Dataset Sources**
Kaggle - https://www.kaggle.com/datasets/msambare/fer2013

**Basic Usage**

The repository is currently compatible with tensorflow-2.0 and makes use of the Keras API using the tensorflow.keras library.

**Workflow Diagram**


<img width="904" alt="Emotion_detection_WorkFlow" src="https://github.com/sambhavm22/Emotion-Detection-Model/assets/58766591/523d2851-a002-4a5d-ae54-0345f368731a">


**Image Distribution for each class**

<img width="983" alt="Screenshot 2024-04-25 at 11 49 12 AM" src="https://github.com/sambhavm22/Emotion-Detection-Model/assets/58766591/d8f9b43e-5d0a-4cd5-917c-a0c2f8b7267b">





Since the image distribution for each category with imbalanced , I have use class weights.



**Result**




The best result come with ResNet50 Model that was able to detect the face emotion with a goof accuracy. With 22,779,527 trainable parameters, the test accuracy reached 60.8% in 50 epochs.



**ResNet50 Model Architecture**

<img width="960" alt="Screenshot 2024-04-25 at 12 37 25 PM" src="https://github.com/sambhavm22/Emotion-Detection-Model/assets/58766591/74b64f65-5f14-4ac7-b5f7-2a3c01ef8202">



**Accuracy and Validation Graph of the best Model**





<img width="888" alt="Screenshot 2024-04-25 at 11 54 13 AM" src="https://github.com/sambhavm22/Emotion-Detection-Model/assets/58766591/f6d2f45a-ee3c-49b7-961a-fa8b29137150">




**Confustion Matrix with the best Model**



<img width="802" alt="Screenshot 2024-04-25 at 11 54 33 AM" src="https://github.com/sambhavm22/Emotion-Detection-Model/assets/58766591/d2c836e3-178c-45a9-873a-a3cedf24d477">




**Algorithm**





1. First, train the data on CNN model from scratch, then with Image Augmentation, then with VGG16 Model and finally with ResNet50 Model. With ResNet50 Model got a decent accuracy.

2. The region of image containing the face is resized to 48x48 and is passed as input to the CNN.

3. The network outputs a list of softmax scores for the seven classes of emotions.

4. The emotion with maximum score is displayed on the screen.




**For more info visit**
https://sambhavm22.medium.com/emotion-detection-model-0819ce26bdad

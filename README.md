****Emotion Detection CNN Model****

**Introduction**
This project aims to classify the emotion on a person's face into one of seven categories, using deep convolutional neural networks. The model is trained on the FER-2013 dataset which was published on International Conference on Machine Learning (ICML). This dataset consists of 35887 grayscale, 48x48 sized face images with seven emotions - angry, disgusted, fearful, happy, neutral, sad and surprised.

**Dependencies**
Python 3, OpenCV, Tensorflow, sklearn, numpy, pandas and matplotlib

**Dataset Sources**
Kaggle - https://www.kaggle.com/datasets/msambare/fer2013

**Basic Usage**
The repository is currently compatible with tensorflow-2.0 and makes use of the Keras API using the tensorflow.keras library.

**Image Distribution for each class**

<img width="983" alt="Screenshot 2024-04-25 at 11 49 12 AM" src="https://github.com/sambhavm22/Emotion-Detection-Model/assets/58766591/d8f9b43e-5d0a-4cd5-917c-a0c2f8b7267b">

**Result**
The best result come with ResNet50 Model that was able to detect the face emotion with a goof accuracy. With 22,779,527 trainable parameters, the test accuracy reached 60.8% in 50 epochs.

**ResNet50 Model Architecture **

<img width="960" alt="Screenshot 2024-04-25 at 12 37 25 PM" src="https://github.com/sambhavm22/Emotion-Detection-Model/assets/58766591/74b64f65-5f14-4ac7-b5f7-2a3c01ef8202">



**Accuracy and Validation Graph**


<img width="888" alt="Screenshot 2024-04-25 at 11 54 13 AM" src="https://github.com/sambhavm22/Emotion-Detection-Model/assets/58766591/f6d2f45a-ee3c-49b7-961a-fa8b29137150">

<img width="802" alt="Screenshot 2024-04-25 at 11 54 33 AM" src="https://github.com/sambhavm22/Emotion-Detection-Model/assets/58766591/d2c836e3-178c-45a9-873a-a3cedf24d477">

**Algorithm**
First, train the data on CNN model, then with Image Augmentation, then with VGG16 Model and finally with ResNet50 Model.

The region of image containing the face is resized to 48x48 and is passed as input to the CNN.

The network outputs a list of softmax scores for the seven classes of emotions.

The emotion with maximum score is displayed on the screen.<img width="860" alt="Screenshot 2024-04-25 at 11 57 09 AM" src="https://github.com/sambhavm22/Emotion-Detection-Model/assets/58766591/b1bf306a-7f62-4876-94cc-0e9d4f8e8b91">




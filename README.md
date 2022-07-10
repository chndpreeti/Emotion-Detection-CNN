# Face-Emotion-Detection

Face Emotions classfication using CNN 

This project aims to classify the emotion on a person's face into one of seven categories, using deep convolutional neural networks. 
The model is trained on the FER-2013 dataset which was published on International Conference on Machine Learning (ICML). 
This dataset consists of 35887 grayscale, 48x48 sized face images with seven emotions - angry, disgusted, fearful, happy, neutral, sad and surprised.


# Dependencies

Python 3, OpenCV, Tensorflow

To install the required packages, run pip install -r requirements.txt.




## Algorithm
First, the haar cascade method is used to detect faces in each frame of the webcam feed.

The region of image containing the face is resized to 48x48 and is passed as input to the CNN.

The network outputs a list of softmax scores for the seven classes of emotions.

The emotion with maximum score is displayed on the screen.



### Example:

![image](https://user-images.githubusercontent.com/46122725/178147886-af0a18ea-0445-415a-83c2-59199789a428.png)
![image](https://user-images.githubusercontent.com/46122725/178147890-314246cc-cc5d-430d-a953-ff2863ab1724.png)
![image](https://user-images.githubusercontent.com/46122725/178147931-6c500b35-2673-4c4e-8bda-8d2e87d46456.png)



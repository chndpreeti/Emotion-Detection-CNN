# Face-Emotion-Detection

This project aims to classify the emotion on a person's face into one of seven categories, using deep convolutional neural networks. 
The model is trained on the FER-2013 dataset which was published on International Conference on Machine Learning (ICML). 
This dataset consists of 35887 grayscale, 48x48 sized face images with seven emotions - angry, disgusted, fearful, happy, neutral, sad and surprised.

## Dataset
This project use Fer2013 Dataset from kaggle competition https://bit.ly/39eIAZm

## Dependencies
Python 3, OpenCV, Tensorflow

## Algorithm

- First, the haar cascade method is used to detect faces in each frame of the webcam feed.

- The region of image containing the face is resized to 48x48 and is passed as input to the CNN.

- The network outputs a list of softmax scores for the seven classes of emotions.

- The emotion with maximum score is displayed on the screen.

#### Model Training :
Run the Train_DATA_Emo.py script. The model will get trained on the dataset.
Model weights will be saved to the data/model directory, and at the completion of the training, the best model will be moved into the data/savedmodels directory.The json file containing the model architecture will also be saved there.

I have trained the model on google colab with 100 epochs achieving 74 % accuracy.


#### Model Testing: 
Run the Test_DATA_Emo.py script. You can edit which model weights and architecture you want to use at the location at the top of the file.


#### Live Emotion Detection: 
Run EvaluateEmotionDetector.py for face detection to detect face emotion by web cam in real time.
The script will output a bounding box around the faces detected and a emotion tag with highest confidence score arounf it.

Below are some example by using the face detection on video files.

### Example:
![image](https://user-images.githubusercontent.com/46122725/178147961-ae774ad0-db46-45cd-af6d-0470d78845ef.png)

![image](https://user-images.githubusercontent.com/46122725/178147931-6c500b35-2673-4c4e-8bda-8d2e87d46456.png)






# CAPSTONE-PROJECT 
We are students from St. Clair College, Group 6, we have undertaken project from CogniXR, in which we have to build and deploy models on their existing website using API which will help them predict the emotions of the clients based on their facial expression and audio input. They will be using this project on their exsiting website to predict the emotions of their clients from the theraphy sessions.

## Models used for predicting emotion from facial expressions
- Used VGG16 with imagenet weights
- Accuracy : 76.43%
- Precision : 52.73%
- Recall : 40.98%
- AUC : 67.83%

## Models used for predicting emotion from audio input
- Used CNN model
- Accuracy : 84.83%
- Precision : 82.14%
- Recall : 81.86%
- AUC : 84.90%

## API implementation (Model_API.py)
- Used flask for making API
- Loaded the save models in the API and performed predictions.
- Passed the predicted values from the API to the webpage to display the results according.
- Webpage displays two bar charts and the predictions of the video and audio predictions made by the API.

## How to run the project
- Before running the Model API.py change the path for load_model function to the path where you have save the pretrained models(We can't upload our trained model for audio and video as it is exceeding the allocated space, so in that case you can create you own model and use it in the API or you can contact any of our team member are they will share with you the trained model by using some other platform).
- Running the Model_API.py will load all the models and run all the functions.
- After successfully running the Model_API.py file, index.html will be loaded on the localhost.
- Once we open the localhost link, we will be asked to upload the video, once we upload the video, the video will be send to the API for predicting its output.
- Once the API has predicted the video input and the audio input the data will be passed to the HTML page and the results willbe displayed in the form of Bar charts and image slider.

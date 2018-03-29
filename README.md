# sentiment_analysis

<b>Instructions</b>
<p>
<b>Run real-time emotion demo:</b>
</p>
<p>
python3 video_emotion_color_demo.py
</p>

<b>Run real-time guided back-prop demo:</b>
<p>
python3 image_gradcam_demo.py
</p>

<p>
<b>Make inference on single images:</b>
 </p>
<p>
python3 image_emotion_gender_demo.py <image_path>
 e.g.
python3 image_emotion_gender_demo.py ../images/test_image.jpg
<p>
 
 <b>Running with Docker<b/b>
 <p>With a few steps one can get its own face classification and detection running. Follow the commands below:</p>
 <p>docker pull ekholabs/face-classifier</p>
<p>docker run -d -p 8084:8084 --name=face-classifier ekholabs/face-classifier</p>
 <p>curl -v -F image=@[path_to_image] http://localhost:8084/classifyImage > image.png</p>

<b>To train previous/new models for emotion classification:</b>
<p>Download the fer2013.tar.gz (https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data)</p>

<p>Move the downloaded file to the datasets directory inside this repository.
 Run the train_emotion_classification.py file
python3 train_emotion_classifier.py
</p>

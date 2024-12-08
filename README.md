Mood for Music (An intelligent mood detection and music recommendation application)
========================================================

The mood detector model detects the mood of the user from still images and video sand recommends music accordingly. The system uses images or video analysis to infer user's mood and provide personalised music recommendation to enhance their emotional experience.
After predicting the emotion from face our system takes the predicted emotion as input and generate recommendation by processing the provided dataset. We will predict the music mood from a model trained with **data_moods.csv**. The recommender system will generate top 40 songs to recommend to the user.

Mood Detection
--------------
**Mood Detection** model will predict one of the emotion among below 7 emotions listed - 
1. Angry 2. Disgust 3. Fear 4. Happy 5. Neutral 6. Sad 7.Surprise

Music Mood Prediction
---------------------

Every songs in the main dataset **data_moods.csv** is predicted to one of the mood among 4 moods listed below-
1. Happy    2. Sad 3. Energetic  4. Calm

By using a music mood classifier model we predicted each songs mood in our intermediate dataset **MusicMood** in the Dataset folder.

Music Recommendation
--------------------
Our main project file is **music_recommender.ipynb** file. This recommendation system is using content based filtering. We follow these steps to recommend music-
* Dataset Pre-processing
* Feature Engineering
* Connect to Music API
* Create Playlist Vector
* Generate Recommendation using cosine similarity

So according to this project, we will take an image of an user and predict emotion using **Mood Detection** model. By prioritizing the songs from our main dataset **MusicMoodFinal.csv** with music mood comparing with different face emotion, this system will generate top 40 songs to recommend for a particular sportify playlist. 



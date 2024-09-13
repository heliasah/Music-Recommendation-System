# Music-Recommendation-System

# Overview
This project implements a content-based music recommendation system using the Spotify API and KMeans clustering. The system recommends songs based on user input and mood clustering. It utilizes features such as acousticness, danceability, energy, and more to cluster songs into distinct moods, then calculates the mean feature vector of the input songs and then finds songs with similar features in the clustered data.

# Setup
Spotify API Credentials
To access the Spotify API, you need to have Spotify API credentials. Set up your SPOTIPY_CLIENT_ID, SPOTIPY_CLIENT_SECRET, and SPOTIPY_REDIRECT_URI as shown below:

```bash
    SPOTIPY_CLIENT_ID = 'your_client_id'
    SPOTIPY_CLIENT_SECRET = 'your_client_secret'
    SPOTIPY_REDIRECT_URI = 'http://localhost:8888/callback'
```
Replace 'your_client_id' and 'your_client_secret' with your actual Spotify API credentials

# Example Usage

 ```bash
    recommended_songs = recommend_songs([{'name': 'Videotape', 'year': 2007},
                                     {'name': 'Smells Like Teen Spirit', 'year': 1991},
                                     {'name': 'Wind Of Change', 'year': 1990},
                                     {'name': 'O Children', 'year': 2004},
                                     {'name': 'Do I Wanna Know?', 'year': 2013}], spotify_df)

 ```
    
Output:

![image](https://github.com/user-attachments/assets/4ed3dd78-0539-4936-ab49-cfc7596809d2)






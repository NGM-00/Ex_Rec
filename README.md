# Spotify-Recommendation-System-With-Deployment

## Planing Stage
In This Project We Build a Spotify Recommendation System as a Machine Learning application

as We Know Spotify is a digital music, podcast, and video service that gives us access to millions of songs and Our Planning 
To build a Spotify Recommender System Using Spotify API.

## First What's A Recommendation System !!
One of the most used machine learning algorithms is recommendation systems. A recommender (or recommendation) system (or engine) is a filtering system which aim is to predict a rating or preference a user would give to an item, eg. a film, a product, a song, etc.

- Spotify use different types of Recommendation Systems which are:
    - Collaborative Filtering Algorithm (Based on users interactions of different track)
    - Content Based Filtering (Based on users demographics and tracks attributes)
    - Natural Language Processing (Based on analyzing tracks lyrics).
- In this project we build our Recommendation System to recommend similar songs to the user input, we used different algorithms which are:
    - Content Based Filtering
    - Clustering
## Data
Data came from 2 sources:
- API Calls of Spotify's Web API to get audio features for each track.
- The Spotify Million Playlist Dataset which contained Four separate JSON files

## Understanding the Dataset:
- The Spotify million playlist dataset consists of 4 JSON dictionary:
    - pid - the playlist ID.
    - name - (optional) - the name of the playlist. For some challenge playlists, the name will be missing.
    - tracks - a (possibly empty) array of tracks that are in the playlist. Each element of this array contains the following fields:
       - pos - the position of the track in the playlist (zero offset)
       - track_name - the name of the track
       - track_uri - the Spotify URI of the track
       - artist_name - the name of the primary artist of the track
       - artist_uri - the Spotify URI of the primary artist of the track
       - album_name - the name of the album that the track is on
       - album_uri -- the Spotify URI of the album that the track is on
       - duration_ms - the duration of the track in milliseconds
    - num_tracks - the total number of tracks in the playlist.
- The Audio Features are scraped from Spotify API using spotipy library, which are:
    - acousticness (A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.)
    - analysis_url (A URL to access the full audio analysis of this track. An access token is required to access this data.)
    - danceability (Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength,     and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.)
    - duration_ms (The duration of the track in milliseconds.)
    - energy (Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range,      perceived loudness, timbre, onset rate, and general entropy.)
id (The Spotify ID for the track.)





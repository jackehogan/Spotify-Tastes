# Spotify-Tastes
Compare Spotify data between users and create playlist of shared tastes.

Run through a Jupyter notebook

You will need to create a dashboard and recieve a client id and secret
https://spotipy.readthedocs.io/en/2.16.0/#

Spotify user data requires authorization, run first cell with spotify username entered as "username" variable. Will prompt authorization.
Either use public playlists or saved songs as data, saved data will require Spotify login/password

Next run following cells to create dataframe of users songs, recommended is using the yearly top 100 or retrieve 1000 most recent in "saved songs"

Repeat with second users data

Create a logistic regression classifier for each user. Use classifier to create playlist of songs with low classification confidence, representing songs in with similar shared  features. 

See graphic featurescomparison.png for visual comparison of users features and points classified as shared.
  blue - first user's songs
  orange - second user's songs
  green - song classified as overlap between users, added to playlist

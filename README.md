# createSpotifyPlaylist

While almost everyone is able to create a free YouTube account, not everyone has access to Spotify Premium. My swim team is constantly adding songs to our shared Spotify playlist, but those who have Apple Music or no music apps tend to be left out. To solve this issue, I created a simple script that takes in a selected Youtube playlist and creates a Spotify playlist with the same songs. Therefore, those without Spotify can simply create or collaborate on a Youtube playlist and share it with someone who has Spotify. They can then use this app to create a Spotify playlist with said songs, which can then be added to our collaborative playlist. This is much more efficient than adding the songs one by one.

See the app in action [here](https://drive.google.com/file/d/1nckzYBobcxktjN7-X1ZinNUhM8Jf9LHH/view?usp=sharing)! (Will open link to Google Drive)

# How to use
Run create_playlist.py. It should prompt you for a playlist ID. Select a public Youtube playlist of songs you would like to add to Spotify. Select the playlist ID, which is located behind the equals sign (=) in the URL.

![alt text](https://github.com/hannahrjiang/createSpotifyPlaylist/blob/main/Images/link.png "Link")

Choose a playlist name and hit enter. The terminal should tell you which songs were successfully added and which were unable to be discovered, and how many songs were added to the playlist. 

![alt text](https://github.com/hannahrjiang/createSpotifyPlaylist/blob/main/Images/Songs.png "Terminal View")

Go to Spotify, and your new playlist should appear.

![alt text](https://github.com/hannahrjiang/createSpotifyPlaylist/blob/main/Images/spotify.png "Spotify View")

# Running the Project
Start by downloading spotify.py, youtube.py, create_playlist.py, and .env.

Create a new app on Spotify. Copy the Client ID and Client Secret into their corresponding variables in the .env file. Hit "edit settings" and scroll to "Redirect URIs." Add http://localhost:5000/callback to the list, then hit save. Back in the .env file, set SPOTIFY_USER_ID to your username and SPOTIFY_REDIRECT_URI to http://localhost:5000/callback. See photo below for details.

![alt text](https://github.com/hannahrjiang/createSpotifyPlaylist/blob/main/Images/spotifyView.png "Spotify View")

For the YOUTUBE_API_KEY, you will need to go to the [credentials page](https://console.cloud.google.com/apis/credentials) in the Youtube API Console. From there, click "create credentials" at the top of the page and select "API Key." Copy the given API key into the corresponding variable in .env.

When all the variable in .env are filled, run the following in your terminal:
```
source .env
```
Then run create_playlist.py. Your script should now work!

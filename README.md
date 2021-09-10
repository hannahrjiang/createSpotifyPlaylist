# createSpotifyPlaylist

While almost everyone is able to create a free YouTube account, not everyone has access to Spotify Premium. My swim team is constantly adding songs to our shared Spotify playlist, but those who have Apple Music or no music apps tend to be left out. To solve this issue, I created a simple script that takes in a selected Youtube playlist and creates a Spotify playlist with the same songs. Therefore, those without Spotify can simply create or collaborate on a Youtube playlist and share it with someone who has Spotify. They can then use this app to create a Spotify playlist with said songs, which can then be added to our collaborative playlist. This is much more efficient than adding the songs one by one.

# How to use
Run create_playlist.py. It should prompt you for a playlist ID. Select a public Youtube playlist of songs you would like to add to Spotify. Select the playlist ID, which is located behind the equals sign (=) in the URL.

![alt text](https://github.com/hannahrjiang/createSpotifyPlaylist/blob/main/Images/link.png "Link")

Choose a playlist name and hit enter. The terminal should tell you which songs were successfully added and which were unable to be discovered, and how many songs were added to the playlist. 

![alt text](https://github.com/hannahrjiang/createSpotifyPlaylist/blob/main/Images/songs.png "Terminal View")

Go to Spotify, and your new playlist should appear.

![alt text](https://github.com/hannahrjiang/createSpotifyPlaylist/blob/main/Images/spotify.png "Spotify View")





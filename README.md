# music-sync
Sync music libraries and playlists between music streaming services

# Important documentation:

* [Spotify API](https://developer.spotify.com/documentation/web-api)
  * [get all playlists](https://developer.spotify.com/documentation/web-api/reference/get-a-list-of-current-users-playlists) (library and catalog)
* [Apple Music API](https://developer.apple.com/documentation/applemusicapi)
  * [get all library playlists](https://developer.apple.com/documentation/applemusicapi/get_all_library_playlists)


# Features:
* Sync Spotify liked songs library to Apple Music library
  * spotify: create a playlist that is a copy of a user's liked songs library
    * there does not seem to be a direct way to fetch all the songs in a user's Spotify library. With the most popular service, users need to manually create a playist including all liked songs, but this should be automated easily
  * Add songs to destination library in the same order they were added in origin library
    * most popular service added my songs in reverse order, so now my library looks like it was in 2019
* Synchronize playlists either live or on intervals
* Fetch user's music taste data that is used to curate recommendations
  * not sure if this is possible with any service tbh... the best solution may just be to copy curated playlists from the service with more data to the preferred service

# music-sync
Sync music libraries and playlists between music streaming services

# Important documentation:

* [Spotify API](https://developer.spotify.com/documentation/web-api)
  * [get all playlists](https://developer.spotify.com/documentation/web-api/reference/get-a-list-of-current-users-playlists) (library and catalog)
* [Apple Music API](https://developer.apple.com/documentation/applemusicapi)
  * [generating developer tokens](https://developer.apple.com/documentation/applemusicapi/generating_developer_tokens)
  * [get all library playlists](https://developer.apple.com/documentation/applemusicapi/get_all_library_playlists)


# Planned features:
* Support for Apple Music and Spotify
    * eventually other services like Soundcloud or Youtube Music
* Sync liked songs across services
  * spotify: create a playlist that is a copy of a user's liked songs library
    * there does not seem to be a direct way to traverse the songs in a user's Spotify library, so we should automatically copy all liked songs into a playlist (with option for deletion afterwards)
  * maintain chronological order
    * mainstream service added my songs in reverse order, so now my library looks like it was in 2019
* Synchronize playlists
  *  either live or on intervals (paid feature? would take resources)
* Transfer user's music taste data
  * not sure if this is possible with any service tbh... it is unlikely that listening history data can be accessed, let alone translated across services
  * the best solution may just be to copy curated playlists from the service with more data to the preferred service

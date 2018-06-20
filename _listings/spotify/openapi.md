---
swagger: "2.0"
x-collection-name: Spotify
x-complete: 1
info:
  title: Spotify
  description: our-web-api-lets-your-applications-fetch-data-from-the-spotify-music-catalog-and-manage-users-playlists-and-saved-music--based-on-simple-rest-principles-our-web-api-endpoints-return-metadata-in-json-format-about-artists-albums-and-tracks-directly-from-the-spotify-catalogue--the-api-also-provides-access-to-userrelated-data-such-as-playlists-and-music-saved-in-a-your-music-library-subject-to-users-authorization-
  version: v1
host: api.spotify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /browse/new-releases:
    get:
      summary: Browse New Releases
      description: '[Get a List of New Releases](https://developer.spotify.com/web-api/get-list-new-releases/)'
      operationId: get-a-list-of-new-releaseshttpsdeveloperspotifycomwebapigetlistnewreleases
      x-api-path-slug: browsenewreleases-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: query
        name: country
        description: The country (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: offset
        description: The index of the first item to return
      responses:
        200:
          description: OK
      tags:
      - Music
      - New Releases
---
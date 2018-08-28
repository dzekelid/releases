---
swagger: "2.0"
x-collection-name: Spotify
x-complete: 0
info:
  title: Spotify Browse New Releases
  description: '[Get a List of New Releases](https://developer.spotify.com/web-api/get-list-new-releases/)'
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---
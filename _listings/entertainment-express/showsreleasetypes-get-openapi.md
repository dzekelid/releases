---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: Entertainment Express Returns a list of Show Release Types.
  description: Release types refer to the type of release and are used in the releases
    object for a show.
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Movies/ReleaseTypes:
    get:
      summary: Returns all Movie ReleaseTypes
      description: 'Release type refers to the release. **EX: Theatrical, Home Video,
        etc.**'
      operationId: GetMovieReleaseTypes
      x-api-path-slug: moviesreleasetypes-get
      responses:
        200:
          description: OK
      tags:
      - Movies
      - ReleaseTypes
  /Shows/ReleaseTypes:
    get:
      summary: Returns a list of Show Release Types.
      description: Release types refer to the type of release and are used in the
        releases object for a show.
      operationId: GetShowReleaseTypes
      x-api-path-slug: showsreleasetypes-get
      responses:
        200:
          description: OK
      tags:
      - Shows
      - ReleaseTypes
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
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 1
info:
  title: Entertainment Express
  description: your-gateway-to-building-incredible-movie-tv-and-game-content-discovery-experiences-
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
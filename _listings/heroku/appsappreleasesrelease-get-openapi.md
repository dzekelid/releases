---
swagger: "2.0"
x-collection-name: Heroku
x-complete: 0
info:
  title: Heroku Get Application Releases
  description: Get application releases.
  version: "1"
host: api.heroku.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/{app}/releases:
    parameters:
      summary: Parameters Application Releases
      description: Parameters application releases.
      operationId: parametersAppsAppReleases
      x-api-path-slug: appsappreleases-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Releases
    get:
      summary: Get Application Releases
      description: List releases for an app.
      operationId: getAppsAppReleases
      x-api-path-slug: appsappreleases-get
      parameters:
      - in: query
        name: Accept
        description: Content type
      - in: header
        name: Accept
        description: Content type
      - in: query
        name: app
        description: The app name
      - in: path
        name: app
      responses:
        200:
          description: OK
      tags:
      - Application
      - Releases
    post:
      summary: Add Application Releases
      description: Add application releases.
      operationId: postAppsAppReleases
      x-api-path-slug: appsappreleases-post
      parameters:
      - in: query
        name: Accept
        description: Content type
      - in: header
        name: Accept
        description: Content type
      - in: query
        name: app
        description: The app name
      - in: path
        name: app
      - in: query
        name: rollback
        description: The release to which to roll back
      responses:
        200:
          description: OK
      tags:
      - Application
      - Releases
  /apps/{app}/releases/{release}:
    parameters:
      summary: Parameters Application Releases
      description: Parameters application releases.
      operationId: parametersAppsAppReleasesRelease
      x-api-path-slug: appsappreleasesrelease-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Application
      - Releases
    get:
      summary: Get Application Releases
      description: Get application releases.
      operationId: getAppsAppReleasesRelease
      x-api-path-slug: appsappreleasesrelease-get
      parameters:
      - in: query
        name: Accept
        description: Content type
      - in: header
        name: Accept
        description: Content type
      - in: query
        name: app
        description: The app name
      - in: path
        name: app
      - in: query
        name: release
        description: The release name
      - in: path
        name: release
      responses:
        200:
          description: OK
      tags:
      - Application
      - Releases
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
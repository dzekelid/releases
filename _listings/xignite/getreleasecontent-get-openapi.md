---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Releases Get Release Content
  description: Return detailed information about a release as well as its content.
  version: v1
host: http://www.xignite.com/
basePath: xReleases.xml/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetEventsReleasedForRange:
    get:
      summary: Get Events Released For Range
      description: Get events released for the specified range.
      operationId: postGeteventsreleasedforrange
      x-api-path-slug: geteventsreleasedforrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Events
      - Released
      - Range
  /GetEventsReleasedForRangeLength:
    get:
      summary: Get Events Released For Range Length
      description: Get events released for the date specified and next number of days
        past it.
      operationId: postGeteventsreleasedforrangelength
      x-api-path-slug: geteventsreleasedforrangelength-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Events
      - Released
      - Range
      - Length
  /GetTopReleasesBySecurity:
    get:
      summary: Get Top Releases By Security
      description: Return the top press releases for a security.
      operationId: GetTopReleasesBySecurity
      x-api-path-slug: gettopreleasesbysecurity-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Top
      - Releases
      - Security
  /GetHistoricalReleasesBySecurity:
    get:
      summary: Get Historical Releases By Security
      description: Return press releases headlines for a security and a date range.
      operationId: GetHistoricalReleasesBySecurity
      x-api-path-slug: gethistoricalreleasesbysecurity-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Releases
      - Security
  /GetTodaysReleasesBySecurity:
    get:
      summary: Get Todays Releases By Security
      description: Return press releases for a security for today.
      operationId: GetTodaysReleasesBySecurity
      x-api-path-slug: gettodaysreleasesbysecurity-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Todays
      - Releases
      - Security
  /GetTodaysMarketReleases:
    get:
      summary: Get Todays Market Releases
      description: Return press releases for today.
      operationId: GetTodaysMarketReleases
      x-api-path-slug: gettodaysmarketreleases-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Todays
      - Market
      - Releases
  /GetTopReleaseSummariesBySecurity:
    get:
      summary: Get Top Release Summaries By Security
      description: Return the top press releases summaries for a security.
      operationId: GetTopReleaseSummariesBySecurity
      x-api-path-slug: gettopreleasesummariesbysecurity-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Top
      - Release
      - Summaries
      - Security
  GetReleaseContent/:
    get:
      summary: Get Release Content
      description: Return detailed information about a release as well as its content.
      operationId: getGetreleasecontent
      x-api-path-slug: getreleasecontent-get
      parameters:
      - in: query
        name: ReleaseID
        description: The press release ID>
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Release
      - Content
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
---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite Global News
  description: financial-news-apis-
  version: 1.0.0
host: globalnews.xignite.com
basePath: xGlobalNews.xml/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
---
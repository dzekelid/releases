---
swagger: "2.0"
x-collection-name: Intrinio
x-complete: 0
info:
  title: Intrinio API Press Releases
  description: Returns the most recent press releases by Nasdaq GlobeNewsire for a
    company.
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /press_releases:
    get:
      summary: Press Releases
      description: Returns the most recent press releases by Nasdaq GlobeNewsire for
        a company.
      operationId: press-releases
      x-api-path-slug: press-releases-get
      parameters:
      - in: query
        name: identifier
        description: the stock market ticker symbol associated with the company&rsquo;s
          common stock
        type: string
      - in: query
        name: page_number
        description: an integer greater than or equal to 1 for specifying the page
          number for the return values
        type: string
      - in: query
        name: page_size
        description: an integer greater than 1 for specifying the number of results
          on each page
        type: string
      - in: query
        name: related
        description: 'filter whether the list returned includes all press releases
          where a company is the subject or only press releases issued by the company:
          all | false | true'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Press Releases
x-streamrank:
  polling_total_time_average: "0.16"
  polling_size_download_average: "30806.53"
  streaming_total_time_average: "0.1"
  streaming_size_download_average: "15431.26"
  change_yes: "52"
  change_no: "3691"
  time_percentage: "39"
  size_percentage: "50"
  change_percentage: "1"
  last_run: "2018-02-19"
  days_run: "3"
  minute_run: "0"
---
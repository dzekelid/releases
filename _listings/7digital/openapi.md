swagger: "2.0"
x-collection-name: 7digital
x-complete: 1
info:
  title: 7digital Purchasing API
  description: the-purchasing-api-allows-3rd-parties-to-deliver-digital-content-to-individual-users-
  version: "1.2"
host: api.7digital.com
basePath: 1.2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  release/chart:
    'get ':
      summary: release/chart
      description: This endpoint returns a chart of the most purchased releases for
        given week. Only albums are included in this chart. To retrieve the most recent
        charts as published on 7digital.com the toDate parameter should be omitted.
      operationId: releasechart
      x-api-path-slug: releasechart-get
      parameters:
      - ~
      - in: query
        name: country
        description: nttttttt 2 letter ISO country code of the country whose releases
          you would like to viewntttttt
      - in: query
        name: imageSize
        description: nttttttt The requested width of the image in pixelsntttttt
      - in: query
        name: page
        description: Page number of the result set
      - in: query
        name: pageSize
        description: Number of items to be returned per page
      - in: query
        name: streamable
        description: If provided search results will contain only releases that can/cannot
          be streamed
      - in: query
        name: toDate
        description: The last day the chart should include data for
      responses:
        200:
          description: OK
      tags:
      - Release
      - Chart
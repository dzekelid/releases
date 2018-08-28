---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Release Static Ip
  version: 1.0.0
  description: Deletes a specific static IP from your account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ReleaseStaticIp:
    get:
      summary: Release Static Ip
      description: Deletes a specific static IP from your account.
      operationId: releaseStaticIp
      x-api-path-slug: actionreleasestaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
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
---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Release Address
  version: 1.0.0
  description: Releases the specified Elastic IP address.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ReleaseAddress:
    get:
      summary: Release Address
      description: Releases the specified Elastic IP address.
      operationId: releaseaddress
      x-api-path-slug: actionreleaseaddress-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address
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
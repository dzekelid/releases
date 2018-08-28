swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 1
info:
  title: AWS Lightsale API
  version: 1.0.0
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
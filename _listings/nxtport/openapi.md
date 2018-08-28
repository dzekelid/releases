swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/releases/:
    post:
      summary: Create release
      description: Serves to create a Container together with its PickupRight that
        gets automatically transferred to the consignee.
      operationId: postApiV1Releases
      x-api-path-slug: apiv1releases-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Release
  /api/v1/containers/{id}/release:
    put:
      summary: Release
      description: Release a container to an organization.
      operationId: putApiV1ContainersRelease
      x-api-path-slug: apiv1containersidrelease-put
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: id of the Container
      responses:
        200:
          description: OK
      tags:
      - Release
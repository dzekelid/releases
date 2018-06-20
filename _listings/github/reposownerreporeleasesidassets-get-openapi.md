---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Get Repos Owner Repo Releases  Assets
  description: List assets for a release
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/releases:
    get:
      summary: Get Repos Owner Repo Releases
      description: Users with push access to the repository will receive all releases
        (i.e., published releases and draft releases). Users with pull access will
        receive published releases only
      operationId: users-with-push-access-to-the-repository-will-receive-all-releases-ie-published-releases-and-draft-r
      x-api-path-slug: reposownerreporeleases-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
    post:
      summary: Add Repos Owner Repo Releases
      description: |-
        Create a release
        Users with push access to the repository can create a release.
      operationId: create-a-releaseusers-with-push-access-to-the-repository-can-create-a-release
      x-api-path-slug: reposownerreporeleases-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
  /repos/{owner}/{repo}/releases/assets/{id}:
    delete:
      summary: Delete Repos Owner Repo Releases Assets
      description: Delete a release asset
      operationId: delete-a-release-asset
      x-api-path-slug: reposownerreporeleasesassetsid-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
      - Assets
    get:
      summary: Get Repos Owner Repo Releases Assets
      description: Get a single release asset
      operationId: get-a-single-release-asset
      x-api-path-slug: reposownerreporeleasesassetsid-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
      - Assets
    patch:
      summary: Patch Repos Owner Repo Releases Assets
      description: |-
        Edit a release asset
        Users with push access to the repository can edit a release asset.
      operationId: edit-a-release-assetusers-with-push-access-to-the-repository-can-edit-a-release-asset
      x-api-path-slug: reposownerreporeleasesassetsid-patch
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
      - Assets
  /repos/{owner}/{repo}/releases/{id}:
    delete:
      summary: Delete Repos Owner Repo Releases
      description: Users with push access to the repository can delete a release.
      operationId: users-with-push-access-to-the-repository-can-delete-a-release
      x-api-path-slug: reposownerreporeleasesid-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
    get:
      summary: Get Repos Owner Repo Releases
      description: Get a single release
      operationId: get-a-single-release
      x-api-path-slug: reposownerreporeleasesid-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
    patch:
      summary: Patch Repos Owner Repo Releases
      description: Users with push access to the repository can edit a release
      operationId: users-with-push-access-to-the-repository-can-edit-a-release
      x-api-path-slug: reposownerreporeleasesid-patch
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
  /repos/{owner}/{repo}/releases/{id}/assets:
    get:
      summary: Get Repos Owner Repo Releases  Assets
      description: List assets for a release
      operationId: list-assets-for-a-release
      x-api-path-slug: reposownerreporeleasesidassets-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: id
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Releases
      - ""
      - Assets
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
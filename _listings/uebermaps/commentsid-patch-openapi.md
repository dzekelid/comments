---
swagger: "2.0"
x-collection-name: uebermaps
x-complete: 0
info:
  title: uebermaps Update comment
  description: Update comment. Wrap comment parameters in [comment].
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /comments/{id}:
    delete:
      summary: Delete comment
      description: Delete comment.
      operationId: comments.id.delete
      x-api-path-slug: commentsid-delete
      parameters:
      - in: path
        name: id
        description: Comment id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Comment
    patch:
      summary: Update comment
      description: Update comment. Wrap comment parameters in [comment].
      operationId: comments.id.patch
      x-api-path-slug: commentsid-patch
      parameters:
      - in: body
        name: comment
        description: Comment attributes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Comment id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Comment
  /maps/{id}/comments:
    post:
      summary: Create map comment
      description: Create map comment. Wrap comment parameters in [comment].
      operationId: maps.id.comments.post
      x-api-path-slug: mapsidcomments-post
      parameters:
      - in: body
        name: comment
        description: comment attributes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: map id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Map
      - Comment
  /spots/{id}/comments:
    post:
      summary: Create spot comment
      description: Create spot comment. Wrap comment parameters in [comment].
      operationId: spots.id.comments.post
      x-api-path-slug: spotsidcomments-post
      parameters:
      - in: body
        name: comment
        description: comment attributes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: spot id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Spot
      - Comment
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
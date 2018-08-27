---
swagger: "2.0"
x-collection-name: Flat
x-complete: 0
info:
  title: Flat Mark the comment as resolved
  description: ""
  termsOfService: https://flat.io/legal
  contact:
    name: Flat
    url: https://flat.io/support
    email: developers@flat.io
  version: 2.1.0
host: api.flat.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /scores/{score}/comments:
    get:
      summary: List comments
      description: This method lists the different comments added on a music score
        (documents and inline) sorted by their post dates.
      operationId: getScoreComments
      x-api-path-slug: scoresscorecomments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - List
      - Comments
    post:
      summary: Post a new comment
      description: |-
        Post a document or a contextualized comment on a document.

        Please note that this method includes an anti-spam system for public scores. We don't guarantee that your comments will be accepted and displayed to end-user. Comments are be blocked by returning a `403` HTTP error and hidden from other users when the `spam` property is `true`.
      operationId: postScoreComment
      x-api-path-slug: scoresscorecomments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Comment
  /scores/{score}/comments/{comment}:
    delete:
      summary: Delete a comment
      description: ""
      operationId: deleteScoreComment
      x-api-path-slug: scoresscorecommentscomment-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Comment
    put:
      summary: Update an existing comment
      description: ""
      operationId: updateScoreComment
      x-api-path-slug: scoresscorecommentscomment-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Existing
      - Comment
  /scores/{score}/comments/{comment}/resolved:
    delete:
      summary: Mark the comment as unresolved
      description: ""
      operationId: markScoreCommentUnresolved
      x-api-path-slug: scoresscorecommentscommentresolved-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Mark
      - Comment
      - As
      - Unresolved
    put:
      summary: Mark the comment as resolved
      description: ""
      operationId: markScoreCommentResolved
      x-api-path-slug: scoresscorecommentscommentresolved-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Mark
      - Comment
      - As
      - Resolved
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
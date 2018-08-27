---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Post Checkin Comments
  description: Posts a comment to this checkin.
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{album}/comments:
    get:
      summary: Get Album Comments
      description: The comments made on this album
      operationId: getAlbumComments
      x-api-path-slug: albumcomments-get
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      responses:
        200:
          description: OK
      tags:
      - Album
      - Comments
    post:
      summary: Post Album Comments
      description: Posts a comment on the album
      operationId: postAlbumComments
      x-api-path-slug: albumcomments-post
      parameters:
      - in: path
        name: album
        description: Represents the ID of the album object
      - in: query
        name: message
        description: Comment text
      responses:
        200:
          description: OK
      tags:
      - Album
      - Comments
  /{checkin}/comments:
    get:
      summary: Get Checkin Comments
      description: All of the comments on this checkin.
      operationId: getCheckinComments
      x-api-path-slug: checkincomments-get
      parameters:
      - in: path
        name: checkin
        description: Represents the ID of the checkin object
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Comments
    post:
      summary: Post Checkin Comments
      description: Posts a comment to this checkin.
      operationId: postCheckinComments
      x-api-path-slug: checkincomments-post
      parameters:
      - in: path
        name: checkin
        description: Represents the ID of the checkin object
      - in: query
        name: message
        description: Comment text
      responses:
        200:
          description: OK
      tags:
      - Checkin
      - Comments
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
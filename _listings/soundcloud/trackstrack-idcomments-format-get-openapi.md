---
swagger: "2.0"
x-collection-name: SoundCloud
x-complete: 0
info:
  title: Sound Cloud Get Tracks Track Comments. Format
  description: Returns comments of a track by track id
  version: 1.0.0
host: api.soundcloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tracks/{track_id}/comments.json:
    get:
      summary: Get Tracks Track Comments
      description: Returns comments of a track by track id
      operationId: getTracksTrackComments.json
      x-api-path-slug: trackstrack-idcomments-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Comments
    post:
      summary: Post Tracks Track Comments
      description: Posts a comments to a track by track id
      operationId: postTracksTrackComments.json
      x-api-path-slug: trackstrack-idcomments-json-post
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Comments
  /users/{user_id}/comments.json:
    get:
      summary: Get Users Comments
      description: Returns a collection of comments made by user id
      operationId: getUsersUserComments.json
      x-api-path-slug: usersuser-idcomments-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Comments
  /me/comments.json:
    get:
      summary: Get Me Comments
      description: Returns a collection of comments made by logged-in user
      operationId: getMeComments.json
      x-api-path-slug: mecomments-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Comments
  /comments/{comment_id}.json:
    get:
      summary: Get Comments
      description: Returns a comment by comment id
      operationId: getCommentsComment.json
      x-api-path-slug: commentscomment-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Comments
  /tracks/{track_id}/comments.{format}:
    get:
      summary: Get Tracks Track Comments. Format
      description: Returns comments of a track by track id
      operationId: getTracksTrackComments.Format
      x-api-path-slug: trackstrack-idcomments-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: track_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Tracks
      - Track
      - Comments
      - ""
      - Format
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
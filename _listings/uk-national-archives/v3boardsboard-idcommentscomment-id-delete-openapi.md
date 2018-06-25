---
swagger: "2.0"
x-collection-name: UK National Archives
x-complete: 0
info:
  title: Getty Images Search API Delete Boards Board Comments Comment
  description: <b>***beta***</b> delete a comment from a board.
  version: "3.0"
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/boards/{board_id}/comments:
    get:
      summary: Get Boards Board Comments
      description: <b>***beta***</b> get comments from a board.
      operationId: getV3BoardsBoardComments
      x-api-path-slug: v3boardsboard-idcomments-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board to retrieve comments from
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Comments
    post:
      summary: Post Boards Board Comments
      description: <b>***beta***</b> add a comment to a board.
      operationId: postV3BoardsBoardComments
      x-api-path-slug: v3boardsboard-idcomments-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board to add a comment to
      - in: body
        name: comment
        description: Comment to be added to the board
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Comments
  /v3/boards/{board_id}/comments/{comment_id}:
    delete:
      summary: Delete Boards Board Comments Comment
      description: <b>***beta***</b> delete a comment from a board.
      operationId: deleteV3BoardsBoardCommentsComment
      x-api-path-slug: v3boardsboard-idcommentscomment-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board containing the comment to delete
      - in: path
        name: comment_id
        description: Specify the comment to delete
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Comments
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
---
swagger: "2.0"
x-collection-name: Getty Images
x-complete: 1
info:
  title: Getty Images
  description: build-applications-using-the-worlds-most-powerful-imagery
  version: 1.0.0
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
      summary: Get comments from a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to retrieve all comments for a specific board.\r\n\r\nYou'll
        need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_GetComments
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
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
      - Comments
    post:
      summary: Add a comment to a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
        this endpoint to add a comment to a board.\r\n\r\nYou'll need an API key and
        a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_AddComment
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
      - in: body
        name: comment
        description: Comment to be added to the board
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
      - Comments
  /v3/boards/{board_id}/comments/{comment_id}:
    delete:
      summary: Delete a comment from a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
        this endpoint to delete a comment from a board.\r\n\r\nYou'll need an API
        key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_DeleteComment
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
      - in: path
        name: comment_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
      - Comments
---
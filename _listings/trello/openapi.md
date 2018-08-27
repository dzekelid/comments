swagger: "2.0"
x-collection-name: Trello
x-complete: 1
info:
  title: Trello
  description: this-document-describes-the-rest-api-of-trello-as-published-by-trello-com---a-hrefhttpstrello-comdocsindex-html-target-blankofficial-documentationa--a-hrefhttpstrello-comdocsapi-target-blankthe-html-pages-that-were-scraped-in-order-to-generate-this-specification-a
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/prefs/comments:
    put:
      summary: Put Boards Preferences Comments
      description: Put boards preferences comments.
      operationId: updateBoardsPrefsCommentsByIdBoard
      x-api-path-slug: boardsidboardprefscomments-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Comments to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Comments
  /cards/{idCard}/actions/comments:
    post:
      summary: Post Cards Actions Comments
      description: Post cards actions comments.
      operationId: addCardsActionsCommentsByIdCard
      x-api-path-slug: cardsidcardactionscomments-post
      parameters:
      - in: body
        name: body
        description: Attributes of Actions Comments to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Actions
      - Comments
  /cards/{idCard}/actions/{idAction}/comments:
    delete:
      summary: Delete Cards Actions Comments
      description: Delete cards actions comments.
      operationId: deleteCardsActionsCommentsByIdCardByIdAction
      x-api-path-slug: cardsidcardactionsidactioncomments-delete
      parameters:
      - in: path
        name: idAction
        description: idAction
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Actions
      - Comments
    put:
      summary: Put Cards Actions Comments
      description: Put cards actions comments.
      operationId: updateCardsActionsCommentsByIdCardByIdAction
      x-api-path-slug: cardsidcardactionsidactioncomments-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Actions Comments to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idAction
        description: idAction
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Actions
      - Comments
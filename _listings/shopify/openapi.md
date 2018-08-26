---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/comments.json:
    get:
      summary: Get a list of all comments
      description: Get a list of all comments.
      operationId: getAdminComments.json
      x-api-path-slug: admincomments-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Comments
  /admin/comments/count.json:
    get:
      summary: Get a count of all comments
      description: Get a count of all comments.
      operationId: getAdminCommentsCount.json
      x-api-path-slug: admincommentscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Comments
---
---
swagger: "2.0"
info:
  title: Disqus Posts Spam
  description: Posts Spam
  termsOfService: https://docs.disqus.com/kb/terms-and-policies/
  version: 1.0.0
host: disqus.com
basePath: api/3.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /posts/spam.json:
    post:
      summary: Posts Spam
      description: "\n     Posts Spam "
      operationId: posts-spam
      parameters:
      - in: query
        name: post
        description: Looks up a post by ID You must be a moderator on the selected
          post&#39;s forum
        type: string
      responses:
        200:
          description: OK
      tags:
      - comments
      - posts
      - spam
definitions: []
x-collection-name: Disqus
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
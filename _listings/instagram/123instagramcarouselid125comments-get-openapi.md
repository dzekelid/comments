---
swagger: "2.0"
x-collection-name: Instagram
x-complete: 0
info:
  title: Instagram Instagram Carousel Comments
  version: 1.0.0
  description: Instagram Carousel Comments
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;instagram-media-id&#125;/comments:
    get:
      summary: Instagram Media Comments
      description: Instagram Media Comments
      operationId: getInstagramMediaComments
      x-api-path-slug: 123instagrammediaid125comments-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - Media
      - Comments
  /&#123;instagram-carousel-id&#125;/comments:
    get:
      summary: Instagram Carousel Comments
      description: Instagram Carousel Comments
      operationId: getInstagramCarouselComments
      x-api-path-slug: 123instagramcarouselid125comments-get
      parameters:
      - in: query
        name: "100"
        description: Invalid parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - Carousel
      - Comments
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---
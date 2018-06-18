---
swagger: "2.0"
x-collection-name: Instagram
x-complete: 1
info:
  title: Instagram Graph API
  version: 1.0.0
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
  /&#123;instagram-carousel-id&#125;/instagram_comments:
    get:
      summary: Instagram Carousel Instagram Comments
      description: Instagram Carousel Instagram Comments
      operationId: getInstagramCarouselInstagramComments
      x-api-path-slug: 123instagramcarouselid125instagram-comments-get
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - Carousel
      - Instagram
      - Comments
---
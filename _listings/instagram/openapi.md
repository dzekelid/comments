swagger: "2.0"
x-collection-name: Instagram
x-complete: 1
info:
  title: Instagram
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
  /&#123;instagram-comment-id&#125;:
    get:
      summary: Instagram Comment
      description: Instagram Comment
      operationId: getInstagramComment
      x-api-path-slug: 123instagramcommentid125-get
      parameters:
      - in: query
        name: comment_typeenum
        description: Enum indicating the type of comment &#123;CAPTION, NORMAL, UNKNOWN&#125;
        type: string
      - in: query
        name: created_atdatetime
        description: Creation time of the comment in milliseconds
        type: string
      - in: query
        name: idstring
        description: Base 64 encoded string of instagram_media_id and instagram_comment_id
        type: string
      - in: query
        name: instagram_comment_idnumeric string
        description: Id of the comment in instagram
        type: string
      - in: query
        name: instagram_userInstagramUser
        description: Instagram user who made the comment
        type: string
      - in: query
        name: mentioned_instagram_userslistInstagramUser
        description: Instagram users that are mentioned in the comment
        type: string
      - in: query
        name: messagestring
        description: Textual message content of the Instagram comment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - Comment
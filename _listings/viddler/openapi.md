---
swagger: "2.0"
x-collection-name: Viddler
x-complete: 1
info:
  title: Viddler  API
  description: the-viddler-api-exposes-viddleru2019s-key-features-to-those-that-would-like-to-build-custom-solutions-on-top-of-viddleru2019s-video-platform-
  termsOfService: http://www.viddler.com/terms-of-use/
  version: v2
host: api.viddler.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  viddler.videos.comments.get:
    get:
      summary: Videos Comments Get
      description: Get comments for a video. If logged in and querying comments for
        own video &#8211; all comments with any moderation status will be returned.
        If quering comments as logged out or for not owned video &#8211; only approved
        comments will be returned if the video itself is public.
      operationId: videos-comments-get
      x-api-path-slug: viddler-videos-comments-get-get
      parameters:
      - in: query
        name: page
      - in: query
        name: parent_id
        description: comment parent ID if you want to get the responses to that particular
          comment
      - in: query
        name: per_page
      - in: query
        name: sessionid
      - in: query
        name: video_id
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - Comments
      - Get
---
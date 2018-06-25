---
name: Viddler
x-slug: viddler
description: www.viddler.com
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/274-viddler.jpg
x-kinRank: "8"
x-alexaRank: "81111"
tags: Comments
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/viddler/apis.md
specificationVersion: "0.14"
apis:
- name: Viddler  API Videos Comments Get
  x-api-slug: viddler--api
  description: Get comments for a video. If logged in and querying comments for own
    video &#8211; all comments with any moderation status will be returned. If quering
    comments as logged out or for not owned video &#8211; only approved comments will
    be returned if the video itself is public.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/274-viddler.jpg
  humanURL: http://www.viddler.com/
  baseURL: https://api.viddler.com//api/v2/viddler.videos.comments.get
  tags: Viddler,Videos,Comments,Get
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/viddler/viddler-videos-comments-get-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/viddler/viddler-videos-comments-get-get-openapi.md
- name: Viddler  API
  x-api-slug: viddler--api
  description: The Viddler API exposes Viddler&rsquo;s key features to those that
    would like to build custom solutionson topof Viddler&rsquo;s video platform.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/274-viddler.jpg
  humanURL: http://www.viddler.com/
  baseURL: https://api.viddler.com//api/v2
  tags: Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/viddler/openapi.md
x-common:
- type: x-base
  url: http://api.viddler.com/api/
- type: x-blog
  url: http://blog.viddler.com/
- type: x-blog-rss
  url: http://blog.viddler.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/viddler
- type: x-crunchbase
  url: https://crunchbase.com/organization/viddler
- type: x-developer
  url: http://developers.viddler.com/
- type: x-email
  url: sales@viddler.com
- type: x-email
  url: privacy@viddler.com
- type: x-email
  url: support@viddler.com
- type: x-email
  url: copyright@viddler.com
- type: x-faq
  url: http://www.viddler.com/help/
- type: x-github
  url: https://github.com/viddler
- type: x-google-plus
  url: https://plus.google.com/+viddler
- type: x-privacy
  url: http://www.viddler.com/privacy-policy/
- type: x-terms-of-service
  url: http://www.viddler.com/terms-of-use/
- type: x-twitter
  url: https://twitter.com/viddler
- type: x-website
  url: http://www.viddler.com/
- type: x-website
  url: http://viddler.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---
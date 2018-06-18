---
name: AngelList
x-slug: angellist
description: AngelList is where the world meets startups. Find a great startup job,
  invest in a startup, or raise money
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
x-kinRank: "9"
x-alexaRank: "2447"
tags: Comments
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/angellist/apis.md
specificationVersion: "0.14"
apis:
- name: AngelList Get Comments
  x-api-slug: angellist
  description: Pulls the comments for given object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///comments
  tags: Startups,Businesses,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/angellist/comments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/angellist/comments-get-openapi.md
- name: AngelList Add Comment
  x-api-slug: angellist
  description: Adds a comment for given object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///comments
  tags: Startups,Businesses,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/angellist/comments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/angellist/comments-post-openapi.md
- name: AngelList Delete Comment
  x-api-slug: angellist
  description: Deletes a comment for given object
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///comments/{comment_id}
  tags: Startups,Businesses,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/angellist/commentscomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/angellist/commentscomment-id-delete-openapi.md
- name: AngelList Get Startup Comments
  x-api-slug: angellist
  description: Get Startup Comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1///startups/{startup_id}/comments
  tags: Startups,Businesses,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/angellist/startupsstartup-idcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/angellist/startupsstartup-idcomments-get-openapi.md
- name: AngelList
  x-api-slug: angellist
  description: AngelList is where the world meets startups. Find a great startup job,
    invest in a startup, or raise money
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/339-angellist.jpg
  humanURL: http://angel.co
  baseURL: https://api.angel.co//1/
  tags: Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/angellist/openapi.md
x-common:
- type: x-blog
  url: https://blog.angel.co
- type: x-base-url
  url: http://api.angel.co/
- type: x-blog
  url: http://blog.angel.co
- type: x-blog-rss
  url: http://blog.angel.co/rss
- type: x-crunchbase
  url: http://www.crunchbase.com/company/angellist
- type: x-crunchbase
  url: https://crunchbase.com/organization/angellist
- type: x-developer
  url: https://angel.co/api
- type: x-email
  url: copyright@angel.co
- type: x-email
  url: syndicates@angel.co
- type: x-email
  url: team@angel.co
- type: x-email
  url: talent@angel.co
- type: x-email
  url: privacy@angel.co
- type: x-email
  url: abuse@angel.co
- type: x-github
  url: https://github.com/angellist
- type: x-postman-collection
  url: http://theapistack.com/data/angellist/angellist-postman-collection.json
- type: x-privacy
  url: https://angel.co/privacy
- type: x-sdks-io
  url: https://sdks.io/SDK/View/angellist-startup-api
- type: x-support
  url: https://angel.co/help
- type: x-terms-of-service
  url: https://angel.co/terms
- type: x-twitter
  url: https://twitter.com/angellist
- type: x-website
  url: http://angel.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---
---
name: Facebook
x-slug: facebook
description: Create an account or log into Facebook. Connect with friends, family
  and other people you know. Share photos and videos, send messages and get updates.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
x-kinRank: "9"
x-alexaRank: "3"
tags: Comments
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/apis.md
specificationVersion: "0.14"
apis:
- name: Facebook Get Album Comments
  x-api-slug: facebook
  description: The comments made on this album
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{album}/comments
  tags: Album,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/albumcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/albumcomments-get-openapi.md
- name: Facebook Post Album Comments
  x-api-slug: facebook
  description: Posts a comment on the album
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{album}/comments
  tags: Album,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/albumcomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/albumcomments-post-openapi.md
- name: Facebook Get Checkin Comments
  x-api-slug: facebook
  description: All of the comments on this checkin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{checkin}/comments
  tags: Checkin,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/checkincomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/checkincomments-get-openapi.md
- name: Facebook Post Checkin Comments
  x-api-slug: facebook
  description: Posts a comment to this checkin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{checkin}/comments
  tags: Checkin,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/checkincomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/checkincomments-post-openapi.md
- name: Facebook Get Link Comments
  x-api-slug: facebook
  description: All of the comments on this link.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{link}/comments
  tags: Link,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/linkcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/linkcomments-get-openapi.md
- name: Facebook Post Link Comments
  x-api-slug: facebook
  description: Posts a comment to this link.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{link}/comments
  tags: Link,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/linkcomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/linkcomments-post-openapi.md
- name: Facebook Get Note Comments
  x-api-slug: facebook
  description: All of the comments on this note.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{note}/comments
  tags: Note,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/notecomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/notecomments-get-openapi.md
- name: Facebook Post Note Comments
  x-api-slug: facebook
  description: Posts a comment to this note.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{note}/comments
  tags: Note,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/notecomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/notecomments-post-openapi.md
- name: Facebook Get Photo Comments
  x-api-slug: facebook
  description: All of the comments on this photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{photo}/comments
  tags: Photo,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/photocomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/photocomments-get-openapi.md
- name: Facebook Post Photo Comments
  x-api-slug: facebook
  description: Posts a comment to this photo.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{photo}/comments
  tags: Photo,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/photocomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/photocomments-post-openapi.md
- name: Facebook Get Add Comments
  x-api-slug: facebook
  description: All of the comments on this post.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{post}/comments
  tags: Post,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/postcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/postcomments-get-openapi.md
- name: Facebook Post Add Comments
  x-api-slug: facebook
  description: Posts a comment to this post.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{post}/comments
  tags: Post,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/postcomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/postcomments-post-openapi.md
- name: Facebook Get Status Comments
  x-api-slug: facebook
  description: All of the comments on this status.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{status}/comments
  tags: Status,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/statuscomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/statuscomments-get-openapi.md
- name: Facebook Post Status Comments
  x-api-slug: facebook
  description: Posts a comment to this status.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{status}/comments
  tags: Status,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/statuscomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/statuscomments-post-openapi.md
- name: Facebook Get Veo Comments
  x-api-slug: facebook
  description: All of the comments on this video.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{video}/comments
  tags: Video,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/videocomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/videocomments-get-openapi.md
- name: Facebook Post Veo Comments
  x-api-slug: facebook
  description: Posts a comment to this video.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com////{video}/comments
  tags: Video,Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/videocomments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/videocomments-post-openapi.md
- name: Facebook
  x-api-slug: facebook
  description: Create an account or log into Facebook. Connect with friends, family
    and other people you know. Share photos and videos, send messages and get updates.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/196-facebook.jpg
  humanURL: http:///business
  baseURL: https://graph.facebook.com//
  tags: Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/facebook/openapi.md
x-common:
- type: x-android-sdk
  url: https://developers.facebook.com/docs/android/share
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/facebook/apidescription?format=internal&ver=1386216190000
- type: x-application-gallery
  url: https://developers.facebook.com/docs/showcase/
- type: x-base
  url: https://graph.facebook.com
- type: x-best-practices
  url: https://developers.facebook.com/docs/sharing/best-practices
- type: x-blog
  url: http://blog.facebook.com
- type: x-blog-rss
  url: https://www.facebook.com/business/news/rss/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/facebook
- type: x-crunchbase
  url: https://crunchbase.com/organization/facebook
- type: x-developer
  url: https://developers.facebook.com/
- type: x-forum
  url: https://www.facebook.com/groups/fbdevelopers
- type: x-github
  url: https://github.com/facebook
- type: x-ios-sdk
  url: https://developers.facebook.com/docs/ios/share
- type: x-issues
  url: https://developers.facebook.com/status/issues/
- type: x-javascript-library
  url: https://developers.facebook.com/docs/reference/javascript/
- type: x-partners
  url: https://facebookmarketingpartners.com/
- type: x-php-sdk
  url: https://developers.facebook.com/docs/reference/php/
- type: x-plugins
  url: https://developers.facebook.com/docs/plugins/
- type: x-privacy
  url: https://www.facebook.com/settings?tab=privacy
- type: x-road-map
  url: https://developers.facebook.com/docs/apps/migrations
- type: x-status
  url: https://developers.facebook.com/status/
- type: x-terms-of-service
  url: https://www.facebook.com/terms
- type: x-terms-of-service
  url: https://developers.facebook.com/policy
- type: x-transparency-report
  url: https://www.facebook.com/about/government_requests
- type: x-twitter
  url: https://twitter.com/facebook
- type: x-website
  url: http:///business
- type: x-website
  url: http://facebook.com
- type: x-website
  url: https://facebook.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---
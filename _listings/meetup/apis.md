---
name: Meetup
x-slug: meetup
description: Find Meetups so you can do more of what matters to you. Or create your
  own group and meet people near you who share your interests.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
x-kinRank: "9"
x-alexaRank: "902"
tags: Comments
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/apis.md
specificationVersion: "0.14"
apis:
- name: Meetup Comments
  x-api-slug: meetup
  description: API method for accessing meetup group comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////comments
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/comments-get-openapi.md
- name: Meetup Comments v2
  x-api-slug: meetup
  description: This method returns messages that appear under Talk about this Meetup.
    To post messages, see the corresponding write method.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_comments
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2event-comments-get-openapi.md
- name: Meetup Event Comment v2
  x-api-slug: meetup
  description: This method posts messages that appear under Talk about this Meetup.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_comment
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2event-comment-post-openapi.md
- name: Meetup Event Comment Get
  x-api-slug: meetup
  description: Retrieve a single event comment or reply
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_comment/:id
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2event-commentid-get-openapi.md
- name: Meetup Event Comment Delete
  x-api-slug: meetup
  description: Delete a single event comment or reply
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_comment/:id
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2event-commentid-delete-openapi.md
- name: Meetup Event Comment Flag
  x-api-slug: meetup
  description: This method creates a spam report for comment content
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_comment_flag
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2event-comment-flag-post-openapi.md
- name: Meetup Event Comment Unsubscribe
  x-api-slug: meetup
  description: Unsubscribe to notifications for updates to a given comment thread
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_comment_subscribe/:id
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2event-comment-subscribeid-delete-openapi.md
- name: Meetup Event Comment Like
  x-api-slug: meetup
  description: Like a given Event comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_comment_like/:id
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2event-comment-likeid-post-openapi.md
- name: Meetup Event Comment Unlike
  x-api-slug: meetup
  description: Unlike a given Event comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_comment_like/:id
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2event-comment-likeid-delete-openapi.md
- name: Meetup Comment Likes
  x-api-slug: meetup
  description: Api for listing likes of a given event comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_comment_likes
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2event-comment-likes-get-openapi.md
- name: Meetup Photo Comment v2
  x-api-slug: meetup
  description: This method posts comments that appear below photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/photo_comment
  tags: Events,Photos,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2photo-comment-post-openapi.md
- name: Meetup Photo Albums
  x-api-slug: meetup
  description: This method returns photo albums associated with Meetup groups. To
    create albums, see the corresponding write method.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/photo_albums
  tags: Events,Photos,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2photo-albums-get-openapi.md
- name: Meetup WebSockets Event Comments Stream
  x-api-slug: meetup
  description: |-
    For browsers that support it, [WebSockets](http://dev.w3.org/html5/websockets/) is a more
    efficient alternative to the long-polling stream. This is a **push only** endpoint and will discard
    any messages received from the client after the socket is open.

    Because browser support for WebSockets is limited, we recommend that you consume this stream
    through the [must.js](https://github.com/meetup/must.js#readme) client, which can fallback to long-polling.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_comments
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/2event-comments-ws-openapi.md
- name: Meetup Event Comments List
  x-api-slug: meetup
  description: |-
    Lists the comments and replies posted in a given Meetup Event.

    To view the list of likes for a comment or reply
    see the [likes](/meetup_api/docs/:urlname/events/:event_id/comments/:comment_id/likes/)
    endpoint
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/events/:event_id/comments
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/urlnameeventsevent-idcomments-get-openapi.md
- name: Meetup Event comment and reply
  x-api-slug: meetup
  description: Creates new comments and replies to existing comments within an Meetup
    event
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/events/:event_id/comments
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/urlnameeventsevent-idcomments-post-openapi.md
- name: Meetup Event comment delete
  x-api-slug: meetup
  description: Deletes comments posted in events
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/events/:event_id/comments/:comment_id
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/urlnameeventsevent-idcommentscomment-id-delete-openapi.md
- name: Meetup Event Comment and Reply Likes
  x-api-slug: meetup
  description: Returns lists of likes for an event comment or reply
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/events/:event_id/comments/:comment_id/likes
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/urlnameeventsevent-idcommentscomment-idlikes-get-openapi.md
- name: Meetup Event Comment Unlike
  x-api-slug: meetup
  description: Unlike a given event comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/events/:event_id/comments/:comment_id/likes
  tags: Events,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/urlnameeventsevent-idcommentscomment-idlikes-delete-openapi.md
- name: Meetup Photo Comment
  x-api-slug: meetup
  description: Creates a new photo comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/events/:event_id/photos/:photo_id/comments
  tags: Events,Photos,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/urlnameeventsevent-idphotosphoto-idcomments-post-openapi.md
- name: Meetup Photo Comment Delete
  x-api-slug: meetup
  description: Deletes photo comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/events/:event_id/photos/:photo_id/comments/:comment_id
  tags: Events,Photos,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/urlnameeventsevent-idphotosphoto-idcommentscomment-id-delete-openapi.md
- name: Meetup Photo Comments
  x-api-slug: meetup
  description: Lists photo comments associated with a photo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/events/:event_id/photos/:photo_id/comments
  tags: Events,Photos,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/urlnameeventsevent-idphotosphoto-idcomments-get-openapi.md
- name: Meetup
  x-api-slug: meetup
  description: Find Meetups so you can do more of what matters to you. Or create your
    own group and meet people near you who share your interests.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/meetup/openapi.md
x-common:
- type: x-base
  url: http://api.meetup.com
- type: x-crunchbase
  url: https://crunchbase.com/organization/meetup
- type: x-developer
  url: http://www.meetup.com/meetup_api/
- type: x-email
  url: privacy@meetup.com
- type: x-email
  url: abuse@meetup.com
- type: x-email
  url: api_license@meetup.com
- type: x-email
  url: arbitration-opt-out@meetup.com
- type: x-email
  url: legal@meetup.com
- type: x-github
  url: https://github.com/meetup
- type: x-pricing
  url: http://www.meetup.com/pricing/
- type: x-privacy
  url: http://www.meetup.com/privacy/
- type: x-support
  url: http://www.meetup.com/help/
- type: x-terms-of-service
  url: http://www.meetup.com/terms/
- type: x-twitter
  url: https://twitter.com/MeetupAPI
- type: x-twitter
  url: https://twitter.com/Meetup
- type: x-website
  url: http://meetup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---
---
name: Blogger
x-slug: blogger
description: Blogger is a blog-publishing service that allows multi-user blogs with
  time-stamped entries. It was developed by Pyra Labs, which was bought by Google
  in 2003. Generally, the blogs are hosted by Google at a subdomain of blogspot.com.
  Blogs can also be hosted in the registered custom domain of the blogger (like www.example.com).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Comments
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/apis.md
specificationVersion: "0.14"
apis:
- name: Blogger API Get Blog Post Comments
  x-api-slug: blogger-api
  description: Retrieves the comments for a post, possibly filtered.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcomments-get-openapi.md
- name: Blogger API Delete Blog Post Comments
  x-api-slug: blogger-api
  description: Delete a comment by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments/{commentId}
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcommentscommentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcommentscommentid-delete-openapi.md
- name: Blogger API Get Blog Post Comment
  x-api-slug: blogger-api
  description: Gets one comment by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments/{commentId}
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcommentscommentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcommentscommentid-get-openapi.md
- name: Blogger API Update Blog Post Comment
  x-api-slug: blogger-api
  description: Marks a comment as not spam.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments/{commentId}/approve
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcommentscommentidapprove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcommentscommentidapprove-post-openapi.md
- name: Blogger API Update Blog Post Comment
  x-api-slug: blogger-api
  description: Removes the content of a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments/{commentId}/removecontent
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcommentscommentidremovecontent-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcommentscommentidremovecontent-post-openapi.md
- name: Blogger API Update Blog Post Comment SPAM
  x-api-slug: blogger-api
  description: Marks a comment as spam.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments/{commentId}/spam
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcommentscommentidspam-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/blogsblogidpostspostidcommentscommentidspam-post-openapi.md
- name: Blogger API
  x-api-slug: blogger-api
  description: The Blogger API v3 allows client applications to view and update Blogger
    content. Your client application can use Blogger API v3 to create new blog posts,
    edit or delete existing posts, and query for posts that match particular criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/blogger/openapi.md
x-common:
- type: x-blog
  url: https://blogger.googleblog.com/
- type: x-website
  url: https://www.blogger.com
- type: x-blog-rss
  url: http://buzz.blogger.com/atom.xml
- type: x-developer
  url: https://developers.google.com/blogger/
- type: x-twitter
  url: https://twitter.com/Blogger
- type: x-getting-started
  url: https://developers.google.com/blogger/docs/3.0/getting_started
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---
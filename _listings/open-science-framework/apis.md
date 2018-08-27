---
name: Open Science Framework
x-slug: open-science-framework
description: OSF provides free and open source project management support for researchers
  across the entire research lifecycle. As a collaboration tool, OSF helps researchers
  work on projects privately with a limited number of collaborators and make parts
  of their projects public, or make all the project publicly accessible for broader
  dissemination. As a workflow system, OSF enables connections to the many services
  researchers already use to streamline their process and increase efficiency. As
  a flexible repository, it can store and archive research data, protocols, and materials.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Comments
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/apis.md
specificationVersion: "0.14"
apis:
- name: Open Science Framework - Delete a comment
  x-api-slug: commentscomment-id-delete
  description: |-
    Deletes a comment. This action can be undone by setting deleted to False in a comment update request.
    #### Returns
    If the request is successful, no content is returned.

    If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-delete-openapi.md
- name: Open Science Framework - Retrieve a comment
  x-api-slug: commentscomment-id-get
  description: |-
    Retrieves the details of a comment
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested comment, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-get-openapi.md
- name: Open Science Framework - Update a comment
  x-api-slug: commentscomment-id-put
  description: |-
    Updates the specified comment by setting the values of the parameters passed. Any parameters not provided will be left unchanged.
    #### Returns
    Returns JSON with a `data` key containing the new representation of the updated comment, if the request is successful.

    If the request is unsuccessful, JSON with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-put-openapi.md
- name: Open Science Framework - List all comments
  x-api-slug: nodesnode-idcomments-get
  description: |-
    A paginated list of comments related to a given node.

    The returned comments are sorted by their creation date, with the most recent comments appearing first.
    ####Permissions
    Comments on public nodes are given read-only access to everyone.

    If the node comment-level is `private`, only contributors have permission to comment.

    If the comment-level is `public`, any logged-in OSF user can comment.

    Comments on private nodes are only visible to contributors and administrators on the parent node.
    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of comment objects. Each resource in the array is a separate comment object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    #### Filtering
    You can optionally request that the response only include comments that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/ezcuj/comments/?filter[target_id]=jg7sezmdnt93

    Nodes may be filtered by their `deleted`, `target_id`, `date_created`, `date_modified`.

    Most fields are string fields and will be filtered using simple substring matching. Public and preprint are boolean fields, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting `true` or `false` in the query will cause the match to fail.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/nodesnode-idcomments-get-openapi.md
- name: Open Science Framework - Create a comment
  x-api-slug: nodesnode-idcomments-post
  description: |-
    Create a comment on a given node overview page or a reply to a comment on that node.

    To create a comment on the node overview page, the target `type` would be "nodes" and the target `id` would be the node `id`.

    To reply to a comment on this node, the target `type` would be "comments" and the target `id` would be the `id` of the comment to reply to.
    ####Required
    A relationship object with a `data` key, containing the target (`comments` or `nodes`) type and a target `id` is required.
    In addition, the `content` attribute describing the relationship between the node and the comment is required.
    ####Returns
    Returns a JSON object with a data key containing the representation of the new comment, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/nodesnode-idcomments-post-openapi.md
- name: Open Science Framework - List all comments
  x-api-slug: registrationsregistration-idcomments-get
  description: |-
    A paginated list of the registration's comments.

    The returned comments are sorted by their creation date, with the most recent comments appearing first.
    ####Permissions
    Comments of public registrations are given read-only access to everyone.

    If the comment-level is `private`, only registration contributors have permission to comment.

    If the comment-level is `public`, any logged-in OSF user can comment.

    Comments of private registrations are only visible to contributors and administrators on the registration.
    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of comment objects. Each resource in the array is a separate comment object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    #### Filtering
    You can optionally request that the response only include comments that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wuerf/comments/?filter[target]=wuerf

    Comments may be filtered by their `deleted`, `target`, `date_created`, `date_modified`.

    Most fields are string fields and will be filtered using simple substring matching. Deleted is a boolean field, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting `true` or `false` in the query will cause the match to fail.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/registrationsregistration-idcomments-get-openapi.md
- name: Open Science Framework - Delete a comment
  x-api-slug: commentscomment-id-delete
  description: |-
    Deletes a comment. This action can be undone by setting deleted to False in a comment update request.
    #### Returns
    If the request is successful, no content is returned.

    If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-delete-openapi.md
- name: Open Science Framework - Retrieve a comment
  x-api-slug: commentscomment-id-get
  description: |-
    Retrieves the details of a comment
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested comment, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-get-openapi.md
- name: Open Science Framework - Update a comment
  x-api-slug: commentscomment-id-put
  description: |-
    Updates the specified comment by setting the values of the parameters passed. Any parameters not provided will be left unchanged.
    #### Returns
    Returns JSON with a `data` key containing the new representation of the updated comment, if the request is successful.

    If the request is unsuccessful, JSON with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-put-openapi.md
- name: Open Science Framework - Actions
  x-api-slug: actions-get
  description: |-
    A log can have one of many actions. The complete list of loggable actions (in the format {identifier}: {description}) is as follows:
    * `project_created`: A Node is created
    * `project_registered`: A Node is registered
    * `project_deleted`: A Node is deleted
    * `created_from`: A Node is created using an existing Node as a template
    * `pointer_created`: A Pointer is created
    * `pointer_forked`: A Pointer is forked
    * `pointer_removed`: A Pointer is removed
    * `node_removed`: A component is deleted
    * `node_forked`: A Node is forked
    ---
    * `made_public`: A Node is made public
    * `made_private`: A Node is made private
    * `tag_added`: A tag is added to a Node
    * `tag_removed`: A tag is removed from a Node
    * `edit_title`: A Node's title is changed
    * `edit_description`: A Node's description is changed
    * `updated_fields`: One or more of a Node's fields are changed
    * `external_ids_added`: An external identifier is added to a Node (e.g. DOI, ARK)
    * `view_only_link_added`: A view-only link was added to a Node
    * `view_only_link_removed`:  A view-only link was removed from a Node
    ---
    * `contributor_added`: A Contributor is added to a Node
    * `contributor_removed`: A Contributor is removed from a Node
    * `contributors_reordered`: A Contributor's position in a Node's bibliography is changed
    * `permissions_updated`: A Contributor`s permissions on a Node are changed
    * `made_contributor_visible`: A Contributor is made bibliographically visible on a Node
    * `made_contributor_invisible`: A Contributor is made bibliographically invisible on a Node
    ---
    * `wiki_updated`: A Node's wiki is updated
    * `wiki_deleted`: A Node's wiki is deleted
    * `wiki_renamed`: A Node's wiki is renamed
    * `made_wiki_public`: A Node's wiki is made public
    * `made_wiki_private`: A Node's wiki is made private
    ---
    * `addon_added`: An add-on is linked to a Node
    * `addon_removed`: An add-on is unlinked from a Node
    * `addon_file_moved`: A File in a Node's linked add-on is moved
    * `addon_file_copied`: A File in a Node's linked add-on is copied
    * `addon_file_renamed`: A File in a Node's linked add-on is renamed
    * `node_authorized`: An addon is authorized for a project
    * `node_deauthorized`: An addon is deauthorized for a project
    * `folder_created`: A Folder is created in a Node's linked add-on
    * `file_added`: A File is added to a Node's linked add-on
    * `file_updated`: A File is updated on a Node's linked add-on
    * `file_removed`: A File is removed from a Node's linked add-on
    * `file_restored`: A File is restored in a Node's linked add-on
    ---
    * `comment_added`: A Comment is added to some item
    * `comment_removed`: A Comment is removed from some item
    * `comment_updated`: A Comment is updated on some item
    ---
    * `embargo_initiated`: An embargoed Registration is proposed on a Node
    * `embargo_approved`: A proposed Embargo of a Node is approved
    * `embargo_cancelled`: A proposed Embargo of a Node is cancelled
    * `embargo_completed`: A proposed Embargo of a Node is completed
    * `retraction_initiated`: A Withdrawal of a Registration is proposed
    * `retraction_approved`: A Withdrawal of a Registration is approved
    * `retraction_cancelled`: A Withdrawal of a Registration is cancelled
    * `registration_initiated`: A Registration of a Node is proposed
    * `registration_approved`: A proposed Registration is approved
    * `registration_cancelled`: A proposed Registration is cancelled
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/actions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/actions-get-openapi.md
- name: Open Science Framework - Update a comment
  x-api-slug: commentscomment-id-put
  description: |-
    Updates the specified comment by setting the values of the parameters passed. Any parameters not provided will be left unchanged.
    #### Returns
    Returns JSON with a `data` key containing the new representation of the updated comment, if the request is successful.

    If the request is unsuccessful, JSON with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-put-openapi.md
- name: Open Science Framework - Retrieve a comment
  x-api-slug: commentscomment-id-get
  description: |-
    Retrieves the details of a comment
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested comment, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-get-openapi.md
- name: Open Science Framework - Delete a comment
  x-api-slug: commentscomment-id-delete
  description: |-
    Deletes a comment. This action can be undone by setting deleted to False in a comment update request.
    #### Returns
    If the request is successful, no content is returned.

    If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/comments/master/_listings/open-science-framework/commentscomment-id-delete-openapi.md
x-common:
- type: x-website
  url: https://cos.io
- type: x-api-gallery
  url: http://open.fintech.api.gallery.streamdata.io
- type: x-api-stack
  url: http://open.science.framework.stack.network
- type: x-github
  url: https://github.com/OSFramework
- type: x-twitter
  url: https://twitter.com/OSFramework
- type: x-website
  url: http://osf.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---
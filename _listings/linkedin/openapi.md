---
swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 1
info:
  title: LinkedIn
  description: bring-user-profiles-and-professional-networks-to-your-apps-
  version: 1.0.0
host: api.linkedin.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /companies/{id}/updates/key={update-key}/update-comments-as-company/:
    post:
      summary: Add Companies Updates Key Update Key Update Comments As Company
      description: Post companies  updates key update key update comments as company
      operationId: postCompaniesUpdatesKeyUpdateKeyUpdateCommentsAsCompany
      x-api-path-slug: companiesidupdateskeyupdatekeyupdatecommentsascompany-post
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Updates
      - Key
      - Update
      - Key
      - Update
      - Comments
      - As
      - Company
  /companies/{id}/updates/key={update-key}/update-comments:
    get:
      summary: Get Companies Updates Key Update Key Update Comments
      description: Get companies  updates key update key update comments
      operationId: getCompaniesUpdatesKeyUpdateKeyUpdateComments
      x-api-path-slug: companiesidupdateskeyupdatekeyupdatecomments-get
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Updates
      - Key
      - Update
      - Key
      - Update
      - Comments
---
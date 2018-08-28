---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Add Reuses Reuse Image
  description: Upload a new reuse image
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reuses/{reuse}/:
    delete:
      summary: Delete Reuses Reuse
      description: Delete a given reuse
      operationId: deleteReusesReuse
      x-api-path-slug: reusesreuse-delete
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
    get:
      summary: Get Reuses Reuse
      description: Fetch a given reuse
      operationId: getReusesReuse
      x-api-path-slug: reusesreuse-get
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
    put:
      summary: Put Reuses Reuse
      description: Update a given reuse
      operationId: putReusesReuse
      x-api-path-slug: reusesreuse-put
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
  /reuses/{reuse}/badges/:
    post:
      summary: Add Reuses Reuse Badges
      description: Create a new badge for a given reuse
      operationId: postReusesReuseBadges
      x-api-path-slug: reusesreusebadges-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Badges
  /reuses/{reuse}/badges/{badge_kind}/:
    delete:
      summary: Delete Reuses Reuse Badges Badge Kind
      description: Delete a badge for a given reuse
      operationId: deleteReusesReuseBadgesBadgeKind
      x-api-path-slug: reusesreusebadgesbadge-kind-delete
      parameters:
      - in: path
        name: badge_kind
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Badges
      - Badge
      - Kind
  /reuses/{reuse}/datasets/:
    post:
      summary: Add Reuses Reuse Datasets
      description: Add a dataset to a given reuse
      operationId: postReusesReuseDatasets
      x-api-path-slug: reusesreusedatasets-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Datasets
  /reuses/{reuse}/featured/:
    delete:
      summary: Delete Reuses Reuse Featured
      description: Unmark a reuse as featured
      operationId: deleteReusesReuseFeatured
      x-api-path-slug: reusesreusefeatured-delete
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Featured
    post:
      summary: Add Reuses Reuse Featured
      description: Mark a reuse as featured
      operationId: postReusesReuseFeatured
      x-api-path-slug: reusesreusefeatured-post
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Featured
  /reuses/{reuse}/image:
    post:
      summary: Add Reuses Reuse Image
      description: Upload a new reuse image
      operationId: postReusesReuseImage
      x-api-path-slug: reusesreuseimage-post
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Image
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---
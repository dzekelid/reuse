---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Get Reuses Reuse
  description: Fetch a given reuse
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